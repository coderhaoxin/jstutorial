---
layout: homepage
title: JavaScript 标准教程（alpha）
date: 2012-11-18
modifiedOn: 2013-10-03
---

<h2 id="introduction">导论</h2>

- [版权声明](introduction/license.html)
- [为什么学习JavaScript？](introduction/why.html)
- [Javascript的历史](introduction/history.html)
- [使用说明](introduction/instruction.html)
- [参考书目](introduction/bibliography.html)

<h2 id="grammar">基本语法</h2>

- [概述](grammar/basic.html)
- [运算符](grammar/operator.html)
- [数值](grammar/number.html)
- [对象](grammar/object.html)
- [数组](grammar/array.html)
- [函数](grammar/function.html)
- [数据类型转换](grammar/conversion.html)
- [错误处理机制](grammar/error.html)
- [编程风格](grammar/style.html)
- [严格模式](grammar/strict.html)

<h2 id="stdlib">标准库</h2>

- [Object对象](stdlib/object.html)
- [Array 对象](stdlib/array.html)
- [原始类型的包装对象](stdlib/wrapper.html)
- [Boolean对象](stdlib/boolean.html)
- [Number对象](stdlib/number.html)
- [String对象](stdlib/string.html)
- [Math对象](stdlib/math.html)
- [Date对象](stdlib/date.html)
- [Regex对象](stdlib/regex.html)
- [JSON对象](stdlib/json.html)
- [类型化数组](stdlib/arraybuffer.html)

<h2 id="oop">面向对象编程</h2>

- [概述](oop/basic.html)
- [封装](oop/encapsulation.html)
- [继承](oop/inheritance.html)
- [Promises](oop/promises.html)
- [ECMAscript 6 介绍](oop/ecmascript6.html)

<h2 id="dom">DOM</h2>

- [dataset](dom/dataset.html)
- [classList](dom/classlist.html)
- [样式表操作](dom/stylesheet.html)
- [拖放操作](dom/dragndrop.html)
- [Mutation Observer](dom/mutationobserver.html)

<h2 id="bom">浏览器对象</h2>

- [浏览器的JavaScript引擎](bom/engine.html)
- [Navigator对象](bom/navigator.html)
- [History对象](bom/history.html)
- [CSS](bom/css.html)
- [Ajax](bom/ajax.html)
- [同域限制与window.postMessage方法](bom/windowpostmessage.html)
- [Web Storage](bom/webstorage.html)
- [WebSocket](bom/websocket.html)
- [Geolocation](bom/geolocation.html)
- [MatchMedia](bom/matchmedia.html)
- [WebRTC](bom/webrtc.html)
- [Navigation Timing](bom/navigationtiming.html)

<h2 id="htmlapi">HTML网页的API</h2>

- [Canvas](htmlapi/canvas.html)
- [SVG图像](htmlapi/svg.html)
- [文件与二进制数据的操作](htmlapi/file.html)
- [Web Worker](htmlapi/webworker.html)
- [服务器端发送事件](htmlapi/eventsource.html)
- [Page Visiblity](htmlapi/pagevisibility.html)
- [FullScreen](htmlapi/fullscreen.html)
- [Web Speech](htmlapi/webspeech.html)
- [requestAnimationFrame](htmlapi/requestanimationframe.html)

<h2 id="jquery">jQuery</h2>

- [选择器](jquery/selector.html)
- [Utility方法](jquery/utility.html)
- [deferred对象](jquery/deferred.html)
- [如何做到jQuery-free？](jquery/jquery-free.html)

<h2 id="library">函数库</h2>

- [Underscore.js](library/underscore.html)
- [Modernizr](library/modernizr.html)
- [Datejs](library/datejs.html)

<h2 id="tool">开发工具</h2>

- [console对象](tool/console.html)
- [Chrome开发工具](tool/chrome.html)
- [性能测试（Benchmark）](tool/benchmark.html)
- [PhantomJS](tool/phantomjs.html)
- [Grunt任务管理工具](tool/grunt.html)
- [RequireJS和AMD规范](tool/requirejs.html)
- [移动端开发](tool/mobile.html)
- [Google Closure](tool/closure.html)
- [Source map](tool/sourcemap.html)

<h2 id="special">专题</h2>

- [设计模式](special/designpattern.html)
- [异步编程](special/asynchronous.html)
- [排序算法](special/sorting.html)
- [有限状态机](special/fsm.html)

<h2 id="nodejs">Node.js</h2>

- [概述](nodejs/basic.html)
- [CommonJS规范](nodejs/commonjs.html)
- [Express框架](nodejs/express.html)

{% comment %}

{% if site.posts.size != 0 %}

## 最新文章

{% for post in site.posts %}
* {{ post.date | date_to_string }} [{{ post.title }}]({{ post.url }})
{% endfor %}

{% endif %}

{% if site.pages.size != 0 %}

## 最新页面

{% for page in site.pages limit:5 %}
{% if page.url !='/index.html' %}
* [{{ page.title }}]( {{ page.url }})（{{ page.date }}）
{% endif %}
{% endfor %}

{% endif %}

{% endcomment %}
