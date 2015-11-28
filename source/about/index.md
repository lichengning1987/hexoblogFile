title: 前端效果库
date: 2015-09-28 15:52:37
tags:
---
这是我整理的一些工作中用到的一些JS效果。
<!--more-->


### 简单的拖拽
说明：原生JS实现的简单拖拽。

具体查看demo: [Drag](/about/drag.html)

### 倒计时
说明：基于jQuery封装的倒计时插件，传参可以传入开始时间和结束时间
使用方法：
``` bash
    //var nowDate = '2015/04/16 01:00:45'; //服务器当前时间
    //var endTime //结束时间格式如同开始时间
    $(obj).activeCountDown({
        lastTime:endTime, //结束时间
        now:new Date(nowdate) //开始时间
    },function(){
        //倒计时结束回调函数
    })
```

具体查看demo: [倒计时](/about/djs.html)

### 购物车动画
说明：基于jQuery封装的购物车动画插件
使用方法：
``` bash
$(obj).on('click',function(){
    $(this).shoping();
 })
```
具体查看demo: [购物车动画](/about/cartAnim.html)

### 图片切换
说明：基于jQuery封装的图片切换插件

具体查看demo: [图片切换](/about/switchImg.html)

### 酒店日历插件
说明：基于jQuery封装的住店日历插件，插件可以传入服务器时间和住宿的天数
``` bash
var date = [2015,11,15],day = 3;
$(".clbtn").datepicker({
    "dateYear":parseInt(date[0]), //服务器时间--当前年
    "dateMonth":parseInt(date[1]),//服务器时间--当前月
    "dateDay":parseInt(date[2]), //服务器时间--当前日
    "day":day //住几天
});
```
具体查看demo: [日历](/about/datapicker.html)