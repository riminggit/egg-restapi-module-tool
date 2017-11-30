# Egg Restapi Module Tool

a example of eggjs, react, antd, dva, webpack, mysql, restful api and other stuff made it work...

you can generate rest api eazily by this tool.

update note:
2017-07-10  initial
2017-07-17  [egg-restapi-module-tool v0.9 Released](https://github.com/fomenyesu/egg-restapi-module-tool/releases/tag/v0.9) 
2017-12-01  update login module with oauth2.0

[中文 README](https://github.com/fomenyesu/egg-restapi-module-tool/blob/master/README.cn.md)

# Examples for [egg](https://github.com/eggjs/egg/)

use react, Antd and Dva to develop front end modules. use eggjs and mysql to be backend. 
you can use npm run dev to develop both side's service. or use it as a boilerplate.

this example include two modules:
1 modules manager : module table's CRUD operation,
2 request manager : an note for restful api witch is generated by module tool.

## Develop

#### Installation

install mysql
start mysql
import testdb.sql to mysql

```
npm install
```
#### Start up：

run npm to start server

```
npm run dev
```

Go to  http://localhost:8080 。

also you can :
npm run dev_static to start front react project
npm run server to start egg server
npm run dev to start both


## Distribute

```bash
$ npm run build
$ npm run pro
```

npm run build to build the front end react project.
npm run pro in server to start project on you server
visit 
http://serverIP:7001

## REST API Example

api/restql/users GET List

```javascript
{
"meta":{"total":3},
"data":[
{"_id":"58d8a899f5f2486f1f6d4236","uid":1,"name":"admin","pass":"123","status":1,"time":"1325472736"},
{"_id":"58db7828a14b14815447cf33","name":"sdf","pass":"123","status":1,"time":"1325472736","uid":3,"__v":0},
{"_id":"58db7d3bcee4d48df6f5bdfd","name":"sdddf","pass":"123","status":1,"time":"1325472736","uid":4,"__v":0}
]
}
```

api/restql/users/1 GET Single Data

```javascript
{
"meta":{"total":1},
"data":[
{"_id":"58d8a899f5f2486f1f6d4236","uid":1,"name":"admin","pass":"123","status":1,"time":"1325472736"}
]
}
```

api/restql/users/2 PUT Update data with uid

```javascript
{"name":"admin123","pass":"123","status":1,"time":"1325472736"}
```

api/restql/users POST insert data

```javascript
{"name":"admin123","pass":"123","status":1,"time":"1325472736"}
```

same with news and news_type for rest api data.

# screen shot

![login.png](http://api.dll0.com/public/img/login.png)
![page1.png](http://api.dll0.com/public/img/page1.png)
![page2.png](http://api.dll0.com/public/img/page2.png)
![page3.png](http://api.dll0.com/public/img/page3.png)

# Thank you

[egg](https://github.com/eggjs/egg/)

[ant-design](https://github.com/ant-design/ant-design/)

[antd-admin](https://github.com/zuiidea/antd-admin)
