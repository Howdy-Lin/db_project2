# db_project2

**1.查詢意外事故當中，造成事故的車輛車輛數目(Number_of_Vehicle)>3， 車速限制(Speed_limit)30時速英里以下的資料:**
**查詢句**db.getCollection("Accident").find({"Number_of_Vehicles":{$gt:3},"Speed_limit":{$lt:30}})  


**2.查詢意外事故當中，駕駛性別（Sex_of_Driver）＝＂女＂(1)，車道外撞擊物體數（Hit_Object_off_Carriageway）＞２**
**查詢句**db.getCollection("Accident").find({ "Sex_of_Driver" : { $eq : 2.0 }, "Hit_Object_off_Carriageway" : { $gt : 2 } })  


**3.查詢意外事故當中，傷亡乘客年齡（Age_of_Casualty）> 60，且傷亡種類為骨折（Casualty_Class） = １**
**查詢句**db.getCollection("Accident").find({"Age_of_Casualty":{$gt:60},"Casualty_Class":{$eq:1}})
