#### 定义

restful api是用于在前端与后台进行通信的一套规范，使用这个规范可以让前后端开发变得更加轻松

#### 协议

使用 http 或 https 协议

#### 数据传输格式

使用 json 的格式

#### HTTP请求的方法

- GET 从服务器上获取资源
- POST 在服务器上新创建一个资源
- PUT 在服务器上更新资源 (客户端提供所有改变后的数据)
- PATCH 在服务器上更新资源 (客户端只提供需要改变的属性)
- DELETE 在服务器上删除资源

#### 示例

- GET /users/ 获取所有用户
- POST /user/ 新建一个用户
- GET /user/id/ 根据id获取一个用户
- PUT /user/id/ 更新某个id的用户信息 (需要提供用户的所有信息)
- PATCH /user/id/ 更新某个id的用户信息 (只需要提供需要改变的信息)
- DELETE /user/id/ 删除一个用户 
  
#### 状态码

状态码 | 原生描述 | 描述
---|--- | --
200 | ok | 服务器成功响应客户端的请求
400 | invalid request | 用户发出的请求有错误，服务器没有进行新建或修改数据的操作
404 | not found | 用户发送的请求的url不存在
500 | Internal server error | 服务器内部错误，出现了bug

#### 高级用法

- 添加装饰器 api_plus里面
- parse的作用 api_plus里面
- 手动实现resource类

