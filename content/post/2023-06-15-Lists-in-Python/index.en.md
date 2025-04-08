---
title: "Lists in Python"
author: ["Madison"]
date: 2023-06-15 09:00:00 -0800
categories: ["Python", "P_Getting Started"]
tags: ["python"] # tags always lowercase
---




Lists are an important tool used in Python. Lists can contain elements of mixed types as well. Let's look at a few examples.


``` python
# List
list1 = []
list1
```

```
## []
```


``` python
list2 = [1, 'UBC', 100]
list2
```

```
## [1, 'UBC', 100]
```

Now let's see a few operations we can perform on a list.


``` python
len(list1)
```

```
## 0
```


``` python
len(list2)
```

```
## 3
```


``` python
# Indexing Example - we will talk more about this later on
list2[2]
```

```
## 100
```
Note - Python indexing starts at zero, so the first element in the list is 0, the second is 1, and the third is 2, so if we actually wanted the second element, we would have to do this:


``` python
list2[1]
```

```
## 'UBC'
```


``` python
type(list2)
```

```
## <class 'list'>
```


``` python
type(list2[1])
```

```
## <class 'str'>
```


As we mentioned earlier, a main difference between lists and tuples is that lists are mutable. Mutable means that elements in a list can be appended, changed, or deleted. 


``` python
mixed_list = [1, 'UBC', 5.0, '1']
mixed_list.append('New')
mixed_list
```

```
## [1, 'UBC', 5.0, '1', 'New']
```
If we decided that we wanted to replace 'New' with 4, we could do so like this:


``` python
mixed_list[4]= 4
mixed_list
```

```
## [1, 'UBC', 5.0, '1', 4]
```
If we wanted to remove elements from the list, we could do so like this:


``` python
mixed_list.remove('UBC')
mixed_list
```

```
## [1, 5.0, '1', 4]
```

Note that this will only remove the first occurrence, if this happened to be in the list more than once. It would also call an error message if the element doesn't exist.

If we wanted to remove it based on the index of the list:


``` python
del mixed_list[0]
mixed_list
```

```
## [5.0, '1', 4]
```
