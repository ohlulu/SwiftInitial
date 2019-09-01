# Optional - 可選型別

* [宣告的部分](宣告的部分)
* [使用的部分](#tag_2)

在之前的課程有說明過，所謂的變數，其實就像是一個盒子；值，就是盒子的內容物。

那既然有盒子，有內容物，就還有一種可能：盒子沒有內容物。

<a href="#tag_1"> 

### 宣告的部分

Optional 完整的宣告是長這樣

 ```swift
 let maybeNil: Optional<Type>
 ```

有點冗長，所以 swift 很貼心的提供語法糖 `?`，使用方法是在`型別的後面`加上 `?` 。

值的部分，則是使用 `nil` 表示。

```swift
let intMaybeNil: Int? = nil

// 對照一般情況
let intAbsValue: Int = 100

// 當然 optinoal 是表示 `有可能` 沒有值，所以你也可以這樣宣告
let intMaybeNil2: Int? = 100
```

> Note: Optional 如果宣告為 let 並且一開始值就設定為 nil，那它將永遠是 nil ，因為 let 不可變。
>
> 所以使用到 optional 的時候通常會宣告為 var。



* 如果我們再定義型別的時候沒有指明變數是 Optional ，那麼在未來不管何時何地，這個變數永遠不可能為 nil

```swift
var number = 100
number = nil // 🚫 編譯器會出現警告，因為我們並沒有宣告 number 可能為 nil

var number: Int? = 100
number = nil // ✅ 合法的宣告與使用
```

* 那什麼時候會出現 nil 呢？🌰

```Swift
var str = "123"
var number = Int(str)
print(number)
// Optional(123)

str = "一二三"
number = Int(str)
print(number)
// nil

print(type(of: number))
// Optional<Int>
```

因為系統不知道你的 `str` 中會存放的是什麼，如果是 `一二三` 這種字串，系統是無法自動幫忙轉成 `Int` 的，所以在這種情況下，`number` 的型別會是 `Int?`



### 使用的部分 <div id ="tag_2"></div>