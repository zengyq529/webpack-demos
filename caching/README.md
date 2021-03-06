
# webpack 缓存


![webxiaoma](https://webxiaoma.github.io/other/manong.jpg)


```
npm install 

npm start
```


### 为什么要进行缓存

正如官网所说：

> 我们使用 webpack 来打包我们的模块化后的应用程序，webpack 会生成一个可部署的 /dist 目录，然后把打包后的内容放置在此目录中。只要 /dist 目录中的内容部署到服务器上，客户端（通常是浏览器）就能够访问网站此服务器的网站及其资产。而最后一步获取资源是比较耗费时间的，这就是为什么浏览器使用一种名为缓存的技术。可以通过命中缓存，以降低网络流量，使网站加载速度更快，然而，如果我们在部署新版本时不更改资源的文件名，浏览器可能会认为它没有被更新，就会使用它的缓存版本。由于缓存的存在，当你需要获取新的代码时，就会显得很棘手。


>通俗的讲，例如我们在项目中引入了jq或者是react这样的库和框架，它的代码我们基本上是不会去改动的，我们并不希望我们在改动我们自己的文件进行编译后，浏览器还要重新加载jq或react,我们只希望浏览器加载我们自己的文件。这样我们需要将像jq或react等库或框架拿出来整合到一个单独的文件中将他们缓存起来。而不必每次都重新请求获取资源。


### 相关资料

- [官网缓存介绍与实现](http://www.css88.com/doc/webpack/guides/caching/)

- [推荐博客](http://www.jianshu.com/p/345c0b05d761)

