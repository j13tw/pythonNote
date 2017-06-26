# Python note

# 

---

H4len\( \) 以一個int物件傳回資料項的長度

&gt;&gt;&gt;len\(\(“one”,\)\)

1

&gt;&gt;&gt; len\(“one”\)

3

&gt;&gt;&gt; len\("automatically”\)

13

---

list型態 有個append\(\)方法，可以將一個物件附加至一個清單

就像這樣：

&gt;&gt;&gt; x = \["zebra",49,-897,"arrvark",200\]

&gt;&gt;&gt; x.append\("more"\)

&gt;&gt;&gt; x

\['zebra', 49, -897, 'arrvark', 200, 'more’\]

list型態 有 insert\(\) 用於將一個資料項插入被給定的索引位置

還有 remove\(\) 用於從被給定的索引位置移除一個資料項

python 的 索引是從 0 開始

&gt;&gt;&gt; x

\['zebra', 49, -897, 'arrvark', 200, 'more’\]

&gt;&gt;&gt; x\[1\]

49

&gt;&gt;&gt; x\[1\] = "forty nine"

&gt;&gt;&gt; x

\['zebra', 'forty nine', -897, 'arrvark', 200, 'more’\]

---



