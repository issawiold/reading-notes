Stacks
======

a stack is a data type where the data you place last is the data that you can take first , when a stack is mentioned the first thing that comes to mind is a stack of files 

![file stack](https://previews.123rf.com/images/olegdudko/olegdudko1807/olegdudko180703294/104626219-stack-of-documents-files.jpg)

the first data added to the stack will be at the very bottom and will be taken out last while the data placed at the top will be taken first or lifo last in first out

we can do that by placing a pointer at the very last element of add to an array or any other type where each time a new element is add the pointer would move to that element  (push) and we remove an element by moving the element before the one it's pointing at now(pop)

==================================================

Queues
======

on the other hand Queues are very similar to queues in real life , when you stand in a queue waiting for your turn where the first person in the queue is the first out 

![a queue of people](https://img.freepik.com/free-vector/queue-people-icon-set-with-different-people-waiting-line-atm-illustration_1284-29300.jpg?w=2000)

 the first data added to the data structure would be the first to be processed and leave while the data add at the last would have to wait for all the data added before it's turn .

we can do that by placing two pointers one at the very start of the queue in the data type we want to use the other is at the very end

everytime we are done processing data at the front we move the pointer at the front to the next element (dequeue) and every time we add an element we move the pointer at the back to the newly added element (enqueue).