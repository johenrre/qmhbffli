### 什么是前后端分离？

- 这里前后端分离并不是传统的方式， 前端通过 `ajax`请求获取数据，后端写`api`.
- 而是指开发环境上的分离 ( 就是有自己的`repository` )



### 传统开发模式缺点

- 传统开发模式就是前端写客户端， 后端写 `api` 服务器
- 前端需要搭建后端的开发环境， 然后运行后端的项目
- 前后端对接的时候后端改动一个地方， 前端可能需要更新项目代码
- 对接多个后端时候， 当一个后端出现问题， 可能就会影响前端的流程
- `Access-Control-Allow-Origin`浏览器出现这个错误。（跨越请求问题, 下面有解决方式）



### Node使用Cors解决跨域请求问题

```js
// 在node服务端app.js里
const cors = require('cors')
const app = express()
app.user(cors())
```



