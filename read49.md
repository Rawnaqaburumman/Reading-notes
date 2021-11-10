# Dunder or magic methods in Python

Dunder or magic methods in Python are the methods having two prefix and suffix underscores in the method name. Dunder here means “Double Under (Underscores)”. These are commonly used for operator overloading. Few examples for magic methods are: __ init __ , __ add __ , __ len __, __ repr __ etc.

The __ init __ method for initialization is invoked without any call, when an instance of a class is created, like constructors in certain other programming languages such as C++, Java, C#, PHP etc. These methods are the reason we can add two strings with ‘+’ operator without any explicit typecasting.

Here’s a simple implementation :

```
# declare our own string class
class String:
      
    # magic method to initiate object
    def __init__(self, string):
        self.string = string
          
# Driver Code
if __name__ == '__main__':
      
    # object creation
    string1 = String('Hello')
  
    # print object location
    print(string1)
```
## Revisiting the normal

The normal distribution is significant to probability and statistics thanks to two factors: the Central Limit Theorem and the Three Sigma Rule.

## Central Limit Theorem

In the previous section, we demonstrated that if we repeated our 10-toss trials many, many times, the average heads-count of all of these trials will approach the 50% we expect from an ideal coin. With more trials, the closer the average of these trials approach the true probability, even if the individual trials themselves are imperfect. This idea is a key tenet of the Central Limit Theorem. In our coin-tossing example, a single trial of 10 throws produces a single estimate of what probability suggests should happen (5 heads). We call it an estimate because we know that it won’t be perfect (i.e. we won’t get 5 heads every time).

If we make many estimates, the Central Limit Theorem dictates that the distribution of these estimates will look like a normal distribution. The zenith of this distribution will line up with the true value that the estimates should take on. In statistics, the peak of the normal distribution lines up with the mean, and that’s exactly what we observed. Thus, given multiple “trials” as our data, the Central Limit Theorem suggests that we can hone in on the theoretical ideal given by probability, even when we don’t know the true probability. Central Limit Theorem lets us know that the average of many trials means will approach the true mean, the Three Sigma Rule will tell us how much the data will be spread out around this mean.
## Iteration: `__len__, __getitem__, __reversed__`

In order to iterate over our account object I need to add some transactions. So first, I’ll define a simple method to add transactions. I’ll keep it simple because this is just setup code to explain dunder methods, and not a production-ready accounting system

## Operator Overloading for Comparing Accounts: `__eq__, __lt__`

## Operator Overloading for Merging Accounts: `__add__` 

In Python, everything is an object. We are completely fine adding two integers or two strings with the + (plus) operator.

## Callable Python Objects: `__call__`
You can make an object callable like a regular function by adding the `__call__` dunder method. For our account class we could print a nice report of all the transactions that make up its balance

## Context Manager Support and the With Statement: `__enter__, __exit__`

A context manager is a simple “protocol” (or interface) that your object needs to follow so it can be used with the with statement. Basically all you need to do is add `__enter__` and `__exit__` methods to an object if you want it to function as a context manager.


## Z-score
The Z-score is a simple calculation that answers the question, “Given a data point, how many standard deviations is it away from the mean?” The equation below is the Z-score equation. Z-score

![5](https://i.imgur.com/3TuDF4G.jpg)

By itself, the Z-score doesn’t provide much information to you. It gains the most value when compared against a Z-table, which tabulates the cumulative probability of a standard normal distribution up until a given Z-score. A standard normal is a normal distribution with a mean of 0 and a standard deviation of 1. The Z-score lets us reference this the Z-table even if our normal distribution is not standard. The cumulative probability is the sum of the probabilities of all values occurring, up until a given point.

An easy example is the mean itself. The mean is the exact middle of the normal distribution, so we know that the sum of all probabilites of getting values from the left side up until the mean is 50%. The values from the Three Sigma Rule actually come up if you try to calculate the cumulative probability between standard deviations. The picture below provides a visualization of the cumulative probability.
