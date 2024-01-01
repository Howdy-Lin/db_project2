# db_project2

**1.查詢意外事故當中，造成事故的車輛車輛數目(Number_of_Vehicle)>3， 車速限制(Speed_limit)30時速英里以下的資料:**<br><br>
db.getCollection("Accident").find({"Number_of_Vehicles":{$gt:3},"Speed_limit":{$lt:30}})<br><br>
**查詢結果**  
![image](https://github.com/Howdy-Lin/db_project2/assets/74965449/2f98a43c-f19d-4c4d-9ede-3e6a8ec0d8a1)

**2.查詢意外事故當中，駕駛性別（Sex_of_Driver）＝＂女＂(1)，車道外撞擊物體數（Hit_Object_off_Carriageway）<２**<br><br>
db.getCollection("Accident").find({ "Sex_of_Driver" : { $eq : 2.0 }, "Hit_Object_off_Carriageway" : { $lt : 2 } })<br><br>
**查詢結果**  
![image](https://github.com/Howdy-Lin/db_project2/assets/74965449/62d5bc13-5e77-4a90-ba2f-2c72ea6a6db1)


**3.查詢意外事故當中，傷亡乘客年齡（Age_of_Casualty）> 60，且傷亡種類為骨折（Casualty_Class） = １**<br><br>
db.getCollection("Accident").find({"Age_of_Casualty":{$gt:60},"Casualty_Class":{$eq:1}})<br><br>
**查詢結果**<br>
![image](https://github.com/Howdy-Lin/db_project2/assets/74965449/9470e07b-8085-460e-ad0e-94ee6fd6ec4c)
