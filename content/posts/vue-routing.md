---
title: Vue Routing
date: 2021-01-12 11:15:00
draft: true
tags:
- Vue
---

I originally picked Vue as my frontend framework of choice because it felt a little lighter than React/Angular and the documentation seemed better/more thorough. Despite this, I still had a little bit of trouble when I first got started with routing in Vue, even though it's pretty straightforward (once you get the hang of it).

The [docs](https://vuejs.org/v2/guide/routing.html) on the Vue.js site described a smaller scale implementation of a vue instance, not a  And the docs on the Vue router page were a bit more illuminating, but still, the examples provided were still quite simple, not really getting at how you might use routing IRL. 

What I found that made the most sense for me was to first create a file 'router.js' to put all my routers, etc in one place. 

Before you can really get going though, you'll need to install the vue-router. So quit your server if it's running and go ahead to your terminal and enter in ``` npm install vue-router```

After that's done, you can go ahead and do the setup for your router, making sure to import Vue, vue-router and any components you want to use in your routing. Here, I have three components: SignUp, HomePage and Login that I will use to create three separate pages on my site, each with their own route. 
```
import Vue from 'vue'
import Router from 'vue-router'
import SignUp from './components/SignUp.vue'
import HomePage from './components/HomePage'
import Login from './components/Login.vue'

```

Once you've done that, you'll want to create the actual routes. I found it made the most sense to just create a separate variable, routes, and set the paths with their respective components there. 
```
const routes = [
    { path: '/signup', component: SignUp }, 
    {path: '/', component: HomePage}, 
    {path: '/login', component: Login}
  ]
  
  ```

  Okay, you've got your routes + components matched, now you have to tell Vue to use this router set up. And another thing you'll need to tell Vue is to use 'history' mode for the router. This will avoid 'Hash' mode, which will give you URLs like  'http://myexample.com/#/about'...not so pretty. Instead, URLs will look like 'http://myexample.com/about', a lot cleaner and nicer to look at!

  ```
  Vue.use(Router)
  
  export default new Router({
    routes,
    mode: 'history'
  })
  ```

  Hooray, your router is set up. Now go back to your ```main.js``` file and import it in. 

  ```
  import router from './router'
  ```

  The next step is to tell your Vue instance to use it. 
  ```
  new Vue({
  //add your router here
  router, 
  render: h => h(App)
  
}).$mount('#app')
```
Great! The router is ready to be used. But 



