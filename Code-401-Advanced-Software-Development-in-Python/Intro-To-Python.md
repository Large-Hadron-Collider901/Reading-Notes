# Introduction To Python

## Beginner's Guide To Big O Notation

* Big O Notation describes the performance or complexity of an algorithm
* It can also be used to describe the execution time required or the space used (in memory or on disk) by an algorithm

### Common Orders Of Growth:

**O(1)** - algorithms that will always execute in the same time or space regardless of the size of the input data set.

**O(N)** - describes an algorithm whose whose performance will grow linearly and in direct proportion to the size of the data set.

**O(N<sup>2</sup>)** - represents an algorithm whose performance is directly proportional to the square of the size of the input data set. 

**O(2^N)** - denotes an algorithm whose growth doubles with each addition to the input data set. These algorithms have an exponential growth curve.

**O(log N)/Logarithms** - describes an algorithm that compares the middle element of a data set (median) against a target value, if the values match, it will return a success. If the target value is higher than the value of the probe element, it will take the upper half of the data set and perform the same operation against it. Likewise, if the target value is lower than the value of the probe element, it will perform the operation against the lower half. It will continue to halve the data set with each iteration until the value has been found or until it can no longer split the data set.

## Names And Values in Python
* Names refer to values - Example: `x = 23` `print(x)` `# 23`
* Many names can refer to one value - Example: `x = 23` `y = x`
* Names are reassigned independently - Example: `x = 23` `y = x` `x = 12` 


*reading sources*: [Beginners-guide-to-Big-O-Notation](https://rob-bell.net/2009/06/a-beginners-guide-to-big-o-notation)

[A-friendly-intro-to-Big-O-Notation](https://www.codenewbie.org/basecs/8)

[Facts-and-Myths-about-Python-names-and-values ](https://www.youtube.com/watch?v=_AEJHKGk9ns)

[How-to-Setup-an-Awesome-Python-Environment-for-Data-Science-or-Anything-Else](https://towardsdatascience.com/how-to-setup-an-awesome-python-environment-for-data-science-or-anything-else-35d358cc95d5)

[Python-3-Module-of-the-Week](https://pymotw.com/3/index.html)