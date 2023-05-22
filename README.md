# Front-end-development-experience


升级 node 版本到 v18.3.0 后，执行 npm run dev 启动 vue-cli-service 本地开发服务报错
例如
```cpp
error:0308010C:digital envelope routines::unsupported
    at new Hash (node:internal/crypto/hash:67:19)
    at Object.createHash (node:crypto:135:10)
```
Windows执行
<code>set NODE_OPTIONS=--openssl-legacy-provider</code>
Linux / Mac执行
<code>export NODE_OPTIONS=--openssl-legacy-provider</code>


vue-soft-ui-dashboard-main的node版本号17


让竖形框铺满

```cpp
height: calc(100vh);
```

**vue3引入ant-design-ui方式**

```shell
npm install ant-design-vue@next
```


在main.js中直接用
```js
import { createApp } from 'vue';
import { Button } from 'ant-design-vue';

const app = createApp(App);
app.use(Button);
app.mount('#app');
```

