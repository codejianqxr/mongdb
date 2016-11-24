# find 命令
  **查询语句,根据指定的条件查询相关的内容,结果是一个集合**       
1. find()   `查找内容`  
2. find({name:"zhangsan"})  `指定条件去查询`  
3. 比较查询  "<" "<=" ">" ">=" "=" "!=" => $gt", "$gte", "$lt", "$lte", "$ne" "没有关键字"  
  3.1 find({age:{"$lt":3}})   
4. 逻辑查询  "and" "or" "in"  "notin"   =>  "无关键字“, "$or", "$in"，"$nin"    
  4.1 find({"$or":[age:16,age:17}]});   
  4.2 find({age:{"$in":[16,17]}});    
  4.3 find({age:{"$nin":[15,16,17]}});  
5. 正则查询
  5.1 find({age:/5$/})  
6. 复杂条件查询
  6.1 find({"$where":function(){}})  
7. 查询指定字段
  7.1 find({name:/^z/},{age:1})  `传入第二个参数,显示的字段值为1,排除的字段值为0`   

# findOne()
  **查询一条信息** 

# 聚合查询
**常见的聚合操作有：count()，distinct，group，mapReduce()**  
1. count  统计集合的数量  ``
  
   
  
