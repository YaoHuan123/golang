##### go的协程的切换机制
- go的协程可以通过 runtime.GoSched()切换！
- 一般是有固定的切换点！
- 使用-race检测访问冲突


##### 切换点
- IO,select
- channel
- 等待锁
- 函数调用
- runtime.GoSched()

##### channel
```
var a channel int // a is nil这样声明的channel是一个nil的不能用
a:=make(channel int,1)
```

##### 只写channel
```
chan<- int只写channel
chan-> int只读channel

```
