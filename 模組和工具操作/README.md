# 使用模組與工具執行操作
## (1-5%)

### New

```
1程式中要引入random套件的randint()函式，並指定函式名稱為ranInt，此時應該使用下列哪個敘述？

① from random.randint as ranInt

② from random import randint as ranInt

③ import random.randint as ranInt

④ import randint from random as ranInt


-------------------------------------
②
```

```
2下列程式碼執行時在第2行產生錯誤，請問導致錯誤的原因是什麼？

01 def read_word(fileName):
02     if os.path.isfile(fileName):
03         f = open(fileName, 'r')
04         for words in f:
05                 print(words)

① 需要引入 os 套件(函式庫)

② os 套件中沒有path物件

③ path物件中沒有isfile方法	

④ isfile方法需要使用兩個引數

--------------------------------
①
```

```
3要產生最小值為 2、最大值為 10的隨機整數亂數，可以使用下列哪兩個指令？

① random.randrange(2, 11, 1)

② random.randrange(2, 10, 1)

③ random.randint(2, 10)

④ random.randint(2, 11)


-------------------------------------
① ③
```

```
4要顯示最小值為 0.0、最大值為 1.0的隨機浮點數亂數，可以使用下列哪個敘述？

① random.random()

② random.randrange(0.0, 1.0)

③ random.randint(0, 1)

④ random.randrange()


------------------------------------
①
```

```
5請問下列哪兩個指令可以產生符合如下條件的隨機亂數？

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


--------------------------------
① ③
```

```
6如果要設計一個符合如下條件的處理數字函式，請問要使用下列哪兩個函式？

• 函式的傳入值為浮點數資料型別。
• 函式的傳回值是浮點數的絕對值。
• 函式的傳回值是整數，浮點數的小數部分要捨棄。

① math.fabs()

② math.floor()

③ math.ceil()

④ math.fmod()

⑤ math.round()


----------------------------------------
①②
```
### Old

1 使用內建模組執行基本操作
	
	- 數學；日期時間；IO；SYS；OS 路徑；隨機

2 透過使用內建模組解決複雜運算問題

	- 數學；日期時間；隨機

```
程式中使用數學運算函數，則在程式開頭處應匯入哪一個套件？

① random    ② time    ③ file    ④ math
```

```
random.randint(1,100) % 10 + 3 敘述的功能，可以取得什麼範圍的亂數值？

① 3~10    ② 3~13    ③ 3~12    ④ 1~13
```

```
math.fabs() 函式的功能為何？

① 取得 0~1 之間的亂數
② 取得數值的絕對值
③ 指數計算
④ 數值無條件進位

```

```
下列何者不可能為 random.randint(3,30) 的回傳值？

① 3    ② 30    ③ 2    ④ 29

```

```
匯入 time 套件時，將 time 套件另外命名為 TM，則匯入的敘述下列何正確？

① import time as TM
② from time as TM
③ from time import * as TM
④ import time from TM

```

```
若要隨機產生 4、8、12、16、24 … 32、36的亂數，則下列哪個敘述正確？

① random.randint(4, 36, 4)
② random.randrange(4, 36, 4)
③ random.randint(4, 36)
④ random.randrange(4, 37, 4)

```

```
若要隨機產生 0.0 ~ 1.0 之間的浮點數，則下列哪個敘述正確？

① random.random(0.1, 1.0)
② random.random()
③ random.randint(0, 1)
④ random.randrange(0.1, 1.0, 0.1)

```

```
time套件函式中，哪一個函式可在程式執行的期間，使暫停一段時間？

① localtime()
② ctime()
③ sleep()
④ time()

```

```
下列何者不是 random.choice('abcd1234') 函式所取得的字元？

① ‘h’       ② ‘3’       ③ ‘4’       ④ ‘c’

```