---
title: "Reading Data in Python"
author: ["Madison"]
date: 2023-06-05 11:00:00 -0800
categories: ["Python", "P_Data"]
tags: ["python", "data"]
---

    


## CSV File

Using the Pandas library, it is very easy to open a CSV file using Python. Simply import the package, and then use the line `pd.read_csv()`. See this example below:


``` python
import pandas as pd
df = pd.read_csv("file.csv")
```


Note that this assumes the file you want to open follows the same filepath as your current directory. If you wanted to use a file in a different directory, simply use `pd.read_csv("/Users/name/rest_of_filepath/file.csv")` instead.

Alternatively, if you were to use base Python, it gets a bit more complicated. Using the CSV library, it would have to be done by iterating through each row in the file. Printing each row would look like this:


``` python
import csv
with open("file.csv", 'r') as file:
  csvreader = csv.reader(file)
  for row in csvreader:
    print(row)
```

```
## ['12\t12']
## ['34\t1']
## ['1\t1']
## ['1\t1']
## ['1\t1']
```

## Text File

Similarly, for a text file, we can use Pandas to simplify the process. We can use the line `pd.read_fwf()` to read in a `.txt` file. For reference, FWF stands for fixed width lines which allows the lengths and features of the file to be specified as fixed values so that it can be read in to Python systematically. See this example below:


``` python
import pandas as pd
df = pd.read_fwf('file.txt')
```


Alternatively, you can also iterate through each row similar to the csv format mentioned above, but we will not go through that. If you would like to try it as an exercise, simply use the second method above in the CSV section and change the file formatting to fit a `.txt` file.

## URL

You can also access data on the internet without having to save a local copy. Take this website for example: [Gapminder Data](https://raw.githubusercontent.com/jstaf/gapminder/master/gapminder/gapminder.csv)

If you follow the link, you will see that it is simply a CSV file with no other formatting or permissions to enter. If we wanted to read this into our Python script, we could do it like this:


``` python
import pandas as pd
url = 'https://raw.githubusercontent.com/jstaf/gapminder/master/gapminder/gapminder.csv'
df = pd.read_csv(url)
```


There are many other file formats and ways to load files into Python. There are great resources online for any other file formats, but these examples above should get you started.
