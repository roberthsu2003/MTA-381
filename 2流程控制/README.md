# 控制帶有決策與迴圈的流程
## (25-30%)

### New

```python
1.下列為換算成績等級的程式碼，換算的規則如下：

• 90(含)~100分為「優」
• 80(含)~89分為「甲」
• 70(含)~79分為「乙」
• 60(含)~69分為「丙」
• 0(含)~59分為「丁」

請回答以下問題來完成程式：
01 score = int(input("請輸入分數"))
02__________________________
03     grade = '優'
04__________________________
05     grade = '甲'
06__________________________
07     grade = '乙'
08__________________________
09     grade = '丙'
10 else:
11     grade = '丁'
12 print("成績等級為：", grade)

A：請問第2行應該填入下列哪段敘述？

① if score <= 90:
② if score >= 90:
③ if score > 90:
④ if score == 90:
 
B：請問第4行應該填入下列哪段敘述？

① if score >= 80:
② elif score >= 80:
③ elif score > 80:
④ else if score >= 80: 

C：請問第6行應該填入下列哪段敘述？

① if score >= 70:
② elif score >= 70:
③ elif score > 70:
④ else if score >= 70:
 
D：請問第8行應該填入下列哪段敘述？

① if score >= 60:
② elif score >= 60:
③ elif score > 60:
④ else if score >= 60: 

-----------------------------------
A:②
B:②
C:②
D:②

score = int(input("請輸入分數"))
if score >= 90:
    grade = '優'
elif score >= 80:
    grade = '甲'
elif score >= 70:
    grade = '乙'
elif score >= 60:
    grade = '丙'
else:
    grade = '丁'
    
print("成績等級為：", grade)
```

```
2.下列為根據最低年齡制定電影分級的函式，假設電影分級的規則如下：

• 限制級：18歲或以上皆可欣賞。
• 輔導級：13(含) ~ 17歲以上皆可欣賞。
• 普遍級：12(含)歲以下皆可欣賞。
• 如果沒有輸入年齡預設為普遍級。

請回答以下問題來完成程式：
01 def movie(age = None):
02     rating = ""
03     if ________________________________
04     elif ______________________________
05     elif ______________________________
06     else ______________________________
07     return rating

A：請問第3行應該填入下列哪個字串？

① age < 13: rating = "普遍級"
② age < 18: rating = "輔導級"
③ : rating = "限制級"
④ age == None: rating = "普遍級"

B：請問第4行應該填入下列哪段條件式？

① age < 13: rating = "普遍級"
② age < 18: rating = "輔導級"
③ : rating = "限制級"
④ age == None: rating = "普遍級"

C：請問第5行應該填入下列哪段條件式？

① age < 13: rating = "普遍級"
② age < 18: rating = "輔導級"
③ : rating = "限制級"
④ age == None: rating = "普遍級"

D：請問第6行應該填入下列哪段條件式？

① age < 13: rating = "普遍級"
② age < 18: rating = "輔導級"
③ : rating = "限制級"
④ age == None: rating = "普遍級"

---------------------------
A:④
B:①
C:②
D:③

def movie(age=None):
    rating = ""
    if age == None: rating = "普遍級"
    elif age < 13: rating = "普遍級"
    elif age < 18: rating = "輔導級"
    else: rating = "限制級"
    return rating
    
print(movie())
print(movie(12))
print(movie(16))
print(movie(19))
```

```
3.下列為計算方根的get_root函式，方根計算的規則如下：

• 函式接受x、y兩個參數。
• 如果x不是負數，則傳回值為 x ** (1 / y)。
• 如果x是負數而且為偶數，則傳回值為"虛數"。
• 如果x是負數而且為奇數，則傳回值為 -(-x) ** (1 / y)。

請回答以下問題來完成程式：
01 def get_root(x, y):
02      ________________________
03           root = x ** (1 / y)
04      ________________________
05           ____________________
06                root = "虛數"
07           ____________________
08                root = -(-x) ** (1 / y)
09      return root

A：請問第2行應該填入下列哪個敘述？
① if x >= 0:    ② if x % 2 == 0:    ③ else:    ④ elif: 

B：請問第4行應該填入下列哪個敘述？
① if x >= 0:    ② if x % 2 == 0:    ③ else:    ④ elif: 

C：請問第5行應該填入下列哪個敘述？
① if x >= 0:   ② if x % 2 == 0:    ③ else:    ④ elif: 

D：請問第7行應該填入下列哪個敘述？
① if x >= 0:    ② if x % 2 == 0:    ③ else:    ④ elif: 

-------------------------------------
A:①
B:③
C:②
D:③

def get_root(x, y):
    if x >= 0:
        root = x ** (1 / y)
    else:
        if x % 2 == 0:
            root = "虛數"
        else:
            root = -(-x) ** (1 / y)
    
    return root

print(get_root(5, 10))
print(get_root(-5,10))
print(get_root(-6,10))
```

```
4.下列為遊樂場門票費用的函式，門票費用的規則如下：

• 5(不含)歲以下免費入場。
• 5(含)歲以上的當地居民門票為100元。
• 5 ~ 17歲的非當地居民門票為200元。
• 18(含)歲的非當地居民門票為300元。

請回答以下問題來完成程式：
01 def price(age, locate):
02     money = 0
03     __________________________________
04          money = 100
05     __________________________________
06          _____________________________
07               money = 200
08          else:
09               money = 300
10     return money

A：請問第3行應該填入下列哪段敘述?

① if age >= 5 and locate == True:
② if age >= 5 or locate == False:
③ if age >= 5 and locate == False:
④ if age >= 5 and age <= 17:

B：請問第5行應該填入下列哪段敘述？

① elif age >= 5 and locate == False:
② else age >=5 and locate == False:
③ elif age >= 5 or locate == False:
④ elif age >= 5 and locate == True:
  
C：請問第6行應該填入下列哪段敘述？
① if age < 16:
② if age >= 5 and locate == False:
③ if age <= 17:
④ elif age >= 5 and locate == True:


-----------------------------------------------
A:①
B:①
C:③

def price(age, locate):
    money = 0
    if age >= 5 and locate == True:
        money = 100
    elif age >= 5 and locate == False:
        if age <= 17:
            money = 200
        else:
            money = 300
    
    return money

print(price(3, False))
print(price(10, True))
print(price(5, False))
print(price(18, False))
```

```
5.下列為檢查輸入整數位數的程式碼，請回答以下問題來完成程式：

01 n = int(input("請輸入整數："))
02 _______________________________
03     digit = "一"
04 _______________________________
05     digit = "二"
06 _______________________________ 
07     digit = "大於二"
08 print(n,"是" ,digit + "位數")

A：請問第2行應該填入下列哪段敘述？

① if n > -10 and n < 10:
② if n > -9 and n < 9:
③ if n > -10 or n < 10:
④ if n > -99 or n < 99:

 
B：請問第4行應該填入下列哪段敘述？

① if n > -100 and n < 100:
② elif n > -100 and n < 100:
③ if n > -100 or n < 100:
④ elif n > -100 or n < 100: 


C：請問第6行應該填入下列哪段敘述？

① else:    ② elif:    ③ elseif:    ④ else  if: 


---------------------------------

n = int(input("請輸入整數："))

if n > -10 and n < 10:
    digit = "一"
elif n > -100 and n < 100:
    digit = "二"
else:
    digit = "大於二"

print(n,"是" ,digit + "位數")

A:①
B:②
C:①
```

```
6.下列為猜1到20亂數整數的程式碼，猜對就結束程式, 猜錯就顯示訊息最多可以猜4次。
請用代碼填入以下問題來完成程式：


01 from random import randint
02 ans = randint(1, 20)
03 times = 1
04 print("猜 1 到 20 的整數，猜錯4次結束程式！")
05 __________________________
06     guess = int(input("請輸入1 ~ 20的整數："))
07     if guess > ans:
08         print("太大了！")
09     elif guess < ans:
10         print("太小了！")
11     else:
12         print("答對了！")
13         ______________________
14     __________________________

① while times <= 4:
② while times < 4:
③ break 
④ pass
⑤ times +=1
⑥ while times < 4
⑦ times = 1

A：第5行的敘述為何？

B：第13行的敘述為何？

C：第14行的敘述為何？ 

--------------------------------------
A:①
B:③
C:⑤  

from random import randint
ans = randint(1, 20)
times = 1
print("猜 1 到 20 的整數，猜錯4次結束程式！")
while times <= 4:
    guess = int(input("請輸入1 ~ 20的整數："))
    if guess > ans:
        print("太大了！")
    elif guess < ans:
        print("太小了！")
    else:
        print("答對了！")
        break

    times +=1
print('程式結束')                        
```

```
7.請用代碼填入以下問題來完成程式：

01 list1 = [1, 2, 3, 4]
02 list2 = ["1", "2", "3", "4"]
03 ___________________
04     print("兩個串列的值相同")
05 ____________________
06     print("兩個串列的值不相同")

① if list1 == list2:
② if list1 == list2
③ else:
④ else


A：第3行的敘述為何？

B：第5行的敘述為何？

-----------------------------------

A:①
B:③

list1 = [1, 2, 3, 4]
list2 = ["1", "2", "3", "4"]
if list1 == list2:
    print("兩個串列的值相同")
else:
    print("兩個串列的值不相同")
```

```
8._________請利用下列中的四個敘述區段，組合成一個檢查輸入字串中字母大小寫的程式
(請填入代碼)。

① word = input("請輸入英文單字：")
② elif word.upper () == word:
     print(word, "全部大寫字母")
③ else:
    print(word, "全部小寫字母")
④ else:
    print(word, "有大、小寫字母")
⑤ if word.lower() == word:
    print(word, "全部小寫字母")
⑥ else:
	print(word, "全部大寫字母")
    
-----------------------------------
① ⑤ ② ④

word = input("請輸入英文單字：")

if word.lower() == word:
    print(word, "全部小寫字母")
elif word.upper() == word:
    print(word, "全部大寫字母")
else:
    print(word, "有大、小寫字母")
    
```

```
9.下列為由score串列讀取成績，並調整成績的程式碼。調整成績的規則如下：

• 成績高於60(含)分不調整。
• 60以下的分數乘以1.1後再加2分。

請回答以下問題來完成程式
01 ________________________
02     if score[i] >= 60:
03          _________________
04     score[i] =int(score[i] * 1.1) + 2

A：請問第1行應該填入下列哪段敘述？
① for i in range(len(score) - 1):
② for i in range(len(score) + 1):
③ for i in range(len(score)):
④ for i in score: 

B：請問第3行應該填入下列哪段指令？

① break    ② continue    ③ exit()    ④ end 

------------------------------
A:③
B:②

score = [57, 78, 69, 92, 35]

for i in range(len(score)):
    if score[i] >= 60:
        continue
    else:
        score[i] = int(score[i] * 1.1) + 2
        
print(score)
```

```
10.下列為顯示3 ~ 10乘法表函式的程式碼，請回答以下問題來完成程式：

01 # 顯示 3 X 10 乘法表
02 def print_tables():
03     _____________________________
04         _______________________________
05               print(x, 'X', y, '=', x * y, end = ' ')
06         print()
07 # 主程式
08 print_tables()

A：請問第3行應該填入下列哪段敘述？
① for x in range(11):
② for x in range(3, 11):
③ for x in range(3, 10, 1):
④ for x in range(10): 

B：請問第4行應該填入下列哪段敘述？
① for y in range(11):
② for y in range(3, 10, 1):
③ for y in range(3, 11):
④ for y in range(10): 

-------------------------------
A:②
B:③

def print_tables():
    for x in range(3, 11):
        for y in range(3, 11):
            print(x, 'X', y, '=', x*y , end=' | ')
        print()

print_tables()

```

```
11.請利用下列敘述區段的代碼(可省略或重複使用)，組合成一個顯示 1 ~ 50中間所有質數的程式。

___________A___________
    ________B__________
            _____C_____
           
    if flag == True:
        print(num, end=',')
    _______D_________
    
① num = 2
   while num < 51:
	    flag = True
	    
② num = 2
   flag = True
        while num < 51:
        
③ break

④ continue

⑤ num = num + 1

⑥ for i in range(2, num):
       if num / i == 0:
	       flag = False
	           
⑦ for i in range(2, num):
       if num % i == 0:
           flag = False

A：________請問A此處依序應該填入哪段敘述？ 

B：________請問B此處依序應該填入哪段敘述？ 

C：________請問C此處依序應該填入哪段敘述？ 

D：________請問D此處依序應該填入哪段敘述？ 


--------------------------------
A:①
B:⑦
C:③
D:⑤
實際程式碼
num = 2
while num < 51:
    flag = True
    for i in range(2, num):
        if num % i == 0:
            flag = False
            break
           
    if flag == True:
        print(num, end=',')
    num = num + 1;
```

```
12.請設計一個圖書館藏書搜尋的函式，函式要符合下列條件：

• 函式接受兩個參數分別是串列和字串。
• 函式的功能是在串列中搜尋該字串。
• 如果搜尋找到該字串，就中止搜尋動作。
• 根據是否找到分別顯示文字訊息。

請利用下列敘述區段的代碼，依序組合成藏書搜尋的函式。
___________A____________
___________B____________
___________C____________
___________D____________
___________E____________

① for i in range(len(books)):

②     if books[i] == title:
          print("{0} 在書庫中！".format(title))
             
③     else:
	      print("{0} 不在書庫中！".format(title))
              
④        break

⑤ def find_book(books, title): 

A：請問A此處依序應該填入哪段敘述？ 

B：請問B此處依序應該填入哪段敘述？ 

C：請問C此處依序應該填入哪段敘述？
 
D：請問D此處依序應該填入哪段敘述？
 
E：請問E此處依序應該填入哪段敘述？ 


-----------------------------------
A:⑤
B:①
C:②
D:④
E:③

def find_book(books, title):
	for i in range(len(books)):
		if books[i] == title:
			print("{0} 在書庫中！".format(title))
			break;
		else:
			print("{0} 不在書庫中！".format(title))
			
```

```
13.請設計一個行動電話號碼檢查程式，電話號碼要符合下列條件：
• 格式必須為 0000-000-000，只由數字和破折號-組成。
• 格式正確就顯示True，否則就顯示False。

 請回答以下問題來完成程式：

01 ______________A______________
02 s = ""
03 ______________B______________
04      ______________C____________
05      tel = input("請輸入行動電話號碼(格式為 0000-000-000)：")
06      s = tel.split('-')
07      if len(s) == 3:
08         if len(s[0]) == 4 and len(s[1]) == 3 and len(s[2])== 3:
09             if s[0].isdigit() and s[1].isdigit() and s[2].isdigit():
10                ____________D____________
11      print(flag)

A：請問第1行要填入下列哪段敘述？
① tel = "" 		② tel = "0000-000-000" 

B：請問第3行應該填入下列哪段敘述？
① while tel != "": 	② while tel != "0000-000-000":

C：請問第4行應該填入下列哪段敘述？
① flag = False 	② flag = True

D：請問第10行應該填入下列哪段敘述？ ① flag = False 	② flag = True 


------------------------------------
tel = "0000-000-000"
s = ""
while tel != "":
    flag = False
    tel = input("請輸入行動電話號碼(格式為 0000-000-000)：")
    s = tel.split('-')
    if len(s) == 3:
        if len(s[0]) == 4 and len(s[1]) == 3 and len(s[2])== 3:
             if s[0].isdigit() and s[1].isdigit() and s[2].isdigit():
                    flag = True
    
    print(flag)
    break;



A:②
B:①
C:①
D:②
```

```
14.請設計一個符合下列條件的函式：
• 函式接受兩個參數分別是串列和變數。
• 逐一顯示串列的元素內容。
• 找到變數指定目標時，就進行跳離的動作。

請用回答以下問題來完成程式：
01 datas=['A','B','C','D','E','F','G','H','I']
02 index = 0
03 ________________(index < len(datas)) :
04     print(datas[index])
05     if datas[index] == 'E':
06        ____________________
07     else:
08        ____________________

A：第3行應該填入下列何者？
① while    ② if    ③ for    ④ break

B：第6行應該填入下列何者？
① while    ② if    ③ for    ④ break

C：第8行應該填入下列何者？
① break    ② continue    ③ index +=1    ④ index =1


----------------------------------------
A:①
B:④
C:③
datas=['A','B','C','D','E','F','G','H','I']
index = 0
while(index < len(datas)):
    print(datas[index])
    if datas[index] == 'E':
        break;
    else:
        index += 1
        

```

### old
1 建構與分析使用分支陳述式的程式碼區段

	- if；elif；else；巢狀及復合條件運算式

2 建構與分析執行反覆運算的程式碼區段

	- while；for；中斷；繼續；通過；巢狀迴圈與包含復合條件運算式的迴圈
	
```
下列何者不是Python的重複結構指令？

① for … next   ② for … else    ③ for …    ④ while … 
```

```
請問下列程式碼執行後，輸出結果為何？

01 sum = 0
02 for x in range(10):
03     sum += x
04 print(x,sum,sep = ',')

① 9,45    ② 10,45    ③ 10,55    ④ 11,55
```

```
假如要計算0到10的偶數和，要在02行要使用哪個敘述？

01 sum = 0
02 _____________________
03     sum += x

① for x in range(,10,2):

② for x in range(,11,2):

③ for x in range(0,11,2):

④ for x in range(10,2):

```

```
有一程式碼如下：

01 x = 0
02 while(x = 10):
03     print(x, end= ' ')
04     x += 1

請問迴圈區塊的執行次數為何？
① 1次    ② 0次    ③無限次   ④ 語法錯誤，無法執行

```

```
有一程式碼如下：
01 x = 0
02 while(x <= 10):
03     print(x)
04     x += 1
05     if(x > 9):
06         break

請問迴圈區塊的執行次數為何？
① 9次    ② 10次    ③ 無限次    ④ 0次 
```

```
下列程式碼最後1次輸出的結果是？

01 x = -256
02 while(x):
03     print(x)
04     x += 1

① -1    ② 0    ③ 1    ④ 語法錯誤，無法執行 

```

```
有一程式碼如下：請問迴圈區塊的執行次數為何？

01 for x in range(1 , 5):
02    x = x - 1 

① 無限次    ② 0次    ③ 4次   ④ 5次
```

```
下列程式希望能列印20次的「Hi!」，請問在range括弧內填入哪一個組引數才能正確列執行？

01 for x in range(   ？   ):
02    print('Hi!')

① 0,100,5    ② 0,101,5    ③ 5,100,5   ④ 21
```

```
對for迴圈的敘述何者是對的？

① 無法轉換成while迴圈
② 至少執行1次迴圈區塊    ③ 可能不會執行迴圈區塊
④ 可產生無窮迴圈
```

```
下列程式碼中，哪一個片段不會被執行？

01 i = 0
02 while(1):
03     i += 1
04     if i > 10:
05         break
06     print(i)
07 else:
08     print('程式結束!')
09 print('時間到!')

① 第5行    ②第6行    ③第8行    ④第9行
```


```
下列何者為s 介於50~59(不包含50和59)之間的條件式？
① s<60 and s>49    ② s>50 and s<59    ③ s>50 or s<59    ④ s>=50 or s<=59
```

```
15 <= age < 65的 if 結構條件式應如何撰寫？

① if (15 < age < 65) :   
② if (age >= 15 and age < 65) :   
③ if (age >= 15 or age < 65) :  
④ if (age >= 15; age < 65) :

```

```
優待票的年齡age，低於15或65以上的歲數，其條件式的寫法為何？

① age < 15 or age >= 65
② age < 15 and age >= 65
③ age >= 15 or age < 65
④ age >= 15 and age < 65
```

```
執行下列程式區段，a值的結果為何？

a=8
b=0
if (a >= 6) : b = 9
if (b < 6) : a =-2

① 9    ② 6    ③ 8    ④ -2
```

```
下列何者不是Python選擇結構的敘述？
① if   ② if  else    ③ if  elif  else    ④ switch
```

```
試寫出下列運算式的比較結果？
① 12 > 12
② 20+12 == 40-8
③ 45 != 45
# 大於,小於要相同資料類型比對
# 等於可以不同資料類型,str > int
④ '30' < 60 
⑤ '0' == 48
⑥ 'A' == 65
```