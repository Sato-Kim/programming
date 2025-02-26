# ループ

## 準備

1. [Google Colaboratory](https://research.google.com/colaboratory/)で「Python 3の新しいノートブック」を作る．
1. ノートブックの名前を「07」に変える．

## 演習

**問題** 単純なループ

```python
for i in range(10):
  print("Hello, World!")
```

**問題** リストに対するループ

```python
fruits = ['Apple', 'Orange', 'Grape']
for f in fruits:
  print(f)
```

**問題** タプルとセットで上と同様のことを試せ。

**問題** 辞書に対するループ

```python
dic = {'A':100, 'B':200, 'C':300}
for k in dic:
  print(k)
```

**問題** ループによるコンテナの変更

```python
# 準備
fruits = ['Apple', 'Orange', 'Grape']
for i, f in enumerate(fruits):
  print(i, f)
```

```python
fruits = ['Apple', 'Orange', 'Grape']
for i, f in enumerate(fruits):
  fruits[i] = f.upper()

print(fruits)
```

```python
# ダメな例
fruits = ['Apple', 'Orange', 'Grape']
for i, f in enumerate(fruits):
  f = f.upper()

print(fruits)
```

**問題** rangeの利用

```python
# 準備
fruits = ['Apple', 'Orange', 'Grape']
for i in range(len(fruits)):
  print(i)
```

```python
fruits = ['Apple', 'Orange', 'Grape']
for i in range(len(fruits)):
  fruits[i] = fruits[i].upper()

print(fruits)
```

**問題** While

```python
i = 10
while i > 0:
  print(i)
  i -= 1
print('Happy New Year!')
```

**問題** forでの書き換え

```python
for i in (range(10, 0, -1)):
  print(i)
print('Happy New Year!')
```
**問題** breakとcontinue

```python
for i in range(10):
  if i == 5:
    break
  print(i)
```

```python
for i in range(10):
  if i == 5:
    continue
  print(i)
```

**問題** 入れ子のループ

```python
for i in range(1, 3):
  print(i)
  for ch in ['a', 'b', 'c']:
    print(f'  {ch}')
```

**問題** `[10, 20, 30, 20, 10, 10, 20]`というリストにおける，個々の数値とその出現回数を調べよ．

**問題（レポート課題）** 前問を[Counter](https://docs.python.org/ja/3/library/collections.html#collections.Counter)を使って解決せよ．

**問題（レポート課題）** 前問を[defaultdict](https://docs.python.org/ja/3/library/collections.html#collections.defaultdict)を使って解決せよ．
