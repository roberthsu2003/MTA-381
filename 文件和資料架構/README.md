# 文件和資料架構
```
請問下列哪個註解程式碼文件的語法是正確？
① def get_average():
         /* 傳回目前平均分數*/
         return average 
         
② // 傳回目前平均分數
    def get_average():
         return average
         
③ ' 傳回目前平均分數
    def get_average():
         return averag
         
④ def get_average():
         # 傳回目前平均分數
         return average
```

```
若要在程式碼中添加文字說明，以便其他成員能夠注意，請問下列哪個
作法是正確？
 ① 將說明文字單獨成行，並且放在括弧內。
② 將說明文字放在任一行的 # 符號之後。
③ 將說明文字放在最後一行程式碼之後，並且用空行區隔。
④ 將說明文字放在第一行程式碼之前，並且用空行區隔 。
```

```
下列為計算方形面積的函式，關於程式碼註解的說明是否正確
請填入 是 或 否。

01 # area 是計算方形面積的函式
02 # w 和 h 分別為方形的寬和高
03 # 傳回 w * h 的值
04 def area(w, h):
05      calc_area = '# 計算方形面積'
06      return w * h # 傳回值

A：第01 ~ 03 行敘述在語法檢查時會被忽略。

B：第02行敘述前的 # 號可以省略。

C：第05行敘述中的字串在語法檢查時會被視為註解。

D：第06行敘述中有包含內嵌的註解。
```

```
下列為計算喝珍珠奶茶攝取熱量的程式碼，其中包含兩個函式，
請從下列敘述中選擇兩個來定義函式

________________________________________
02      name = input("請輸入姓名：")
03      return name
________________________________________
05      total_cal = num * calories
06      return total_cal
07 user = input_name()
07 cups = int(input(user + "請輸入一天喝幾杯珍珠奶茶？"))
08 print(user + " 你攝取了", calc(cups, 160), "大卡")

① 01 def input_name():
② 01 def input_name(user):
③ 01 def input_name(name):
④ 04 def calc():
⑤ 04 def calc(num, total_cal):
⑥ 04 def calc(num, calories):

```

```
下列為計算學生加分的程式碼，其中add_score函式的功能如下：

• 函式傳回值是原始分數(score)加上加分(add)。
• 如果rest為False，表學生全勤加分加倍。
• 如果函式沒有傳入add變數時，預設值為 1。

關於程式碼敘述的說明是否正確
請填入 是 、 否

01 def add_score(score, rest, add):
02      if rest == False:
03           add *= 2
04      return score + add
05 stuScore = 75
06 addScore = 2
07 isRest = True
08 newScore = add_score(stuScore, isRest, addScore)

A：第01行敘述要修改如下，才能符合函式的功能需求。   01 def add_score(score, rest, add = 1): 
  
B：只要為任何參數定義預設值，則其右側的參數也必須定義預設值。

C：如果呼叫函式時只傳兩個參數時，則第三個參數的值為 None。

D：執行第03 行敘述後，第 06 行的addScore變數值會被改變。
```

```
下列為計算帳戶金額的函式，函式要符合如下條件：

• 函式的名稱為save_money。
• 函式會接受原帳戶金額(money)和存款金額(save)兩個參數。
• 函式會將存款金額加到帳戶金額中。
• 函式會傳回計算後的帳戶金額。

請回答下列問題，來完成函式程式碼：
01 ________A__________ _________B___________
02      money += save
03 ______________________

A：第01行敘述中的A ，應該使用下面哪個指令？
① save_money      ② def save_money      ③ return save_money

B：第01行敘述中的B ，應該使用下面哪個指令？
① (money, save):      ② ():     ③ (money, save)       ④ ()

C：第03行敘述應該使用下面哪個敘述？
① return save    ② return money    ③ return     ④ return save_money

```