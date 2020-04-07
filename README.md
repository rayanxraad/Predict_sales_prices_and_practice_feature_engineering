
<img src="http://imgur.com/1ZcRyrc.png" style="float: left; margin: 20px; height: 55px">

# linear_predictors - DSI7 - Group 2

# Team Members:

- Rawan Almalki
- Rayan Raad
- Ghalib Tawfiq

# Kaggle Link:
- https://www.kaggle.com/ghalib93/house-prices?scriptVersionId=31096323

### missing data

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**MSZoning**|object|Test|['RH', 'RL', 'RM', 'FV', 'C (all)', nan]
|**Utilities**|object|Test|['AllPub', nan]-Type of utilities available|
|**Exterior1st**|object|Test|['VinylSd', 'Wd Sdng', 'HdBoard', 'Plywood', 'MetalSd','CemntBd','WdShing', 'BrkFace', 'AsbShng', 'BrkComm', 'Stucco', 'AsphShn',nan,'CBlock']-Exterior covering on house|
|**Exterior2nd**|object|train|['VinylSd', 'Wd Sdng', 'HdBoard', 'Plywood', 'MetalSd', 'Brk Cmn','CmentBd', 'Test', 'Wd Shng', 'AsbShng', 'Stucco', 'CBlock','BrkFace', 'AsphShn', nan, 'Stone']- Exterior covering on house (if more than one material)|
|**MasVnrType**|object|Test|['None', 'BrkFace', 'Stone', 'BrkCmn', nan]-Masonry veneer type|
|**BsmtQual**|object|Test|['TA', 'Gd', 'Ex', 'Fa', nan]-Evaluates the height of the basement|
|**KitchenQual**|object|Test|['TA', 'Gd', 'Ex', 'Fa', nan]- Kitchen quality|
|**Functional**|object|Test|['Typ', 'Min2', 'Min1', 'Mod', 'Maj1', 'Sev', 'Maj2', nan]-Home functionality (Assume typical unless deductions are warranted)|
|**MasVnrType**|object|Train|['BrkFace', 'None', 'Stone', 'BrkCmn', nan]-Masonry veneer type|
|**Electrical**|object|Train|['SBrkr', 'FuseF', 'FuseA', 'FuseP', 'Mix', nan]-Electrical system|






#####
### DATAFRAME
|**Feature**|**Type**|**Dataset**|**Description**|
|---|---|---|---|
|**MSSubClass**|object|Test |[20 ,60 ,120 ,160 ,80 ,30 ,50 ,90 ,85 ,190 ,45 , 70 ,75 ,180 ,40 ,150 ]-Identifies the type of dwelling involved in the sale|
|**MSZoning**|object|Test|['RH' ,'RL' ,'RM' ,'FV' , 'C (all)']-Identifies the general zoning classification of the sale.|
|**LotFrontage**|int64|Test|Linear feet of street connected to property|
|**LotArea**|int64|Test|Lot size in square feet|
|**Street**|object|Test|['Pave', 'Grvl']-Type of road access to property|
|**Alley**|object|Test|['NA','Pave', 'Grvl']-Type of alley access to property|
|**LotShape**|object|Test|['Reg', 'IR1', 'IR2', 'IR3']-General shape of property|
|**LandContour**|object|Test|['Lvl', 'HLS', 'Bnk', 'Low']-Flatness of the property|
|**Utilities**|object|Test|['AllPub']-Type of utilities available|
|**LotConfig**|object|Test|['Inside', 'Corner', 'FR2', 'CulDSac', 'FR3']-Lot configuration|
|**LandSlope**|object|Test|['Gtl', 'Mod', 'Sev']-Slope of property|
|**Neighborhood**|object|Test|['NAmes', 'Gilbert', 'StoneBr', 'BrDale', 'NPkVill','NridgHt','Blmngtn', 'NoRidge', 'Somerst', 'SawyerW', 'Sawyer', 'NWAmes','OldTown','BrkSide', 'ClearCr', 'SWISU', 'Edwards', 'CollgCr','Crawfor', 'Blueste','IDOTRR', 'Mitchel', 'Timber', 'MeadowV','Veenker']-Physical locations within Ames city limits|
|**Condition1**|object|Test|'Feedr', 'Norm', 'PosN', 'RRNe', 'Artery', 'RRNn', 'PosA', 'RRAn','RRAe']-Proximity to various conditions|
|**Condition2**|object|Test|['Norm', 'Feedr', 'PosA', 'PosN', 'Artery']-Proximity to various conditions (if more than one is present)|
|**BldgType**|object|Test|['1Fam', 'TwnhsE', 'Twnhs', 'Duplex', '2fmCon']-Type of dwelling|
|**HouseStyle**|object|Test|['1Story', '2Story', 'SLvl', '1.5Fin', 'SFoyer', '2.5Unf', '1.5Unf']-Style of dwelling|
|**OverallQual**|object|Test|[ 5,  6,  8,  7,  4,  9,  2,  3, 10,  1]-Rates the overall material and finish of the house|
|**OverallCond**|object|Test|[6, 5, 7, 8, 2, 9, 3, 4, 1]-Rates the overall condition of the house|
|**YearBuilt**|int64|Test|Original construction date|
|**YearRemodAdd**|int64|Test|Remodel date (same as construction date if no remodeling or additions)|
|**RoofStyle**|object|Test|['Gable', 'Hip', 'Gambrel', 'Flat', 'Mansard', 'Shed']- Type of roof|
|**RoofMatl**|object|Test|['CompShg', 'Tar&Grv', 'WdShake', 'WdShngl']-Roof material|
|**Exterior1st**|object|Test|['VinylSd', 'Wd Sdng', 'HdBoard', 'Plywood', 'MetalSd','CemntBd','WdShing', 'BrkFace', 'AsbShng', 'BrkComm', 'Stucco', 'AsphShn', 'CBlock']- Exterior covering on house|
|**Exterior2nd**|object|Test|['VinylSd', 'Wd Sdng', 'HdBoard', 'Plywood', 'MetalSd', 'Brk Cmn','CmentBd', 'ImStucc', 'Wd Shng', 'AsbShng', 'Stucco', 'CBlock','BrkFace', 'AsphShn', 'Stone']- Exterior covering on house (if more than one material)|
|**MasVnrType**|object|Test|['None', 'BrkFace', 'Stone', 'BrkCmn']-Masonry veneer type|
|**MasVnrArea**|flot|Test| Masonry veneer area in square feet|
|**ExterQual**|object|Test|['TA', 'Gd', 'Ex', 'Fa']-Evaluates the quality of the material on the exterior|
|**ExterCond**|object|Test|['TA', 'Gd', 'Fa', 'Po', 'Ex']-Evaluates the present condition of the material on the exterior|
|**Foundation**|object|Test|['CBlock', 'PConc', 'BrkTil', 'Stone', 'Slab', 'Wood']-Type of foundation|
|**BsmtQual**|object|Test|['TA', 'Gd', 'Ex', 'Fa']-Evaluates the height of the basement|
|**BsmtCond**|object|Test|['TA', 'Po', 'Fa', 'Gd', 'NA']-Evaluates the general condition of the basement|
|**BsmtExposure**|object|Test|['No', 'Gd', 'Mn', 'Av', 'NA']-Refers to walkout or garden level walls|
|**BsmtFinType1**|object|Test|['Rec', 'ALQ', 'GLQ', 'Unf', 'BLQ', 'LwQ', 'NA']- Rating of basement finished area|
|**BsmtFinSF1**|int64|Test|Type 1 finished square feet|
|**BsmtFinType2**|object|Test|['LwQ', 'Unf', 'Rec', 'BLQ', 'GLQ', 'ALQ','NA']-Rating of basement finished area (if multiple types)|
|**BsmtFinSF2**|int64|Test|Type 2 finished square feet|
|**BsmtUnfSF**|int64|Test| Unfinished square feet of basement area|
|**TotalBsmtSF**|int64|Test| Total square feet of basement area|
|**Heating**|object|Test|['GasA', 'GasW', 'Grav', 'Wall']- Type of heating|
|**HeatingQC**|object|Test|['TA', 'Gd', 'Ex', 'Fa', 'Po']- Heating quality and condition|
|**CentralAir**|object|Test|['Y', 'N']-Central air conditioning|
|**Electrical**|object|Test|['SBrkr', 'FuseA', 'FuseF', 'FuseP']-Electrical system|
|**1stFlrSF**|int64|Test|First Floor square feet|
|**2ndFlrSF**|int64|Test| Second floor square feet|
|**LowQualFinSF**|int64|Test|Low quality finished square feet (all floors)|
|**GrLivArea**|int64|Test|Above grade (ground) living area square feet|
|**BsmtFullBath**|int64|Test|Basement full bathrooms|
|**BsmtHalfBath**|int64|Test|Basement half bathrooms|
|**FullBath**|int64|Test| Full bathrooms above grade|
|**HalfBath**|int64|Test|Half baths above grade|
|**KitchenQual**|object|Test|['TA', 'Gd', 'Ex', 'Fa']- Kitchen quality|
|**TotRmsAbvGrd**|int64|Test|Total rooms above grade (does not include bathrooms)|
|**Functional**|object|Test|['Typ', 'Min2', 'Min1', 'Mod', 'Maj1', 'Sev', 'Maj2']-Home functionality (Assume typical unless deductions are warranted)|
|**Fireplaces**|int64|Test|Number of fireplaces|
|**FireplaceQu**|object|Test|['NA', 'TA', 'Gd', 'Po', 'Fa', 'Ex']- Fireplace quality|
|**GarageType**|object|Test|['Attchd', 'Detchd', 'BuiltIn', 'NA', 'Basment', '2Types', 'CarPort']- Garage location|
|**GarageYrBlt**|int64|Test|Year garage was built|
|**GarageFinish**|object|Test|['Unf', 'Fin', 'RFn', 'NA']-Interior finish of the garage|
|**GarageCars**|int64|Test|Size of garage in car capacity|
|**GarageArea**|int64|Test|Size of garage in square feet|
|**GarageQual**|object|Test|['TA', 'NA', 'Fa', 'Gd', 'Po']-Garage quality|
|**GarageCond**|object|Test|['TA', 'NA', 'Fa', 'Gd', 'Po', 'Ex']-Garage condition|
|**PavedDrive**|object|Test|'Y', 'N', 'P']-Paved driveway|
|**WoodDeckSF**|int64|Test|Wood deck area in square feet|
|**OpenPorchSF**|int64|Test|Open porch area in square feet|
|**EnclosedPorch**|int64|Test| Enclosed porch area in square feet|
|**3SsnPorch**|int64|Test| Three season porch area in square feet|
|**ScreenPorch**|int64|Test|Screen porch area in square feet|
|**PoolArea**|int64|Test|Pool area in square feet|
|**PoolQC**|int64|Test|['NA', 'Ex', 'Gd']-Pool quality|
|**Fence**|int64|Test|['MnPrv', 'NA', 'GdPrv', 'GdWo', 'MnWw']-Fence quality|
|**MiscVal**|int64|Test|$Value of miscellaneous feature|
|**MoSold**|int64|Test|Month Sold (MM)|
|**SaleType**|int64|Test|Year Sold (YYYY)|
|**SaleCondition**|object|Test|['Normal', 'Partial', 'Abnorml', 'Family', 'Alloca', 'AdjLand']-Condition of sale|
|**MSSubClass**|object|Train|[ 60,  20,  70,  50, 190,  45,  90, 120,  30,  85,  80, 160,75,180,  40]-Identifies the type of dwelling involved in the sale|
|**MSZoning**|object|Train|['RL', 'RM', 'C (all)', 'FV', 'RH']-Identifies the general zoning classification of the sale.|
|**LotFrontage**|int64|Train|Linear feet of street connected to property|
|**LotArea**|int64|Train|Lot size in square feet|
|**Street**|object|Train|['Pave', 'Grvl']-Type of road access to property|
|**Alley**|object|Train|['NA','Pave', 'Grvl']-Type of alley access to property|
|**LotShape**|object|Train|['Reg', 'IR1', 'IR2', 'IR3']-General shape of property|
|**LandContour**|object|Train|['Lvl', 'HLS', 'Bnk', 'Low']-Flatness of the property|
|**Utilities**|object|Train|['AllPub', 'NoSeWa']-Type of utilities available|
|**LotConfig**|object|Train|['Inside', 'Corner', 'FR2', 'CulDSac', 'FR3']-Lot configuration|
|**LandSlope**|object|Train|['Gtl', 'Mod', 'Sev']-Slope of property|
|**Neighborhood**|object|Train|['CollgCr', 'Veenker', 'Crawfor', 'NoRidge', 'Mitchel','Somerst','NWAmes', 'OldTown', 'BrkSide', 'Sawyer', 'NridgHt', 'NAmes','SawyerW', 'IDOTRR', 'MeadowV', 'Edwards', 'Timber', 'Gilbert','StoneBr', 'ClearCr', 'NPkVill', 'Blmngtn', 'BrDale', 'SWISU','Blueste']-Physical locations within Ames city limits|
|**Condition1**|object|Train|['Norm', 'Feedr', 'PosN', 'Artery', 'RRAe', 'RRNn','RRAn','PosA','RRNe']-Proximity to various conditions|
|**Condition2**|object|Train|['Norm', 'Artery', 'RRNn', 'Feedr', 'PosN', 'PosA', 'RRAn','RRAe']-Proximity to various conditions (if more than one is present)|
|**BldgType**|object|Train|['1Fam', '2fmCon', 'Duplex', 'TwnhsE', 'Twnhs']-Type of dwelling|
|**HouseStyle**|object|Train|['2Story', '1Story', '1.5Fin', '1.5Unf', 'SFoyer','SLvl','2.5Unf','2.5Fin']-Style of dwelling|
|**OverallQual**|object|Train|[ 5,  6,  8,  7,  4,  9,  2,  3, 10,  1]-Rates the overall material and finish of the house|
|**OverallCond**|object|Train|[6, 5, 7, 8, 2, 9, 3, 4, 1]-Rates the overall condition of the house|
|**YearBuilt**|int64|Train**|Original construction date|
|**YearRemodAdd**|int64|Train|Remodel date (same as construction date if no remodeling or additions)|
|**RoofStyle**|object|Train|['Gable', 'Hip', 'Gambrel', 'Flat', 'Mansard', 'Shed']- Type of roof|
|**RoofMatl**|object|Train|['CompShg', 'WdShngl', 'Metal', 'WdShake', 'Membran','Tar&Grv','Roll', 'ClyTile']-Roof material|
|**Exterior1st**|object|Train|['VinylSd', 'MetalSd', 'Wd Sdng', 'HdBoard', 'BrkFace','WdShing','CemntBd', 'Plywood', 'AsbShng', 'Stucco', 'BrkComm', 'AsphShn','Stone', 'ImStucc', 'CBlock']- Exterior covering on house|
|**Exterior2nd**|object|Train|['VinylSd', 'Wd Sdng', 'HdBoard', 'Plywood', 'MetalSd', 'Brk Cmn','CmentBd', 'ImStucc', 'Wd Shng', 'AsbShng', 'Stucco', 'CBlock','BrkFace', 'AsphShn', 'Stone']- Exterior covering on house (if more than one material)|
|**MasVnrType**|object|Train|['BrkFace', 'None', 'Stone', 'BrkCmn']-Masonry veneer type|
|**MasVnrArea**|flot|Train| Masonry veneer area in square feet|
|**ExterQual**|object|Train|['TA', 'Gd', 'Ex', 'Fa']-Evaluates the quality of the material on the exterior|
|**ExterCond**|object|Train|['TA', 'Gd', 'Fa', 'Po', 'Ex']-Evaluates the present condition of the material on the exterior|
|**Foundation**|object|Train|['CBlock', 'PConc', 'BrkTil', 'Stone', 'Slab', 'Wood']-Type of foundation|
|**BsmtQual**|object|Train|['Gd', 'TA', 'Ex', 'NA', 'Fa']-Evaluates the height of the basement|
|**BsmtCond**|object|Train|['TA', 'Po', 'Fa', 'Gd', 'NA']-Evaluates the general condition of the basement|
|**BsmtExposure**|object|Train|['No', 'Gd', 'Mn', 'Av', 'NA']-Refers to walkout or garden level walls|
|**BsmtFinType1**|object|Train|['Rec', 'ALQ', 'GLQ', 'Unf', 'BLQ', 'LwQ', 'NA']- Rating of basement finished area|
|**BsmtFinSF1**|int64|Train|Type 1 finished square feet|
|**BsmtFinType2**|object|Train|['LwQ', 'Unf', 'Rec', 'BLQ', 'GLQ', 'ALQ','NA']-Rating of basement finished area (if multiple types)|
|**BsmtFinSF2**|int64|Train|Type 2 finished square feet|
|**BsmtUnfSF**|int64|Train| Unfinished square feet of basement area|
|**TotalBsmtSF**|int64|Train| Total square feet of basement area|
|**Heating**|object|Train|['GasA', 'GasW', 'Grav', 'Wall', 'OthW', 'Floor']- Type of heating|
|**HeatingQC**|object|Train|['TA', 'Gd', 'Ex', 'Fa', 'Po']- Heating quality and condition|
|**CentralAir**|object|Train|['Y', 'N']-Central air conditioning|
|**Electrical**|object|Train|['SBrkr', 'FuseF', 'FuseA', 'FuseP', 'Mix']-Electrical system|
|**1stFlrSF**|int64|Train|First Floor square feet|
|**2ndFlrSF**|int64|Train| Second floor square feet|
|**LowQualFinSF**|int64|Train|Low quality finished square feet (all floors)|
|**GrLivArea**|int64|Train|Above grade (ground) living area square feet|
|**BsmtFullBath**|int64|Train|Basement full bathrooms|
|**BsmtHalfBath**|int64|Train|Basement half bathrooms|
|**FullBath**|int64|Train| Full bathrooms above grade|
|**HalfBath**|int64|Train|Half baths above grade|
|**KitchenQual**|object|Train|['TA', 'Gd', 'Ex', 'Fa']- Kitchen quality|
|**TotRmsAbvGrd**|int64|Train|Total rooms above grade (does not include bathrooms)|
|**Functional**|object|Train|['Typ', 'Min2', 'Min1', 'Mod', 'Maj1', 'Sev', 'Maj2']-Home functionality (Assume typical unless deductions are warranted)|
|**Fireplaces**|int64|Train|Number of fireplaces|
|**FireplaceQu**|object|Train|['NA', 'TA', 'Gd', 'Po', 'Fa', 'Ex']- Fireplace quality|
|**GarageType**|object|Train|['Attchd', 'Detchd', 'BuiltIn', 'NA', 'Basment', '2Types', 'CarPort']- Garage location|
|**GarageYrBlt**|int64|Train|Year garage was built|
|**GarageFinish**|object|Train|['Unf', 'Fin', 'RFn', 'NA']-Interior finish of the garage|
|**GarageCars**|int64|Train|Size of garage in car capacity|
|**GarageArea**|int64|Train|Size of garage in square feet|
|**GarageQual**|object|Train|['TA', 'NA', 'Fa', 'Gd', 'Po']-Garage quality|
|**GarageCond**|object|Train|['TA', 'NA', 'Fa', 'Gd', 'Po', 'Ex']-Garage condition|
|**PavedDriv**|object|Train|'Y', 'N', 'P']-Paved driveway|
|**WoodDeckSF**|int64|Train|Wood deck area in square feet|
|**OpenPorchSF**|int64|Train|Open porch area in square feet|
|**EnclosedPorch**|int64|Train| Enclosed porch area in square feet|
|**3SsnPorch**|int64|Train| Three season porch area in square feet|
|**ScreenPorch**|int64|Train|Screen porch area in square feet|
|**PoolArea**|int64|Train|Pool area in square feet|
|**PoolQC**|int64|Train|['NA', 'Ex', 'Gd']-Pool quality|
|**Fence**|int64|Train|['MnPrv', 'NA', 'GdPrv', 'GdWo', 'MnWw']-Fence quality|
|**MiscVal**|int64|Train|$Value of miscellaneous feature|
|**MoSold**|int64|Train|Month Sold (MM)|
|**SaleType**|int64|Train|Year Sold (YYYY)|
|**SaleCondition**|Train|Test|['Normal', 'Partial', 'Abnorml', 'Family', 'Alloca', 'AdjLand']-Condition of sale|
# linear_predictors

### missing data

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**MSZoning**|object|Test|['RH', 'RL', 'RM', 'FV', 'C (all)', nan]
|**Utilities**|object|Test|['AllPub', nan]-Type of utilities available|
|**Exterior1st**|object|Test|['VinylSd', 'Wd Sdng', 'HdBoard', 'Plywood', 'MetalSd','CemntBd','WdShing', 'BrkFace', 'AsbShng', 'BrkComm', 'Stucco', 'AsphShn',nan,'CBlock']-Exterior covering on house|
|**Exterior2nd**|object|train|['VinylSd', 'Wd Sdng', 'HdBoard', 'Plywood', 'MetalSd', 'Brk Cmn','CmentBd', 'Test', 'Wd Shng', 'AsbShng', 'Stucco', 'CBlock','BrkFace', 'AsphShn', nan, 'Stone']- Exterior covering on house (if more than one material)|
|**MasVnrType**|object|Test|['None', 'BrkFace', 'Stone', 'BrkCmn', nan]-Masonry veneer type|
|**BsmtQual**|object|Test|['TA', 'Gd', 'Ex', 'Fa', nan]-Evaluates the height of the basement|
|**KitchenQual**|object|Test|['TA', 'Gd', 'Ex', 'Fa', nan]- Kitchen quality|
|**Functional**|object|Test|['Typ', 'Min2', 'Min1', 'Mod', 'Maj1', 'Sev', 'Maj2', nan]-Home functionality (Assume typical unless deductions are warranted)|
|**MasVnrType**|object|Train|['BrkFace', 'None', 'Stone', 'BrkCmn', nan]-Masonry veneer type|
|**Electrical**|object|Train|['SBrkr', 'FuseF', 'FuseA', 'FuseP', 'Mix', nan]-Electrical system|






#####
### DATAFRAME
|**Feature**|**Type**|**Dataset**|**Description**|
|---|---|---|---|
|**MSSubClass**|object|Test |[20 ,60 ,120 ,160 ,80 ,30 ,50 ,90 ,85 ,190 ,45 , 70 ,75 ,180 ,40 ,150 ]-Identifies the type of dwelling involved in the sale|
|**MSZoning**|object|Test|['RH' ,'RL' ,'RM' ,'FV' , 'C (all)']-Identifies the general zoning classification of the sale.|
|**LotFrontage**|int64|Test|Linear feet of street connected to property|
|**LotArea**|int64|Test|Lot size in square feet|
|**Street**|object|Test|['Pave', 'Grvl']-Type of road access to property|
|**Alley**|object|Test|['NA','Pave', 'Grvl']-Type of alley access to property|
|**LotShape**|object|Test|['Reg', 'IR1', 'IR2', 'IR3']-General shape of property|
|**LandContour**|object|Test|['Lvl', 'HLS', 'Bnk', 'Low']-Flatness of the property|
|**Utilities**|object|Test|['AllPub']-Type of utilities available|
|**LotConfig**|object|Test|['Inside', 'Corner', 'FR2', 'CulDSac', 'FR3']-Lot configuration|
|**LandSlope**|object|Test|['Gtl', 'Mod', 'Sev']-Slope of property|
|**Neighborhood**|object|Test|['NAmes', 'Gilbert', 'StoneBr', 'BrDale', 'NPkVill','NridgHt','Blmngtn', 'NoRidge', 'Somerst', 'SawyerW', 'Sawyer', 'NWAmes','OldTown','BrkSide', 'ClearCr', 'SWISU', 'Edwards', 'CollgCr','Crawfor', 'Blueste','IDOTRR', 'Mitchel', 'Timber', 'MeadowV','Veenker']-Physical locations within Ames city limits|
|**Condition1**|object|Test|'Feedr', 'Norm', 'PosN', 'RRNe', 'Artery', 'RRNn', 'PosA', 'RRAn','RRAe']-Proximity to various conditions|
|**Condition2**|object|Test|['Norm', 'Feedr', 'PosA', 'PosN', 'Artery']-Proximity to various conditions (if more than one is present)|
|**BldgType**|object|Test|['1Fam', 'TwnhsE', 'Twnhs', 'Duplex', '2fmCon']-Type of dwelling|
|**HouseStyle**|object|Test|['1Story', '2Story', 'SLvl', '1.5Fin', 'SFoyer', '2.5Unf', '1.5Unf']-Style of dwelling|
|**OverallQual**|object|Test|[ 5,  6,  8,  7,  4,  9,  2,  3, 10,  1]-Rates the overall material and finish of the house|
|**OverallCond**|object|Test|[6, 5, 7, 8, 2, 9, 3, 4, 1]-Rates the overall condition of the house|
|**YearBuilt**|int64|Test|Original construction date|
|**YearRemodAdd**|int64|Test|Remodel date (same as construction date if no remodeling or additions)|
|**RoofStyle**|object|Test|['Gable', 'Hip', 'Gambrel', 'Flat', 'Mansard', 'Shed']- Type of roof|
|**RoofMatl**|object|Test|['CompShg', 'Tar&Grv', 'WdShake', 'WdShngl']-Roof material|
|**Exterior1st**|object|Test|['VinylSd', 'Wd Sdng', 'HdBoard', 'Plywood', 'MetalSd','CemntBd','WdShing', 'BrkFace', 'AsbShng', 'BrkComm', 'Stucco', 'AsphShn', 'CBlock']- Exterior covering on house|
|**Exterior2nd**|object|Test|['VinylSd', 'Wd Sdng', 'HdBoard', 'Plywood', 'MetalSd', 'Brk Cmn','CmentBd', 'ImStucc', 'Wd Shng', 'AsbShng', 'Stucco', 'CBlock','BrkFace', 'AsphShn', 'Stone']- Exterior covering on house (if more than one material)|
|**MasVnrType**|object|Test|['None', 'BrkFace', 'Stone', 'BrkCmn']-Masonry veneer type|
|**MasVnrArea**|flot|Test| Masonry veneer area in square feet|
|**ExterQual**|object|Test|['TA', 'Gd', 'Ex', 'Fa']-Evaluates the quality of the material on the exterior|
|**ExterCond**|object|Test|['TA', 'Gd', 'Fa', 'Po', 'Ex']-Evaluates the present condition of the material on the exterior|
|**Foundation**|object|Test|['CBlock', 'PConc', 'BrkTil', 'Stone', 'Slab', 'Wood']-Type of foundation|
|**BsmtQual**|object|Test|['TA', 'Gd', 'Ex', 'Fa']-Evaluates the height of the basement|
|**BsmtCond**|object|Test|['TA', 'Po', 'Fa', 'Gd', 'NA']-Evaluates the general condition of the basement|
|**BsmtExposure**|object|Test|['No', 'Gd', 'Mn', 'Av', 'NA']-Refers to walkout or garden level walls|
|**BsmtFinType1**|object|Test|['Rec', 'ALQ', 'GLQ', 'Unf', 'BLQ', 'LwQ', 'NA']- Rating of basement finished area|
|**BsmtFinSF1**|int64|Test|Type 1 finished square feet|
|**BsmtFinType2**|object|Test|['LwQ', 'Unf', 'Rec', 'BLQ', 'GLQ', 'ALQ','NA']-Rating of basement finished area (if multiple types)|
|**BsmtFinSF2**|int64|Test|Type 2 finished square feet|
|**BsmtUnfSF**|int64|Test| Unfinished square feet of basement area|
|**TotalBsmtSF**|int64|Test| Total square feet of basement area|
|**Heating**|object|Test|['GasA', 'GasW', 'Grav', 'Wall']- Type of heating|
|**HeatingQC**|object|Test|['TA', 'Gd', 'Ex', 'Fa', 'Po']- Heating quality and condition|
|**CentralAir**|object|Test|['Y', 'N']-Central air conditioning|
|**Electrical**|object|Test|['SBrkr', 'FuseA', 'FuseF', 'FuseP']-Electrical system|
|**1stFlrSF**|int64|Test|First Floor square feet|
|**2ndFlrSF**|int64|Test| Second floor square feet|
|**LowQualFinSF**|int64|Test|Low quality finished square feet (all floors)|
|**GrLivArea**|int64|Test|Above grade (ground) living area square feet|
|**BsmtFullBath**|int64|Test|Basement full bathrooms|
|**BsmtHalfBath**|int64|Test|Basement half bathrooms|
|**FullBath**|int64|Test| Full bathrooms above grade|
|**HalfBath**|int64|Test|Half baths above grade|
|**KitchenQual**|object|Test|['TA', 'Gd', 'Ex', 'Fa']- Kitchen quality|
|**TotRmsAbvGrd**|int64|Test|Total rooms above grade (does not include bathrooms)|
|**Functional**|object|Test|['Typ', 'Min2', 'Min1', 'Mod', 'Maj1', 'Sev', 'Maj2']-Home functionality (Assume typical unless deductions are warranted)|
|**Fireplaces**|int64|Test|Number of fireplaces|
|**FireplaceQu**|object|Test|['NA', 'TA', 'Gd', 'Po', 'Fa', 'Ex']- Fireplace quality|
|**GarageType**|object|Test|['Attchd', 'Detchd', 'BuiltIn', 'NA', 'Basment', '2Types', 'CarPort']- Garage location|
|**GarageYrBlt**|int64|Test|Year garage was built|
|**GarageFinish**|object|Test|['Unf', 'Fin', 'RFn', 'NA']-Interior finish of the garage|
|**GarageCars**|int64|Test|Size of garage in car capacity|
|**GarageArea**|int64|Test|Size of garage in square feet|
|**GarageQual**|object|Test|['TA', 'NA', 'Fa', 'Gd', 'Po']-Garage quality|
|**GarageCond**|object|Test|['TA', 'NA', 'Fa', 'Gd', 'Po', 'Ex']-Garage condition|
|**PavedDrive**|object|Test|'Y', 'N', 'P']-Paved driveway|
|**WoodDeckSF**|int64|Test|Wood deck area in square feet|
|**OpenPorchSF**|int64|Test|Open porch area in square feet|
|**EnclosedPorch**|int64|Test| Enclosed porch area in square feet|
|**3SsnPorch**|int64|Test| Three season porch area in square feet|
|**ScreenPorch**|int64|Test|Screen porch area in square feet|
|**PoolArea**|int64|Test|Pool area in square feet|
|**PoolQC**|int64|Test|['NA', 'Ex', 'Gd']-Pool quality|
|**Fence**|int64|Test|['MnPrv', 'NA', 'GdPrv', 'GdWo', 'MnWw']-Fence quality|
|**MiscVal**|int64|Test|$Value of miscellaneous feature|
|**MoSold**|int64|Test|Month Sold (MM)|
|**SaleType**|int64|Test|Year Sold (YYYY)|
|**SaleCondition**|object|Test|['Normal', 'Partial', 'Abnorml', 'Family', 'Alloca', 'AdjLand']-Condition of sale|
|**MSSubClass**|object|Train|[ 60,  20,  70,  50, 190,  45,  90, 120,  30,  85,  80, 160,75,180,  40]-Identifies the type of dwelling involved in the sale|
|**MSZoning**|object|Train|['RL', 'RM', 'C (all)', 'FV', 'RH']-Identifies the general zoning classification of the sale.|
|**LotFrontage**|int64|Train|Linear feet of street connected to property|
|**LotArea**|int64|Train|Lot size in square feet|
|**Street**|object|Train|['Pave', 'Grvl']-Type of road access to property|
|**Alley**|object|Train|['NA','Pave', 'Grvl']-Type of alley access to property|
|**LotShape**|object|Train|['Reg', 'IR1', 'IR2', 'IR3']-General shape of property|
|**LandContour**|object|Train|['Lvl', 'HLS', 'Bnk', 'Low']-Flatness of the property|
|**Utilities**|object|Train|['AllPub', 'NoSeWa']-Type of utilities available|
|**LotConfig**|object|Train|['Inside', 'Corner', 'FR2', 'CulDSac', 'FR3']-Lot configuration|
|**LandSlope**|object|Train|['Gtl', 'Mod', 'Sev']-Slope of property|
|**Neighborhood**|object|Train|['CollgCr', 'Veenker', 'Crawfor', 'NoRidge', 'Mitchel','Somerst','NWAmes', 'OldTown', 'BrkSide', 'Sawyer', 'NridgHt', 'NAmes','SawyerW', 'IDOTRR', 'MeadowV', 'Edwards', 'Timber', 'Gilbert','StoneBr', 'ClearCr', 'NPkVill', 'Blmngtn', 'BrDale', 'SWISU','Blueste']-Physical locations within Ames city limits|
|**Condition1**|object|Train|['Norm', 'Feedr', 'PosN', 'Artery', 'RRAe', 'RRNn','RRAn','PosA','RRNe']-Proximity to various conditions|
|**Condition2**|object|Train|['Norm', 'Artery', 'RRNn', 'Feedr', 'PosN', 'PosA', 'RRAn','RRAe']-Proximity to various conditions (if more than one is present)|
|**BldgType**|object|Train|['1Fam', '2fmCon', 'Duplex', 'TwnhsE', 'Twnhs']-Type of dwelling|
|**HouseStyle**|object|Train|['2Story', '1Story', '1.5Fin', '1.5Unf', 'SFoyer','SLvl','2.5Unf','2.5Fin']-Style of dwelling|
|**OverallQual**|object|Train|[ 5,  6,  8,  7,  4,  9,  2,  3, 10,  1]-Rates the overall material and finish of the house|
|**OverallCond**|object|Train|[6, 5, 7, 8, 2, 9, 3, 4, 1]-Rates the overall condition of the house|
|**YearBuilt**|int64|Train**|Original construction date|
|**YearRemodAdd**|int64|Train|Remodel date (same as construction date if no remodeling or additions)|
|**RoofStyle**|object|Train|['Gable', 'Hip', 'Gambrel', 'Flat', 'Mansard', 'Shed']- Type of roof|
|**RoofMatl**|object|Train|['CompShg', 'WdShngl', 'Metal', 'WdShake', 'Membran','Tar&Grv','Roll', 'ClyTile']-Roof material|
|**Exterior1st**|object|Train|['VinylSd', 'MetalSd', 'Wd Sdng', 'HdBoard', 'BrkFace','WdShing','CemntBd', 'Plywood', 'AsbShng', 'Stucco', 'BrkComm', 'AsphShn','Stone', 'ImStucc', 'CBlock']- Exterior covering on house|
|**Exterior2nd**|object|Train|['VinylSd', 'Wd Sdng', 'HdBoard', 'Plywood', 'MetalSd', 'Brk Cmn','CmentBd', 'ImStucc', 'Wd Shng', 'AsbShng', 'Stucco', 'CBlock','BrkFace', 'AsphShn', 'Stone']- Exterior covering on house (if more than one material)|
|**MasVnrType**|object|Train|['BrkFace', 'None', 'Stone', 'BrkCmn']-Masonry veneer type|
|**MasVnrArea**|flot|Train| Masonry veneer area in square feet|
|**ExterQual**|object|Train|['TA', 'Gd', 'Ex', 'Fa']-Evaluates the quality of the material on the exterior|
|**ExterCond**|object|Train|['TA', 'Gd', 'Fa', 'Po', 'Ex']-Evaluates the present condition of the material on the exterior|
|**Foundation**|object|Train|['CBlock', 'PConc', 'BrkTil', 'Stone', 'Slab', 'Wood']-Type of foundation|
|**BsmtQual**|object|Train|['Gd', 'TA', 'Ex', 'NA', 'Fa']-Evaluates the height of the basement|
|**BsmtCond**|object|Train|['TA', 'Po', 'Fa', 'Gd', 'NA']-Evaluates the general condition of the basement|
|**BsmtExposure**|object|Train|['No', 'Gd', 'Mn', 'Av', 'NA']-Refers to walkout or garden level walls|
|**BsmtFinType1**|object|Train|['Rec', 'ALQ', 'GLQ', 'Unf', 'BLQ', 'LwQ', 'NA']- Rating of basement finished area|
|**BsmtFinSF1**|int64|Train|Type 1 finished square feet|
|**BsmtFinType2**|object|Train|['LwQ', 'Unf', 'Rec', 'BLQ', 'GLQ', 'ALQ','NA']-Rating of basement finished area (if multiple types)|
|**BsmtFinSF2**|int64|Train|Type 2 finished square feet|
|**BsmtUnfSF**|int64|Train| Unfinished square feet of basement area|
|**TotalBsmtSF**|int64|Train| Total square feet of basement area|
|**Heating**|object|Train|['GasA', 'GasW', 'Grav', 'Wall', 'OthW', 'Floor']- Type of heating|
|**HeatingQC**|object|Train|['TA', 'Gd', 'Ex', 'Fa', 'Po']- Heating quality and condition|
|**CentralAir**|object|Train|['Y', 'N']-Central air conditioning|
|**Electrical**|object|Train|['SBrkr', 'FuseF', 'FuseA', 'FuseP', 'Mix']-Electrical system|
|**1stFlrSF**|int64|Train|First Floor square feet|
|**2ndFlrSF**|int64|Train| Second floor square feet|
|**LowQualFinSF**|int64|Train|Low quality finished square feet (all floors)|
|**GrLivArea**|int64|Train|Above grade (ground) living area square feet|
|**BsmtFullBath**|int64|Train|Basement full bathrooms|
|**BsmtHalfBath**|int64|Train|Basement half bathrooms|
|**FullBath**|int64|Train| Full bathrooms above grade|
|**HalfBath**|int64|Train|Half baths above grade|
|**KitchenQual**|object|Train|['TA', 'Gd', 'Ex', 'Fa']- Kitchen quality|
|**TotRmsAbvGrd**|int64|Train|Total rooms above grade (does not include bathrooms)|
|**Functional**|object|Train|['Typ', 'Min2', 'Min1', 'Mod', 'Maj1', 'Sev', 'Maj2']-Home functionality (Assume typical unless deductions are warranted)|
|**Fireplaces**|int64|Train|Number of fireplaces|
|**FireplaceQu**|object|Train|['NA', 'TA', 'Gd', 'Po', 'Fa', 'Ex']- Fireplace quality|
|**GarageType**|object|Train|['Attchd', 'Detchd', 'BuiltIn', 'NA', 'Basment', '2Types', 'CarPort']- Garage location|
|**GarageYrBlt**|int64|Train|Year garage was built|
|**GarageFinish**|object|Train|['Unf', 'Fin', 'RFn', 'NA']-Interior finish of the garage|
|**GarageCars**|int64|Train|Size of garage in car capacity|
|**GarageArea**|int64|Train|Size of garage in square feet|
|**GarageQual**|object|Train|['TA', 'NA', 'Fa', 'Gd', 'Po']-Garage quality|
|**GarageCond**|object|Train|['TA', 'NA', 'Fa', 'Gd', 'Po', 'Ex']-Garage condition|
|**PavedDriv**|object|Train|'Y', 'N', 'P']-Paved driveway|
|**WoodDeckSF**|int64|Train|Wood deck area in square feet|
|**OpenPorchSF**|int64|Train|Open porch area in square feet|
|**EnclosedPorch**|int64|Train| Enclosed porch area in square feet|
|**3SsnPorch**|int64|Train| Three season porch area in square feet|
|**ScreenPorch**|int64|Train|Screen porch area in square feet|
|**PoolArea**|int64|Train|Pool area in square feet|
|**PoolQC**|int64|Train|['NA', 'Ex', 'Gd']-Pool quality|
|**Fence**|int64|Train|['MnPrv', 'NA', 'GdPrv', 'GdWo', 'MnWw']-Fence quality|
|**MiscVal**|int64|Train|$Value of miscellaneous feature|
|**MoSold**|int64|Train|Month Sold (MM)|
|**SaleType**|int64|Train|Year Sold (YYYY)|
|**SaleCondition**|Train|Test|['Normal', 'Partial', 'Abnorml', 'Family', 'Alloca', 'AdjLand']-Condition of sale|
