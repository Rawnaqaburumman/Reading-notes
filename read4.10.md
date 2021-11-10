# Stacks and Queues
# What is a Stack
- A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.

- Stacks follow these concepts:
## FILO
- First In Last Out:
his means that the first item added in the stack will be the last item popped out of the stack.

## LIFO
Last In First Out

This means that the last item added to the stack will be the first item popped out of the stack.

## Stack Visualization
#### Push O(1)
- Pushing a Node onto a stack will always be an O(1) operation. This is because it takes the same amount of time no matter how many Nodes (n) you have in the stack.
![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/pushStack1.PNG)
- Next, you need to assign the next property of Node 5 to reference the same Node that top is referencing: Node 4
![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/pushStack2.PNG)

- Technically at this point, your new Node is added to your stack, but there is no indication that it is the first Node in the stack. To make this happen, you have to re-assign our reference top to the newly added Node, Node 5.
- ![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/pushStack3.PNG)


## Pop O(1)
Popping a Node off a stack is the action of removing a Node from the top. When conducting a pop, the top Node will be re-assigned to the Node that lives below and the top Node is returned to the user.

## Peek O(1)
When conducting a peek, you will only be inspecting the front Node of the queue.
#### Queues
Typically, you want to check isEmpty before conducting a peek. This will ensure that an exception is not raised. Alternately, you can wrap the call in a try/catch block.
A Queue is a linear structure which follows a particular order in which the operations are performed. The order is First In First Out (FIFO). A good example of a queue is any queue of consumers for a resource where the consumer that came first is served first. The difference between stacks and queues is in removing. In a stack we remove the item the most recently added; in a queue, we remove the item the least recently added.

### ![](https://media.geeksforgeeks.org/wp-content/cdn-uploads/gq/2014/02/Queue.png)
