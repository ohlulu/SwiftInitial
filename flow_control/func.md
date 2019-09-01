# 函數 func

函數：又叫做 function、方法

用途是執行一段程式碼，可以有參數，有回傳，也可以都沒有。

* 函數的宣告

完整的格式如下：
```swift
// 無參數，也無回傳
func {函數名稱}() {

}

// 有參數，也無回傳
func {函數名稱}({參數名稱1}: {參數型別1}, {參數名稱2}: {參數型別2}) {
    
}

// 無參數，有回傳
func {函數名稱}() -> {回傳型別} {
    return {回傳值}
}
```

實際用法：

```swift
// 無參數，也無回傳
func doSomething() {
    print("doSomething")
}

// 有參數，也無回傳
func printSum(x: Int, y: Int) {
    print(x + y)
}

// 無參數，有回傳
func getSum(x: Int, y: Int) -> Int {
    return x + y
}
```

# 練習
1. 宣告一個 func 