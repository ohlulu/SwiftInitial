# Swift 語法介紹

   1. 常數、變數宣告（命名規則、保留字）

      * 小寫開頭
      * 駝峰式

   2. 註解（單行、多行、巢狀）

      ```swift
      // <- 單行註解
      ```

      ```swift
      /*
       多行註解
       */	
      ```

      ```swift
      /*
       /*
       巢狀註解 (不重要)
       */
      */
      ```

   3. 型別宣告、型別標注

       ```swift
       // 宣告一個整數變數
       var number: Int

       // 宣告一個字串常數
       let str: String = "It is a string ."
       ```

   4. 型別安全、型別推斷

       ```swift
       // swift 會推斷出 number 變數是整數
       var number = 1 
       print(type(of: number))
       ```


1. 運算子

   1. 運算子（ \+ \- \* / %）（複合運算）
   2. 比較運算子 
      * 等於（`a == b`）
      * 不等於（`a != b`）
      * 大於（`a > b`）
      * 小於（`a < b`）
      * 大於等於（`a >= b`）（🚫 =<）
      * 小於等於（`a <= b`）（🚫 =>）
   3. 邏輯運算子 （not、and、or）
   4. 優先順序（）

2. 資料型態

   1. Int, String, Bool, Double ( Float ), tuple….

   2. String 的基本運用（結合、變數、）

   3. 集合型別 (Array, Dictionary, Set)

      1. Array

      ```
       * Array 陣列
       * 一個`有序`的資料集合，利用 Index 來取出陣列中的值
       * 利用 , 來區分每一組數值
       * ex: let arr = [0, 1, 2]
       * arr[0]
       * arr[1]
       * note: 存放的內容，必須明確的讓 swift 知道：陣列中存放的型別是什麼
      ```

      2. Dictionary

      ```
       * Dictionary 字典
       * 一種`無序`的資料集合，是一組 key value
       * 用 : 區分 key valueㄝ，左邊是 key，右邊是 value
       * 一樣用 , 來區分每一組數值
       * key 必須是唯一
       * 用 key 來取值
      ```

      3. Set

      ```
       * 一種`無序`的資料集合，跟 Array 很像，但存放的值必須是唯一
      ```
