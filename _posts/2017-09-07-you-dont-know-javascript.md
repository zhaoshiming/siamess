---
layout: default
title: 你不知道的javascript上卷
---

<h2>{{ page.title }}</h2>
<p class="important">最近梦魇越来越严重了。</p>
<p>js在执行之前会由编译器进行编译，编译过程分为词法分析，语法分析和代码生成。然后由引擎进行执行。</p>
<p class="siamess-left">编译器部分：</p>
<p>在遇到一句var a = 12; 声明的时候，会在词法分析阶段把代码变为词法单元，就是切开。然后生成可以让引擎执行的代码。</p>
<p class="siamess-left">引擎部分：</p>
<p> 在遇到赋值语句的时候，或者是遇到一个变量的时候会询问a是否已在作用域里面，在就给这个变量进行赋值，不在就继续查找，找不到就抛出错误。也就是说，js会对声明语句进行两次处理，一次是声明，一次是赋值。先声明后赋值。</p>
<p>this 的四种绑定</p>
<ul>
	<li>默认绑定，就是this指向的是当前的全局作用域</li>
	<li>隐式绑定，就是this指向当前对象</li>
	<li>显示绑定，使用foo.call(obj) 和 foo.apply(obj) 把显式的把参数作为this的指向,那么foo中的this就指向了obj</li>
	<li></li>
</ul>















<p>{{ page.date | date_to_string }}</p>