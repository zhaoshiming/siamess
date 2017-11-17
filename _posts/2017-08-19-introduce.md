---
layout: default
title: here is my introduce
---

# 基础算法

#### 给出一个数组，要求判断是否存在两个数的和等于指定数字
思路是遍历数组，用当前数组元素和当前元素后面的全部元素进行相加比对。如果等于指定数字，那么返回index的值。
``` javascript
var twoSum = function(nums, target) { 
    for(var i = 0;i< nums.length;i++){
      for(var j = i+1;j< nums.length;j++){
        var code = nums[i] + nums[j];
        if (code == target){
           return [i,j];
        }
      }
    }
  return arr;
};
```
#### 给出一个数，要求反转当前数字</p>
思路是当前数字转为数组，进行反转，再转为数字
``` javascript
var reverse = function(x) {
    if(x>0){
      return Number(x.toString().split('').reverse().join(''));
    }else {
      x = x*-1;
      return Number(x.toString().split('').reverse().join(''))*-1;
    }
    
};
```
#### 给出一个数，要求判断是否是回文，例如1221，或13531
思路是当前数字转为数组，分两种情况，一种是偶数位的数字，一种是奇数位的数字。
``` javascript
var isPalindrome = function(x) {
    if(x<0){
        x = x*-1;
    }
    var arr = x.toString().split('');
    var len = arr.length;
    if(len%2 == 0){
        var mid = len/2;
        for(var i = 0;i<mid;i++){
           if(arr[i]==arr[len-1-i]){
               continue;
           }else {
               return false;
           }
       }
    }else {
        var anotherMid = (arr.length+1)/2-1;
        for (var m = 0;m<anotherMid;m++){
            if (arr[i]==arr[len-1-i]){
                continue;
                }else{
                    return false;
                }
        }
    }
};
```

