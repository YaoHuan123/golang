#### 基础类型
- string
```
func stringTest(){
	s := "hello"
	srr:=[]byte(s)
	srr[1] = 's'
	// 下面输出的还是hello
	fmt.Println(s)
}
```
- map
```
  //取值
	m := map[string]string{"1":"hello"}
  k,ok:=m["2"]
	fmt.Println(k,ok)
  // 可以作为key的类型
	// 除了slice   map   function 其它内建类型都可以作为key
  // struct类型不包含上诉字段，也可以作为 key
  delete(m,"1")
```
- 指针
```
// c++中默认是值传递，可以声明为引用
// c++中vector执行的是深copy
// java中除了内置类型，都是引用传递
// golang中只有值传递
// golang默认是浅copy
```
- 全局变量
```
//1.全局变量必须要有var修饰
var (
	a = 100
	b = 200
)
```

- golang是静态类型语言
```
var r io.Reader
r = os.Stdin
// 这里r是io.Reader类型，不是os.Stdin类型
```

- 深入理解interface
```
interface 中保存的是值，类型对
```

- 使用github上的包，使用go get命令下载下来，一般是放在GOPATH的src下面的


