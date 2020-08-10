# 執行疑難排解與錯誤處理
## (5-10%)

### New
	
```
1如果test61.txt檔案不存在，請評估下列程式碼執行的情形？

01 import sys
02 try:
03      fName = 'test61.txt'
04      file = open(fName, 'r')
05 except IOError:
06      print(fName + '檔案無法開啟!')
07 else:
08     i = 1
09     for data in file:
10           print(data.rstrip())
11           i += 1
12     file.close()

① 程式碼可以執行，不需修改程式。
② 程式碼會產生執行階段錯誤。
③ 程式碼可以執行，但會有邏輯錯誤。
④ 程式碼會產生語法錯誤。

--------------------------------
①
```

```
2下列程式碼是計算num連除遞增整數的值，請問執行的結果為何？

01 ok = True
02 i = 0
03 num = 15000
04 05 while(ok):
06      if i <= 8:
07           num = num / i
08           i += 1
09      else:
10           ok =False
11 print(num)

① 第05 行敘述會造成無窮迴圈程式不會終止。
② 第05 行敘述有語法錯誤，應該改為while(ok == True): ③ 第07 行敘述會因為除數為零，而造成執行階段錯誤。
④ 第08 行敘述有語法錯誤，應該改為i = i + 1。


-------------------------------------
③
```

```
3下列為計算學生成績的程式碼，程式執行後發現計算結果不正確，請回答下列問題來修改程式碼：

01 stuScore = [85, 72, 65, 45, 93]
02 num = 0
03 total = 0
04 for i in range(len(stuScore) - 1):
05      num += 1
06      total += stuScore[i]
07      avg = total // num
08 print('成績總分為：', total)
09 print('平均成績為：', avg)

A：第04行敘述應該改用下面哪個敘述？
① for i in range(1, len(stuScore) - 1):
② for i in range(len(stuScore) + 1):
③ for i in range(len(stuScore) - 1):
④ for i in range(len(stuScore)):

B：第07行敘述應該改用下面哪個敘述？
① avg = total / num
② avg = total % num 
③ avg = total * num	
④ avg = total ** num


------------------------------------
A:④
B:①
```

```
4下列為讀取資料檔案，並且列印檔案中的每一字的函式。
為使萬一檔案不存在，程式碼也能正確執行，請問下列哪三行敘述必須增加縮排？

01 import os
02 def read_file(fileName):
03     cap = None
04     if os.path.isfile(fileName):
05         file = open(fileName, 'r')
06     while cap != '':
07         cap = file.read(1)
08         print(cap)

① 第1行    ② 第2行    ③ 第3行    ④ 第4行

⑤ 第5行    ⑥ 第6行    ⑦ 第7行    ⑧ 第8行


------------------------------------------
⑥ ⑦ ⑧
```

```
5下列為讀取串列元素內容，並且讀到指定元素內容時結束的程式碼。
但是執行有錯誤產生，請回答下列問題來修改程式碼。

01 datas = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J']
02 i = 0
03 while (i < 10)
04     print(datas[i])
05     if datas[i] = 'D'
06         break
07     else:
08         i += 1

A：第03行敘述應該使用下面哪個敘述？
① while (i < 10):
② while (i < 11):
③ while (i < 9):
④ while [i < 11]

B：第05行敘述應該使用下面哪個敘述？
① if datas[i] = 'D':
② if datas[i] == 'D':
③ if datas(i) != 'D':
④ if datas[i] != 'D':


------------------------------------------
A:① 
B:②
```

```
6下列關於try語法的說明是否正確，請填入是 、 否。
A：try 的語法中，可以有一個或是多個except 敘述。

B：try 的語法中，可以有一個沒有except 敘述的 finally 敘述。

C：try 的語法中，可以有一個finally 敘述和except 敘述。 

D：try 的語法中，可以有一個或是多個finally 敘述。 


--------------------------------------
A:是
B:是
C:是
D:否
```

```
7下列為不斷接受使用者輸入整數值，直到輸入正確為止的程式碼
請回答下列問題來完成程式碼：

01 while True:
02    _______________________________________
03         num = int(input('請輸入一個整數：'))
04         break
05   _______________ValueError:
06         print('這不是整數！')

A：第02行應該使用下面哪個敘述？
① try:    ② finally:    ③ except:    ④ else:    ⑤raise:

B：第05行敘述應該填入下面哪個指令？
① try:    ② finally:    ③ except:    ④ else:    ⑤raise:


--------------------------------------------
A:①
B:③
```
### old  
1 分析、偵測及修復出現錯誤的程式碼區段

	- 文法錯誤、邏輯錯誤、運行時間錯誤

2 分析與建構處理例外狀況的程式碼區段

	- 嘗試；排除；其他；最終；改善

```
例外處理可以應用在哪一種錯誤？

① 邏輯錯誤
② 執行時期錯誤
③ 語法錯誤
④ 檔案錯誤

```

```
使用try敘述，至少要多少個except 配合？

① 0個      ② 1個      ③ 2個      ④ 3個

```

```
程式在處理例外時，finally敘述區段被執行的情況為何？

① 無論例外是否會發生，都會執行。
② 只要有例外發生時，就會執行。
③ 有例外發生時，不會執行；沒有例外發生時，才會執行。
④ 程式中斷時執行

```

```
下列有關例外處理的敘述何者錯誤？

① 當程式在執行時期發生錯誤或不正常狀況，稱之為例外。
② 若程式沒有設計例外處理，當發生例外時，程式照常執行。
③ 使用try敘述，至少要一個except配合。
④ finally敘述區段可以省略。

```

```
檔案處理遇到檔案找不到時產生錯誤，是哪一種例外處理？

① except NameError
② except FileNotFoundError
③ except IOError
④ except IndexError 

```
