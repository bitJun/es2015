# es2015
## 数组的新增方法
1.map
例：
let arr = [1,2,3,4,5,6,7,8,9,10];
arr.map((item)=>{return item*item}) //输出结果是 [1, 4, 9, 16, 25, 36, 49, 64, 81, 100]
let app = [10,20,30,40,50,60,70,80,90,100];
app.map((item)=> {if(item<60){return '不及格'}else{return '及格'}})  //输出结果是 ["不及格", "不及格", "不及格", "不及格", "不及格", "及格", "及格", "及格", "及格", "及格"]


2.reduce
例：
let reduce = [10,20,30,40,50,60,70,80,90,100];
reduce.reduce((item,index)=>{return item + index})  //输出结果是 550

输出结果是多对一的关系

3.filter
例：
let filter = [11,22,33,44,5,4,3,2,66,77];
filter.filter((item)=>{return item%3 === 0})  //输出结果是 [33, 3, 66]

4.forEach
例：
let sum = 0;
let each = [11,22,33,44,5,4,3,2,66,77];
let total = (item)=>{sum += item;console.log(sum)};
each.forEach(total)
输出结果是：
11        VM638:3
33        VM638:3
66        VM638:3
110       VM638:3
115       VM638:3
119       VM638:3
122       VM638:3
124       VM638:3
190       VM638:3
267       VM638:3
