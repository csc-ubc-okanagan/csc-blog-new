---
title: Dictionaries in Python
author: ["Madison"]
date: 2023-06-15 09:00:00 -0800
categories: ["Python", "P_Getting Started"]
tags: ["python"] # tags always lowercase
---



A dictionary lists key-value pairs, which could also be thought of as associated values where a key matches to the associated value. Let's look at a few examples.


``` python
# Dictionary - mapping between values
house = {'bedrooms': 3, 'bathrooms': 2, 
         'city': 'Kelowna', 'price': 250000}
```



``` python
house['price']
```

```
## 250000
```



``` python
course = {'Data Science': ['DATA100', 'DATA200', 'DATA300'],
            'Science': ['SCIENCE100', 'SCIENCE200', 'SCIENCE300']}
```



``` python
course['Data Science']
```

```
## ['DATA100', 'DATA200', 'DATA300']
```

What if we wanted to turn the following information into a dictionary. 

Name | ID | Campus | Courses
:--- | :--- | :--- | :---
Dan | 12345678 | Okanagan | DATA100, ENGL100, HIST100, CHEM100

This is how we would do this:


```{.python .fold-hide}
student = {'Name' : 'Dan',
            'ID' : 12345678,
            'Campus' : 'Okanagan',
            'Courses': ['DATA100', 'ENGL100', 'HIST100', 'CHEM100']}
student
```

```
## {'Name': 'Dan', 'ID': 12345678, 'Campus': 'Okanagan', 'Courses': ['DATA100', 'ENGL100', 'HIST100', 'CHEM100']}
```

