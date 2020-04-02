# 資料類型的運算式
```
下列哪個浮點數常值最大？

① 1.234    ② 1.234e2    ③ 1.234e6   ④ 1.234e-4
```

```
下列哪個變數宣告方式錯誤？

① a    ② a=5    ③ a, b=5    ④ a, b=5, 1.4
```

```
下列哪個資料使用bool()函式轉型後，結果為False？

 ① ' '(空字串)    ②'False'     ③ 1    ④ -1
```

```
a = a + b  敘述可以改寫為何？

① a = +b    ② a = b    ③ b =  a + b    ④ a += b 
```

```
7 / 2 和 7 // 2運算式的值是屬於下列哪種資料型別？

① float  int    ② int float    ③ float float    ④ int int
```

```
請問x和y的值為下列何者時，會使邏輯運算式not(x or y)的結果為True(真)?

① x=1 y=0     ② x=1 y=1     ③ x=0 y=0     ④ x=0 y=1
```

```
請問要將'12.5'字串轉型為浮點數數值，可以使用下列哪個函式?

① bool()     ② float()     ③ int()     ④ str() 
```

```
請問input()函式執行後，使用者所輸入的整數資料，會以下列哪種資料型別傳回?

① bool     ② float     ③ int     ④ str  
```

```
要計算變數x加5再乘以3然後取平方，最後指定給變數y，請問下列哪個敘述正確?

① y=((x+5)*3)**2     ② x=((y+5)*2)**3   ③ y=(x+5*3)*2    ④ y=((x+5)*2)**3
```

```
請問0 or 3和3 and 'a'兩個運算式執行的結果為何?

① True False     ② 3 'a'     ③ 0 3     ④ True True
```

```
x=13、y=2，請問x/y、x//y和x%y運算式執行的結果分別為何?

① 6、6.5、1     ② 6.5、1、6     ③ 6.5、6、1     ④ 6、1、6.5
```

```
Python比較(關係)運算子所傳回的結果為哪種型別的資料？

① 布林  ② 整數  ③ 字元  ④ 字串
```

```
python比較(關係)運算式的結果為真，則會傳回什麼資料？

①  True  ② 0  ③ 真  ④ 1
```

```
Python比較運算式的結果為假，則會傳回什麼資料？

①  False    ② 0    ③ 偽    ④ -1
```


```
以下程式碼，執行時輸出值為何?

lst_1 = [1, 2]
lst_2 = [3, 4]
lst_3 = lst_1 + lst_2 
lst_4 = lst_3 * 2 
print(lst_4)

① [8, 12]
② [[1, 2], [3, 4], [1, 2], [3, 4]]
③ [1, 2, 3, 4, 1, 2, 3, 4]
④ [[1, 2, 3, 4], [1, 2, 3, 4]]
```

```
以下是計算跑步平均時速的程式碼，輸出結果要盡可能精準。
請問A、B處的程式碼應該為何？

distance = ____A_____(input('請輸入距離(單位：公尺)：'))
time =_____B_____ (input('請輸入時間(單位：秒)'))
avg = distance / 1000 / time / 3600
print('平均時速 = ', avg, ' 公里/小時')

A: ① int    ② string    ③ float   ④ bool
B: ① int    ② float     ③ string  ④ bool
```

```
已知商店營業額(total)和顧客人數(num)，要顯示顧客的平均消費金額，輸出時必須去除小數部分，請問下列哪兩個程式碼正確？

① avg = total / num
② avg = int(total / num)
③ avg = float(total // num)
④ avg = total // num
```

```
列各種資料，其正確資料型別為何？請填入下列型別 bool、float、int、str

A：  _______height = 172  
B：  _______pass = True
C：  _______name = "張無忌"
D：  _______score = 98.0
E：  _______tel = '0928000000'  

```

```
下列是年齡計算程式，請問程式中變數的資料型別為何？請填入下列型別 bool、float、int、str：

01 born = input("請輸入出生的民國年： ")
02 year = input("請輸入現在的民國年： ")
03 age = eval(year) - eval(born)
04 msg = "你的年齡是： " + str(age)
05 print(msg)

A: 在 01 行中 born 的資料型別為何？
B: 在 03 行中 age 的資料型別為何？
C: 在 04 行中 msg 的資料型別為何？
```

```
下列程式碼執行後，變數的資料型別是否正確，請填入 是 、 否。
01 x1 = '5'
02 y1 = 4
03 a = x1 * y1
04 x2, y2 = 6, 3 05 b = x2 / y2
06 x3, y3 = 1.0, 2
07 c = x3 + y3

A：_________變數 a 的資料類型為 str。
B：_________變數 b 的資料類型是 float。
C：_________變數 c 的資料類型為 int。 
```

```
下列常值請用bool、float、int、str填入正確的資料型別：

A：______type(+5E10)
B：______type(4.0)
C：______type("False ")
D：______type(True)

```

```
下列程式碼是用來以座號查詢學生姓名，但執行結果並不正確，請回答下列問題，來找出可能的錯誤。

01 datas = {1: '張三', 2: '李四', 3: '王五'}
02 num = input('請輸入座號: ')
03 if not num in datas:
04     print('該座號不存在！')
05 else:
06     print("學生姓名為： " + datas[num])

A：第01 行敘述的datas 字典中，儲存哪兩種資料類型？
① string、bool    ② float、string   ③ int、string      ④ int、float

B：第 02 行敘述的 num 變數的資料型別為何？
① bool    ② float     ③ int   ④ string   

C：第 03 行敘述執行時，為何在 datas 字典中找不到資料?  ① 程式邏輯錯誤    ② 資料型別不匹配     ③ 變數名稱誤用保留字   ④ 語法不正確
```

```
下列是用來查詢傳入值資料型別的函式，請根據執行結果回答下列問題

01 def dataType(val):
02      return type(val)
03 print(dataType(False))
04 print(dataType(3.0))
05 print(dataType(3))
06 print(dataType("False"))

A：第03 行敘述的執行結果為何？
① <class'bool'>    ② <class'float'>    ③ <class'int'>      ④ <class'str'>

B：第04 行敘述的執行結果為何？
① <class'bool'>    ② <class'float'>    ③ <class'int'>      ④ <class'str'>

C：第05 行敘述的執行結果為何？
① <class'bool'>    ② <class'float'>    ③ <class'int'>      ④ <class'str'>

D：第06 行敘述的執行結果為何？
① <class'bool'>    ② <class'float'>    ③ <class'int'>      ④ <class'str'>
```

```
讓使用者輸入一個整數值，但即使輸入小數也能轉換為整數，請問下列哪個敘述符合要求？

① num = input("請輸入整數：")
② num = int((input("請輸入整數："))
③ num = float(input("請輸入整數："))
④ num = str(input("請輸入整數："))
```

```
下列函式可以將傳入的字串，以相反的順序重組後傳回新字串，請回答下列問題來完成程式碼。

01 def reverse_word(old_word):
02     word = ''
03     for index in________:
04         word +=_______ 05     return word 06 print(reverse_word("nohtyP"))

A：第03 行敘述的空格應該填入下列哪個指令？
① range(len(word) + 1)
② range(len(old_word) - 1)  ③ range(len(old_word))
④ range(len(old_word) - 1, -1, -1)

B：第04 行敘述的空格應該填入下列哪個指令？
① old_word[index-1]
② old_word[len(old_word)-len(word)]
③ old_word[len(word)-1]
④ old_word[index]

```

```
以下程式碼是計算今天遊戲過關數，請問第03 行應該填入下列哪個敘述？
01 last = input("請問你昨天過第幾關?")
02 now = input("請問你今天過第幾關?")
03 ____________________

① print("恭賀你今天通過了 " + str(int(now) - int(last)) + " 關!")
② print("恭賀你今天通過了 " + (int(now) - int(last)) + " 關!")
③ print("恭賀你今天通過了 " + str(int(now - last)) + " 關!")
④ print("恭賀你今天通過了 " + str(now - last) + " 關!")

```

```
如果word = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ' 時，請用代碼填入下列分割操作的結果：

①ZWTQNKHEB、②PMJG、③DEFGHIJKLMNO、④PONMLKJIHGFE、⑤DEFGHIJKLMNOP、⑥DGJM、⑦OLIF、⑧""

A：word[3:15]
B：word[3:15:3]
C：word[3:15:-3]
D：word[15:3:-3]
E：word[15:3]
F：word[::-3]
```

```
14.students 串列(清單)包含 100 位學生的姓名，最後15位為轉出學生。如果要分割串列顯示目前在校學生，請問可以使用下列哪兩個指令？

① students[0:-14]
② students[0:-15]
③ students[1:-14]
④ students[:-15]
⑤ students[1:-15]

```

```
books 串列(清單)包含 300 本書的編號，如要取得第2個編號開始到最後，而且間隔1個編號的串列(如：2, 4, 6…)，請問可以使用下列哪個指令？

① books[2:2]    ② books[::2]    ③ books[1::2]    ④ books[1:2]

```

```
下列程式碼中，x是使用者輸入的整數，y 等於 x 乘以 -1，然後再平方。
要確保結果正確，請用代碼填入完成第2行的敘述：(可使用一次、多次、或不使用)

01 x = eval(input("請輸入一個整數："))
02 y = _______________________
                                  
① -
② (
③ )
④ *2
⑤ **2
⑥ 2
⑦ x

```

