## 파이썬 itertools

### from itertools import ...으로 사용됨

data = ['A', 'B', 'C']<br/>
r = 2

## 1. 순열: permutations

math.factorial(len(data)) / math.factorial(len(data)-r)

자기자신 X, 순서 O, 중복 O

['A', 'B']<br/>
['A', 'C']<br/>
['B', 'A']<br/>
['B', 'C']<br/>
['C', 'A']<br/>
['C', 'B']<br/>

## 2. 조합: combinations

math.factorial(len(data)) / math.factorial(len(data)-r) \* math.factorial(r)

자기자신 X, 순서 X, 중복 X

['A', 'B']<br/>
['A', 'C']<br/>
['B', 'C']<br/>

## 3. 중복 순열: product

len(data)\*\*r

자기자신 O, 순서 O, 중복 O

['A', 'A']<br/>
['A', 'B']<br/>
['A', 'C']<br/>
['B', 'A']<br/>
['B', 'B']<br/>
['B', 'C']<br/>
['C', 'A']<br/>
['C', 'B']<br/>
['C', 'C']<br/>
