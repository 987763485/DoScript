# DoScript

一个Rust编写的脚本语言

## 语法

### 包
```js
 import std
 import api from http
```

### 常量

```rust
const PI = 3.14
const PI :f32 = 3.14
```

### 变量
```rust
let title  = 'hello'
let title :string = 'hello'
```

### 条件语句
```rust
if (a = 10) {
	 //to do something
    return true
}else {
	 //to do something
    return false
}
```

### 循环语句
```rust
for (let i = 0; i < 10; i++) {
    //to do
}
```

### 数组
```js
let arr  = [1,2,3,4,5]
let arr :[]int = [1,2,3,4,5]
arr[0] = 10
arr.push()
arr.pop()
arr.contan() 
```

### 元组
```js
let t = (1,"hello",1010)
let t :(int,string,int) = (1,"hello",1010)
```

### 字典
```rust
let mut map :HashMap<string, int> = HashMap::new();
map.insert("Alice", 100);
map.insert("Bob", 90);
map.insert("Charlie", 95);
let alice_map = map.get("Alice");
```



### 函数

```rust
func main(){
	//to do
    setTextProperties({title:"hello"})
    <p></p>
}

func setTextProperties(p:Properties) -> Properties{
    //to do
    return p
}

//匿名函数
const variable = func() -> Properties {
    return 
}
//箭头函数
const variable = () -> Properties => {
    return 
}

func createParagraphs() {
	<段落 属性=p>
		<文字 属性=p></文本>
	</段落>
	<p properties=p>
		<text properties=p></text>
	</p>
}
```

### 结构体
```rust
struct  Properties{
    title: string,  
    setTitle: func()-> string {
        //to do something
        return self.title = "hello"
    },
    getTitle: ()-> string => {
    //to do something
        return self.title
    }
}

```

### 继承
```rust
struct Preson :Properties {
}

//语法糖
struct Preson  {    
    super :Properties
}

let person = new Person({
    title : "hello"
})

person.super.title = "hello"
```
### 枚举
```rust
enum Result<S, E>{
    Ok(S),
    Err(E)
}

enum Option<T> {
    Some(T),
    None,
}
```

### 函数重载
```rust
func getName(p: Peolpe) -> string {

}

func getName(p: Student) -> string {

}
```

### 模式匹配
```rust
func value_in_cents(coin: Coin) -> int {
    match coin {
        Coin::Penny => 1,
        Coin::Nickel => 5,
        Coin::Dime => 10,
        Coin::Quarter => 25,
    }
}
```
### 装饰器
```rust
@name(value=2)
func name() -> string {

}
```

### 异常处理
```rust
try {
    // to do
    throw new Exception()
} catch (e: SomeException) {
    // 处理程序
} finally {
    // 可选的 finally 块
}
```

