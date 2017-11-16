---
layout: default
title: js编写约定
---

<h2>{{ page.title }}</h2>
<p>my first page</p>
<p class="siamess-left">浮点数</p>
<p>js中全部的数字都是双精度浮点数，由于存在精度陷阱，一般都是尽量进行整数的计算。比如最基础的货币，可以换算到最小单位进行计算以避免精度陷阱。</p>
<p class="siamess-left">隐式的强制转换</p>
<p>好的键盘和屏幕对你的肩膀来说特别的重要！</p>
<p>然后解决类型转化的方法是上ts，强制参数的类型，就不是有这些问题了，开不开心？</p>
<p class="siamess-left">原始对象优于封装对象</p>
<p>其实就是因为原始类型不能使用方法，所以就封装了一下，但是封装之后的变量是一个对象，具有对象的全部特性。原始类型上进行操作也是可以的，比如string的toUpperCase,但是这个操作是在新建的string的对象的基础下进行操作的，不会影响之前的string原始。所以，如果你想在一个原始类型的数据下进行操作，那么记得把操作之后的数据保存到一个新的变量下。</p>
<ul>
	<li>使用 === 而不是 ==，说到底还是ts。</li>
	<li>编码规范，别忘了 ;</li>
</ul>
<p class="siamess-left">闭包</p>
<p>我给的定义是，函数执行结束之后，仍然保留函数作用域内的变量，不被释放。或者可以说是函数返回一个函数，返回的这个函数具有访问外层函数变量的权限。</p>
function a(){                    <br>
	var call = 'jeda';           <br>
	function b(){                <br>
		return call+tt;          <br>
	}                            <br>
	return b;                    <br>
}                                <br>
a();                             <br>
<p class="siamess-left">作用域</p>
<p>js没有遍历作用域，只有函数作用域。而且变量存在提升，声明的遍历都会被提到所在函数作用域的顶部（如果有函数作用域的话），函数也会被提升到顶部。</p>
<p>使用let，创建块级作用域，es6，你，值得拥有。</p>
<p class="siamess-left">函数在不同情况下的this指向</p>
<p>直接运行，那么this指向的是最外层作用域</p>
<p>函数表达式运行，那么是作为对象的方法进行调用，指向当前对象。</p>
<p>new Object()这样的调用，会分为好几步，比如var list = new Call();那么就相当于新建了一个对象，并且把这个对象给了list，新对象拥有this新建对象的。</p>
<p>还有一种是call和apply调用。自己去找。</p>
<p class="siamess-left">对象的原型</p>
<p>三个原型访问器：分别为C.prototype， 用于建立由new C()创建的对象原型。Object.getPrototypeOf(obj),用于获取obj对象的原型对象的标准方法，obj._proto_获取obj对象原型对象的非标准方法。</p>




















<p>{{ page.date | date_to_string }}</p>