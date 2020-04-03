# 模組和工具操作
## 16%
```
程式中要引入random套件的randint()函式，並指定函式名稱為ranInt，此時應該使用下列哪個敘述？

① from random.randint as ranInt

② from random import randint as ranInt

③ import random.randint as ranInt

④ import randint from random as ranInt

```

```
下列程式碼執行時在第2行產生錯誤，請問導致錯誤的原因是什麼？

01 def read_word(fileName):
02     if os.path.isfile(fileName):
03         f = open(fileName, 'r')
04         for words in f:
05                 print(words)

① 需要引入 os 套件(函式庫)

② os 套件中沒有path物件

③ path物件中沒有isfile方法	

④ isfile方法需要使用兩個引數
```

```
要產生最小值為 2、最大值為 10的隨機整數亂數，可以使用下列哪兩個指令？

① random.randrange(2, 11, 1)

② random.randrange(2, 10, 1)

③ random.randint(2, 10)

④ random.randint(2, 11)

```

```
要顯示最小值為 0.0、最大值為 1.0的隨機浮點數亂數，可以使用下列哪個敘述？

① random.random()

② random.randrange(0.0, 1.0)

③ random.randint(0, 1)

④ random.randrange()

```

```
請問下列哪兩個指令可以產生符合如下條件的隨機亂數？

• 亂數是 3 的倍數。
• 最小值為3，最大值為90。

① from random import randint
	randint(1, 30) * 3
	
② from random import randint
    randint(0, 30) * 3
    
③ from random import randrange
	randrange(3, 91, 3)
	
④ from random import randrange
	randrange(0, 91, 3)

```

```
如果要設計一個符合如下條件的處理數字函式，請問要使用下列哪兩個函式？

• 函式的傳入值為浮點數資料型別。
• 函式的傳回值是浮點數的絕對值。
• 函式的傳回值是整數，浮點數的小數部分要捨棄。

① math.fabs()

② math.floor()

③ math.ceil()

④ math.fmod()

⑤ math.round()

```
