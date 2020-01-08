`window.location.href`

它是异步的，不会立即就阻塞所有的代码，在进行页面跳转前会至少等待一个页面离开事件

```
(function(){

    window.location.href= 'www.baidu.com';
    console.log(123);
}())
```

以上代码，在跳转到百度之前会执行下面的console输出123

如果需要立即跳转不执行后续方法，可以在location.href后面加上return false

