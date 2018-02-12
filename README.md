# VUE中实现Swiper轮播图

> A Vue.js project

## Build Setup

``` bash
#安装Swiper插件
npm install vue-awesome-swiper

#main.js
require('swiper/dist/css/swiper.css')
import VueAwesomeSwiper from 'vue-awesome-swiper'
Vue.use(VueAwesomeSwiper)

#App.vue 这个非常重要，没有的话Swiper参数无效
import Swiper from 'swiper'

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
