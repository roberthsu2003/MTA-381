# 執行輸入與輸出操作
## (20-25)%

### New

```
1下列為簡單的檔案操作程式，程式的功能如下：
• 檢查檔案test45.txt是否存在？
• 如果檔案存在，則顯示檔案內容。
• 如果檔案不存在，就新增test45.txt檔案。 • 在檔案結尾加上 "end" 字串。

請回答以下問題來完成程式。
01 import os
02 if ____________________________________:
03     file = open('test45.txt')
04     _________________________________________
05     file.close()
06 file = ______________________________________
07 ___________________________________('end')
08 file.close()

A：請問第2行應該填入下列哪段指令？
① isfile('test45.txt')
② path.isfile('test45.txt')
③ os.exist('test45.txt')
④ os.path.isfile('test45.txt')
 
B：請問第4行應該填入下列哪段敘述？
① print('test45.txt')
② output('test45.txt')
③ print(file.read())
④ print(file.get('test45.txt'))

C：請問第6行應該填入下列哪段指令？
① open('test45.txt', 'a')
② open('test45.txt', 'a+')
③ open('test45.txt', 'w')
④ open('test45.txt', 'w+')

D：請問第7行應該填入下列哪段敘述？
① Append     ② os.file.add     ③ file.write    ④ os.write

_________________________
import os
if os.path.isfile('test45.txt'):
    file = open('test45.txt')
    print(file.read())
    file.close()

file = open('test45.txt', 'a+')
file.write('end')
file.close()

A:④
B:③ 
C:②
D:③

```

```
2請利用下列敘述區段的代碼，組合成一個讀取檔案第一行內容的函式

• 如果檔案存在，就傳回檔案的第一行內容。
• 如果檔案不存在，則傳回'檔案不存在'。

01 import os
02 def read_line(fileName):
03     _____________________________ 
04     _____________________________
05     _____________________________ 06     _____________________________
07     _____________________________

①    with open(fileName, 'r') as f:
②    return '檔案不存在'
③    return f.readline()
④ if os.path.isfile(fileName):
⑤ else:

A：第3行應該填入何者？
B：第4行應該填入何者？ C：第5行應該填入何者？
D：第6行應該填入何者？ E：第7行應該填入何者？

_______________________
import os
def read_line(fileName):
	if os.path.isfile(fileName):
		with open(fileName, 'r') as f:
			return f.readline()
	else:
		return '檔案不存在'
			
A:④
B:①
C:③
D:⑤
E:②
```

```
3要將資料讀寫到文字檔test47.txt中，如果該檔案已有內容就刪除內容；如果檔案不存在就新增。
此時，應該使用下列哪個敘述？

① open('test47.txt', "w+")
② open('test47.txt', "r+")
③ open('test47.txt', "w")
④ open('test47.txt', "r")

_________________________
w -> 打开一个文件只用于写入。如果该文件已存在则打开文件，并从开头开始编辑，即原有内容会被删除。如果该文件不存在，创建新文件。

r -> 以只读方式打开文件。文件的指针将会放在文件的开头。这是默认模式。

w+ -> 打开一个文件用于读写。如果该文件已存在则打开文件，并从开头开始编辑，即原有内容会被删除。如果该文件不存在，创建新文件。

r+ -> 打开一个文件用于读写。文件指针将会放在文件的开头。
①
```



```
4設計一個可以讀取資料庫檔案的程式，功能必須符合下列條件：

• 檔案包含貨品編號、成品、售價、數量等資料，例如A001, 123, 160, 50。
• 檔案中的每一行都要讀取和顯示。
• 如果讀到空行則忽略不處理。
• 完成所有行的讀取後，顯示結束訊息並關閉檔案。

請問下列程式碼的第5、6行，應該使用下列哪兩個敘述？

01 f = open("test48.txt", 'r')
02 eof = False
03 while eof == False:
04     data = f.readline()
05     ______________________________
06        ______________________________
07          print(data.strip())
08     else:
09        eof = True
10        print("結束")
11 f.close()

① if data != '':
	if data != '\n':
	
② if data != '\n': 
      if data != '': 
      
③ if data == '':
	if data == '\n':
	
④ if data == '\n':
	if data == '':

____________________________________
f = open("test48.txt", 'r')
eof = False
while eof == False:
     data = f.readline()
     if data != '':
        if data != '\n':
	         print(data.strip())
     else:
        eof = True
        print("結束")
f.close()


①
```

```
5下列為計算平均分數的程式碼，程式功能如下:
• 可以接受任意筆輸入的含小數分數。
• 結束輸入分數後，就顯示平均分數，分數要四捨五入到小數第二位。

請回答以下問題來完成程式：

01 sum, num = 0, 0
02 avg = 0.0
03 while (num != -1):
04     score = _____________________________
05     if score == -1:
06          break
07     sum += score
08     num += 1
09 avg = float(sum / num)
10 __________B__________ + _________C__________

A：請問第4行應該填入下列哪段指令？
① float(input('請輸入成績(0 ~ 100)，停止時請輸入0：') )
② float(input('請輸入成績(0 ~ 100)，停止時請輸入-1：') )
③ input('請輸入成績(0 ~ 100)，停止時請輸入0：') ④ input('請輸入成績(0 ~ 100)，停止時請輸入-1：')

B：請問第10行的B應該填入下列哪段敘述？
① input('平均成績： '
② output('平均成績： '
③ printline('平均成績： '
④ print('平均成績： '

C：請問第10行的C應該填入下列哪段敘述？
① format(avg, '.2f'))
② format(avg, '.2d'))
③ avg.format('.2d'))
④ format.avg('.2f'))

_________________________

sum, num = 0, 0
avg = 0.0
while (num != -1):
    score = float(input('請輸入成績(0 ~ 100)，停止時請輸入-1：') )
    if score == -1:
       break
     sum += score
     num += 1
avg = float(sum / num)
print('平均成績： ' + format(avg, '.2f'))

A:②
B:④ 
C:①               
```

```
6請問下列程式碼的執行結果為何？

01 import datetime
02 d = datetime.datetime(2002, 4, 1)
03 print('{:%B-%d-%y}'.format(d))
04 n = 123456.789
05 print('{:,.4f}'.format(n))

① 01-04-2002
   123,456.7890

② 04-01-02
   123,456.789

③ April-01-2002
   123,456.7890
   
④ January-04-02
   123456.789
   
_______________________
③
```

```
7.下列為計算平均分數的程式碼，程式功能如下：

• 可以接受輸入的使用者姓名。
• 可以接受任意筆輸入的整數分數，輸入-1可以結束程式並顯示訊息。
• 顯示姓名時會靠左對齊，當姓名少於10個字元會保留空格。
• 顯示平均分數時，要在小數點左邊保留三個位置，小數點右邊保留一個位置。

01 name = input("請輸入姓名：")
02 score, num ,sum = 0, 0, 0
03 while (score != -1):
04      score = int(input("請輸入成績：(停止時請輸入-1)"))
05      if score == -1:
06           break
07      sum += score
08      num += 1
09      avg = sum / num
10 print("______A_______：平均分數 =_______B_________"%(name, avg))

A：請問第10行的A應該填入下列哪段指令?
① %10f      ② %10s     ③ %-10f      ④ %-10s

B：請問第10行的B應該填入下列哪段指令？
① %3.1f     ② %5.1f     ③ %1.3f     ④ %1.5f     

______________________________
name = input("請輸入姓名：")
score, num ,sum = 0, 0, 0
while (score != -1):
   score = int(input("請輸入成績：(停止時請輸入-1)"))
     if score == -1:
          break
     sum += score
     num += 1
     avg = sum / num
print("%-10s：平均分數 = %5.1f"%(name, avg))

A:④
B:②
```

```
8下列為讀取資料檔並將結果依照格式列印的函式，函式的功能如下

• 資料檔中包含貨品的相關資訊，每筆記錄有品名、成本和售價。
	例如：修護霜,7.5,10.25。
• 列印輸出時品名要佔 10 個空格範圍，並且文字靠左對齊。
• 成本要佔 5 個空格範圍並靠右對齊，小數點後最多只留一個位數。
• 價格要佔 7 個空格範圍並靠右對齊，小數點後最多只留兩個位數。

請利用下列指令的代碼(可省略或重複使用)，組合完成第5行敘述？

01 def print_data(data_file):
02     f = open(data_file,'r')
03     for datas in f:
04         d = datas.split(",")
05         __________________".format(d[0], eval(d[1]), eval(d[2])))


①print(" 
    
②{10: 0} 
     
③{5:1f}  
    
④{7:2f} 
     
⑤{2:7.2f}  
    
⑥{1:5.1f} 
     
⑦{0:10}

_____________________
def print_data(data_file):
    f = open(data_file,'r')
    for datas in f:
        d = datas.split(",")
        print("{0:10}{1:5.1f}{2:7.2f}".format(d[0], eval(d[1]), eval(d[2])))

① ⑦ ⑥ ⑤
```

```
9下列為接受使用者輸入的資料，並依照格式列印的程式碼，顯示的格式如下：

• 姓名前後必須用雙引號括住。
• 分數直接顯示不用引號或其他字元括住。
• 姓名和分數之間用逗號隔開。

請問第3行填入下列哪些敘述，可以符合上面的顯示格式？(複選)

01 name = input("請輸入姓名：")
02 score = input("請輸入分數：")
03 __________________________

① print('"{0}",{1}'.format(name, score)) ② print('"%s",%s' % (name, score))  ③ print('"' + name + '",' + score)  ④ print(name + ',' + score)、 ⑤ print("{0},{1}".format(name, score))

______________________
name = input("請輸入姓名：")
score = input("請輸入分數：")
print('"{0}",{1}'.format(name, score))
print('"%s",%s' % (name, score))
print('"' + name + '",' + score) 
① ② ③
```

```
10下列為接受使用者輸入的資料，並顯示的程式碼。
請問第2行要填入下列哪個敘述，才能完成程式的功能？

01 print("請輸入最喜歡的水果：")
02 _________________________
03 print(fruit)

① fruit = input()
② fruit = input
③ input(fruit)	
④ input("fruit ")

_____________________
print("請輸入最喜歡的水果：")
fruit = input()
print(fruit)

①
```
### old

1 建構並分析執行檔案輸入與輸出操作的程式碼區段  

	- 陳述式的打開；關閉；讀取；寫入；附加；檢查是否存在以及刪除
	
2 建構並分析執行主控臺輸入與輸出操作的程式碼區段
	
	- 從主控臺讀取輸入；列印格式化文字；使用指令行引數
	
```
請問input()函式執行後，使用者所輸入的整數資料，會以下列哪種資料型別傳回?

① bool     ② float     ③ int     ④ str  

```

```
將字串資料寫入檔案，可使用哪一個函式？

① read()      ② flush()      ③ write()      ④ print()

```

```
將一行字串由檔案讀出，可使用哪一個方法？

① readline()
② flush()
③ read()
④ write()

```

```
哪一個函式是用來開啟檔案？

① open()
② close()
③ input()
④ output()

```

```
欲讀取檔案內容，要使用何種模式開檔？

① w      ② r      ③ a      ④ c

```

```
執行下列程式片段，其結果如何？
x = 120
try:
	print(x, end = '  ')
except:
	x = x + 50
	print(x, end = '  ')
finally:
	print(x, end = '  ')

① 120  120      ② 120      ③ 170      ④ 120  170
```
