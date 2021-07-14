# Project Description
In this Project, MongoDB used as Database for weekly demand collection system.

# Requirements
* MongoDB
* Json file / document file
* Jupyter Notebook

# MongoDB compass screenshots
<p align="left">
  <img width="600" height="360" src="https://github.com/myusufuc/Project_0/blob/main/1%20(1).png">
  <img width="600" height="360" src="https://github.com/myusufuc/Project_0/blob/main/1%20(2).png">
</p>

# MongoDB queries
1. insert_many():
   ```
   Weekly_Demand_Collection.insert_many(File_Data)
   ```
   * upload the initial json/document file data.

2. insert_one():
  ```
   Weekly_Demand_Collection.insert_one(Data_With_Id)
   ```
   * Insert single document into collection
   
3. find():
   ```
   Weekly_Demand_Collection.find({"id":1729422})
   ```
   * finding single id
   
4. limit():
   ```
   Weekly_Demand_Collection.find().limit(5)
   for i in we:
      print(i)
   ```
   * show collection with limit
4. count():
   ```
   Weekly_Demand_Collection.find().count()
   ```
   * count te total number of documents in collection

6. update_one():
   ```
   Weekly_Demand_Collection.update_one({"id":1729422},{"$set" : {"week":4}})
   ```
   * updating single value

7. update_many():
   ```
   Weekly_Demand_Collection.update_many({"id":1253588},{"$set" : {'week': 1,'center_id': 34,'meal_id': 1933}})
   ```
   * updating multiple values

8. delete_one():
   ```
   Weekly_Demand_Collection.delete_one({"id":1729422})
   ```
   * deleting single value

9. delete_many():
   ```
   Weekly_Demand_Collection.delete_many({"id":1253588,"id":1747636,"id":1535438,"id": 1463533})
   ```
   * deleting multiple values
