##### defer是退出某一个函数时执行的，不是退出某一个作用域执行，这点和我c++中自己写的哪个玩意不一样

##### 闭包中传递的是引用
```
import (
	"fmt"
)

func main() {
	a := []int{1, 2, 3}
	for _, i := range a {
		fmt.Println(i)
		defer func() {
			fmt.Println(i)
		}()
	}
	fmt.Println("ok")
}
```
