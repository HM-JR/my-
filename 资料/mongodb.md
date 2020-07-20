```

**MongoDB特点**
```

```python
【1】非关系型数据库,数据以键值对方式存储，端口27017
【2】MongoDB基于磁盘存储
【3】MongoDB数据类型单一,值为JSON文档,而Redis基于内存,
   3.1> MySQL数据类型：数值类型、字符类型、日期时间类型、枚举类型
   3.2> Redis数据类型：字符串、列表、哈希、集合、有序集合
   3.3> MongoDB数据类型：值为JSON文档
【4】MongoDB: 库 -> 集合 -> 文档
     MySQL  : 库 -> 表  ->  表记录
```

- **MongoDB常用命令**

  ```python
  Linux进入: mongo
  >show dbs                  - 查看所有库
  >use 库名                   - 切换库
  >show collections          - 查看当前库中所有集合
  >db.集合名.find().pretty()  - 查看集合中文档
  >db.集合名.count()          - 统计文档条数
  >db.集合名.drop()           - 删除集合
  >db.dropDatabase()         - 删除当前库
  ```
  
  ```python
  import pymongo
  
  # 1.连接对象
  conn = pymongo.MongoClient(host = 'localhost',port = 27017)
  # 2.库对象
  db = conn['maoyandb']
  # 3.集合对象
  myset = db['maoyanset']
  # 4.插入数据库
  myset.insert_one({'name':'赵敏'})
  myset.insert_many([{'name':'小昭'},{'age':'30'}])
  ```
  
- 

  ```python
  
  ```

## 

- ****

  ```
  
  ```
  
- 


- 

  ```
  
  ```
  