# Python note

# 

---

群集資料型態

len\( \) 以一個int物件傳回資料項的長度

```python
len((“one”,))
```

1

```python
len(“one”)
```

3

```python
len("automatically”)
```

13

list型態 有個append\(\)方法，可以將一個物件附加至一個清單

就像這樣：

```python
x = ["zebra",49,-897,"arrvark",200]
x.append("more")
x
```

\['zebra', 49, -897, 'arrvark', 200, 'more’\]

list型態 有 insert\(\) 用於將一個資料項插入被給定的索引位置

還有 remove\(\) 用於從被給定的索引位置移除一個資料項

python 的 索引是從 0 開始

```python
x
```

\['zebra', 49, -897, 'arrvark', 200, 'more’\]

```python
x[1]
```

49

```python
x[1] = "forty nine"
x
```

\['zebra', 'forty nine', -897, 'arrvark', 200, 'more’\]

---

雖然a與b是不同的物件\(具有不同的身份\)，但他們有相同的值，

所以他們是相等的。

```python
a = "many paths"
b = "many paths"
a is b
```

False

```python
a == b
```

True

隸屬運算符

對於序列或群集之類的資料型態，像是字串、清單和位元組，我們可以使使用 in 運算元來測試隸屬關係，使用 not in 來測試無隸屬關係：

```python
 P = (4,"frog",9,-33,9,2)
 2 in P
```

True

```python
phrase = "wild SWans by Jung Chang"
"J" in phrase
```

True

---

邏輯運算符

短路表達式x AND y，事實上等價於條件語句：if x then y else false。短路表達式x OR y，則等價於條件語句：if x then true else y。

```python
five = 5
two = 2
zero = 0
five and two
```

2

```python
two and five
```

5

```python
five and zero
```

0

```python
five or two
```

5

```python
two or five
```

2

```python
zero or five
```

5

```python
5 | 3
```

7

```python
2&1
```

0

---

if 陳述句

與其他語言不同的是Python使用縮排來表示它的區塊結構。

```py
if lines <1000:
    print\("small"\)
elif lines <10000:
    print\("medium"\)
else:
    print("large")
```

---

for...in陳述句

```py
>>>for country in ["Denmark","Finland","Norway","Sweden"]:
       print\(country\)
```

Denmark

Finland

Norway

Sweden

```py
>>> for letter in "ABCDEFGHIJKLMNOPQRSTUVWXYZ":    

       if letter in "AEIOU":

           print\(letter,"is vowel"\)

      else:

          print\(letter,"is a consonant"\)
```

A is vowel

B is a consonant

C is a consonant

D is a consonant

E is vowel

F is a consonant

G is a consonant

H is a consonant

I is vowel

J is a consonant

K is a consonant

L is a consonant

M is a consonant

N is a consonant

O is vowel

P is a consonant

Q is a consonant

R is a consonant

S is a consonant

T is a consonant

U is vowel

V is a consonant

W is a consonant

X is a consonant

Y is a consonant

Z is a consonant

---

函式的建立與呼叫

```py
    def get_int(msg):
        while True:
            try:
                i=int\(input\(msg\)\)
        return i
        except ValueError as err:
            print\(err\)
```

```python
get_int(3)
```

3

```python
get_int(q)
```

invalid literal for int\(\) with base 10: 'get\_int\(q\)’



計算成績

```python
grades = [100, 100, 90, 40, 80, 100, 85, 70, 90, 65, 90, 85, 50.5]
def grades_sum(scores):
    total = 0
    for score in scores:
        total += score
    print total
    return total
grades_sum(grades)
```



