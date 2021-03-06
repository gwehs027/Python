### 儲存資料的方式：
```
Python的資料儲存容器，可以分為tuple、串列(list)、字典(dict)與集合(set)四種，每一種結構都有其適合使用的情況與使用限制。
tuple用於依序儲存資料，可以依照順序取出資料，但不能更改，是不可變的物件；
串列(list)也是用於依序儲存資料，可以依照順序取出，也可以更改。
字典(dict)儲存的資料為「鍵(key)」與「值(value)」對應的資料，使用「鍵」查詢「值」。取出字典所有資料後，發現與建構字典時輸入資料的順序不同，字典儲存資料是沒有順序性的，字典也可視為關聯性陣列(associative array)。
集合(set)儲存沒有順序性的資料，要找出資料是否存在，儲存不需要鍵與值對應的資料，就很適合使用集合。
```

### tuple使用方式
```
例1：
t1 = ()
print(t1)

例2：
t2 = 1, 2 ,3
print(t2)

例3
t3 = (1, 2, 3)
print(t3)

例4
t3 = (1, 2, 3)
print(t3[0])

例5
t3 = (1, 2, 3)
a, b, c= t3
print('a=', a, ',b=', b, ',c=', c)

例6
a = 10
b = 20
print('交換前','a=', a, ',b=', b)
a, b = b, a
print('交換後','a=', a, ',b=', b)

例7
t4 = (1,2,3,4)
t5 = (t4,5,6)
print(t5)
print(len(t5))
print(t5[0][0])

例8
t6 = ('z', )
print(t6)

Q1:
a =  10,b = 20
如何將a和b的值互換？

```

### 串列的使用
```
串列為可修改的序列資料，可以修改元素資料、新增、刪除、插入與取出元素，使用list函式可以將資料轉換成串列，並可以使用[::]取出串列的一部分。
使用「[]」建立新的串列。

例1
shoplist1 = ['牛奶', '蛋', '咖啡豆', '西瓜', '鳳梨']
print('購物清單shoplist1為')
print(shoplist1)

例2
shoplist2 = ['牛奶', '蛋', '咖啡豆', '西瓜', '鳳梨']
print('顯示shoplist2[0]為',shoplist2[0])

例3
shoplist3 = ['牛奶', '蛋', '咖啡豆', '西瓜', '鳳梨']
print('購物清單shoplist3的長度為', len(shoplist3))

例4
shoplist = ['牛奶', '蛋', '咖啡豆', '西瓜', '鳳梨']
shoplist[1] = '皮蛋'
print("執行 shoplist[1] = '皮蛋' 後")
print(shoplist)

例5
shoplist1 = ['牛奶', '蛋', '咖啡豆']
shoplist2 = ['西瓜', '鳳梨']
shoplist_all = shoplist1 + shoplist2
print(shoplist_all)

例6
list1 = list('python')
print(list1)
tuple2 = ('a', 'b', 1, 2)
list2 = list(tuple2)
print(list2)



```
