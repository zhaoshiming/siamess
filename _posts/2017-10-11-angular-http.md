---
layout: default
title: angular 数据请求
---

<h2>{{ page.title }}</h2>
<p class="important">??????????????????????????</p>
<div>
	var xhr = new XMLHttpRequest();
	xhr.open("get", "response.php");
	xhr.send();
	xhr.onreadystatechange = function () {

	}
</div>
















<p>{{ page.date | date_to_string }}</p>
