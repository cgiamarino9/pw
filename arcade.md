# This is an ArcGIS Pro Arcade expression that groups land use values into labels
```
var landUse = $feature.PW_Zoning
var sfr = Includes(['1100','1111','1110', '1113'], landUse)
var mobile = Includes(['1130','1131','1132'], landUse)
var mixres = Includes(['1140','1100'], landUse)
var multires = Includes(['1120','1121','1122','1123','1124'], landUse)
var ruralres = Includes(['1150'], landUse)
var mixrescom = Includes(['1600','1610','1620'], landUse)
var specplan = Includes(['7777'], landUse)
var comser = Includes(['1200','1220','1221', '1222','1223','1230', '1231','1232', '1233'], landUse)
var genoff = Includes(['1210','1211','1212', '1213'], landUse)
var edu = Includes(['1260','1261','1262', '1263','1264','1265', '1266'], landUse)
var mixcomind = Includes(['1500'], landUse)
var mil = Includes(['1270','1271','1272','1273','1274','1275','1276'], landUse)
var fac = Includes(['1240','1241','1242', '1243','1244','1245', '1246', '1247', '1250', '1251','1252', '1253'], landUse)
var ind = Includes(['1300','1310','1311', '1312','1313','1314', '1320', '1321', '1322', '1323','1324', '1325', '1330', '1331','1332', '1340'], landUse)
var wat = Includes(['4000','4100','4200','4300','4400','4500'], landUse)
var osr = Includes(['1800','1810','1820', '1830','1840','1850', '1860', '1870', '1880', '1890'], landUse)
var ag = Includes(['2000','2100','2110', '2120','2200','2300', '2400', '2500', '2600', '2700'], landUse)
var vac = Includes(['3000','3100','3200', '3300', '3400','1900'], landUse)
var trans = Includes(['1400', '1410', '1411', '1412', '1413', '1414', '1415', '1416', '1417', '1418', '1419','1420', '1430', '1431', '1432', '1433', '1434','1435', '1436', '1437','1438', '1440', '1441', '1442', '1450', '1406'], landUse)
var undcons = Includes(['1700'], landUse)
var und = Includes(['8888'], landUse)
var unk = Includes(['9999'], landUse)
if (sfr == True) {
    return 'Single Family Residential'
}
else if (mobile == True) {
    return 'Mobile Homes and Trailer Parks'
}
else if (mixres == True) {
    return 'Mixed Residential'
}
else if (multires == True) {
    return 'Multi-Family Residential'
}
else if (ruralres == True) {
    return 'Rural Residential'
}
else if (mixrescom == True) {
    return 'Mixed Residential and Commercial'
}
else if (specplan == True) {
    return 'Specific Plan'
}
else if (comser == True) {
    return 'Commercial and Services'
}
else if (genoff == True) {
    return 'General Office'
}
else if (edu == True) {
    return 'Education'
}
else if (mixcomind == True) {
    return 'Mixed Commercial and Industrial'
}
else if (mil == True) {
    return 'Military Installations'
}
else if (fac == True) {
    return 'Facilities'
}
else if (ind == True) {
    return 'Industrial'
}
else if (wat == True) {
    return 'Water'
}
else if (osr == True) {
    return 'Open Space and Recreation'
}
else if (ag == True) {
    return 'Agriculture'
}
else if (vac == True) {
    return 'Vacant'
}
else if (trans == True) {
    return 'Transportation, Communication, and Utilities'
}
else if (undcons == True) {
    return 'Under Construction'
}
else if (und == True) {
    return 'Undevelopable'
}
else {
    return 'Unknown'
}



```
