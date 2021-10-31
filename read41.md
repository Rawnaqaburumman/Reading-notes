# A beginner's guide to Big O Notation:

## What is a Big O Notation:
Is used in Computer Science to describe the performance or complexity of an algorithm,like:
- the execution time required
- the space used (e.g. in memory or on disk)


## Big O Notation types:
![Big 0 Notion](https://images.squarespace-cdn.com/content/v1/5acbdd3a25bf024c12f4c8b4/1599000012698-NJEGM0BCGG5ZKGIWC1GU/Big%2BO%2BNotation%2BSummary%2B%281%29.jpg)


# Examples:
### O(1)
```  bool IsFirstElementNull(IList<String> elements)
 
{
    return elements[0] == null;
}
```

### O(2^N)
``` int Fibonacci(int number)
{
    if (number <= 1) return number;
       
    return Fibonacci(number - 2) + Fibonacci(number - 1); 
}

```


Refeences:
<a href="A beginner's guide to Big O Notation">https://rob-bell.net/2009/06/a-beginners-guide-to-big-o-notation</a>
