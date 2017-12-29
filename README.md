# vue_axios

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

##配置
```bash
# main.js
import http from './utils/http'
import api from './utils/api'

Vue.prototype.$http = http;
Vue.prototype.api = api;

#xxx.vue

GET
fetchLeague: async function () {
  let params = {

  };
  const res = await this.$http.get(this.api.leagues, params)
  console.log(res)
},

POST
fetchLeague: async function () {
  let params = {

  };
  const res = await this.$http.post(this.api.leagues, params)
  console.log(res)
},

```
