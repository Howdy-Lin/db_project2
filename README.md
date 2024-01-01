# db_project2

**1.查詢意外事故當中，造成事故的車輛車輛數目(Number_of_Vehicle)>3， 車速限制(Speed_limit)30時速英里以下的資料:**
db.getCollection("Accident").find({"Number_of_Vehicles":{$gt:3},"Speed_limit":{$lt:30}})


**2.查詢意外事故當中，駕駛性別（Sex_of_Driver）＝＂女＂(1)，車道外撞擊物體數（Hit_Object_off_Carriageway）＞２**
db.getCollection("Accident").find({ "Sex_of_Driver" : { $eq : 2.0 }, "Hit_Object_off_Carriageway" : { $gt : 2 } })
