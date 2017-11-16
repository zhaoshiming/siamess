---
layout: default
title: css伪类
---

<h2>{{ page.title }}</h2>
<p class="siamess-left">这里是一些对伪类的整理</p>
<p>css引入伪类和伪元素概念是为了格式化文档树以外的信息.也就是说伪类和伪元素是用来修饰不在文档树中的部分。</p>
<br>
<p>伪类用于当已有元素处于某个状态的时候，为其添加对应的样式。</p>
<p>伪元素用于创建一些不在文档树中的元素，并且添加对应的样式。</p>
<p class="siamess-left">伪类和伪元素的区别</p>
<p>伪类的操作对象是文档树中已有的元素，而伪元素则创建了一个文档数外的元素。因此，伪类与伪元素的区别在于：有没有创建一个文档树之外的元素。</p>
<p class="siamess-left">具体用法</p>
<img src="/img/fake.png" class="image" /><br>
<img src="/img/fake2.png" class="image" /><br>
<p class="siamess-left">我的小demo</p>
<p>这里主要讲下伪元素的实现方法，比如给标题添加一个左引导，或者是给元素右边加一个小三角形。实现的思路就是元素的position: relative; 元素的::before或者是::after伪元素的position: absolute;进行绝对定位，主要会去设置content: ''; width: '';border: ;这几个属性来实现你需要的效果。 </p>
<p>
转载自AlloyTeam：http://www.alloyteam.com/2016/05/summary-of-pseudo-classes-and-pseudo-elements/
</p>
<p>{{ page.date | date_to_string }}</p>