# 問題排解和錯誤處理
```
如果test61.txt檔案不存在，請評估下列程式碼執行的情形？

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

```

```
下列程式碼是計算num連除遞增整數的值，請問執行的結果為何？

① 第05 行敘述會造成無窮迴圈程式不會終止。
② 第05 行敘述有語法錯誤，應該改為while(ok == True): ③ 第07 行敘述會因為除數為零，而造成執行階段錯誤。
④ 第08 行敘述有語法錯誤，應該改為i = i + 1。


```