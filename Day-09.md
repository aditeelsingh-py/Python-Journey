  # List vs Tuple
  ^mutable  ^immutable
  ^more memory  ^less memory
  ^insertion deletion easy  ^accessing elements is easy
  ^traversing is time consuming  ^not time consuming

  # DEEP COPY and SHALLOW COPY
  import copy
  original=[[1,2],[3,4]]
  deepcopy=copy.deepcopy(original)
  deepcopy[0][0]=99
  print("original",original)
  print("deepcopy",deepcopy)

  # SHALLOW COPY

  import copy
  original=[[1,2],[3,4]]
  shallow_copy=copy.copy(original)
  shallow_copy[0][0]=99
  print("original",original)
  print("copy",shallow_copy)

  # type of sorting in python
  *Tim sort algorithm
  *hybrid sorting algorithm -> merge sort + insertion sort
  *worst complexity = o(NlogN)
  # DECORATORS
  # Remove duplicate elements
str=[1,2,3,4,5,5,4]
l=[]
for i in str:
    if i not in l:
        l.append(i)
print(l)

OUTPUT- [1, 2, 3, 4, 5]
# group words by length
str="he is superman"
words=str.split()
d={}
for in range(len(words)):
 length=len(words[i])
 if length not in d:
  d[length]=[]
  d[length].append(words[i])
print(d)
OUTPUT- {2: ['he', 'is'], 8: ['superman', 'abcdefgh']}
  
  
