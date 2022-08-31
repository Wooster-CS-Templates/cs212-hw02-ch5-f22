# Chapter 5 Homework Questions

**Name:** YOUR NAME HERE

Answer the questions below. When asked to create a process tree for an answer use the following markdown to represent it:

```textile
a
|_b
|_c
  |_d
```

The block syntax that the tree is contained in is important for the markdown to render correctly. Note how the text inside the block syntax uses the pipe character `|` ( types with`Shift + \`) and the underscore `_` to show the leaves and branches in the tree.


## Question 1

Run `$ python3 fork.py -s 10 -a 6 -F` and create the **final** process tree below that would result from the process actions listed.


```textile
ANSWER HERE
```


## Question 2

One control the simulator gives you is the fork percentage, controlled by the `-f` flag. The higher it is, the more likely the next action is a fork; the lower it is, the more likely the action is an exit. Run the simulator with a large number of actions (e.g., -a 100) and vary the fork percentage from 0.1 to 0.9. What do you think the resulting final process trees will look like as the percent- age changes? Verify your answer afterward by running fork.py with the  `-c` option.


ANSWER HERE


## Question 3

Run `$ python3 fork.py -s 44 -a 9 -f 0.3 -t`and provide the sequence of process actions for each process tree shown.


1. Answer
2. Answer
3. ...


## Question 4

One interesting thing to note is what happens when a child exits; what happens to its children in the process tree? To study this, let’s create a specific example:

`$ python3 ./fork.py -A a+b,b+c,c+d,c+e,c-`

This example has process ’a’ create ’b’, which in turn creates ’c’, which then creates ’d’ and ’e’. However, then, ’c’ exits. Take a moment to speculate with your group what you think the process tree should like after the exit. Run the same command again with the `-c` flag to verify your guess. Do some internet research about what happens to orphaned processes on Unix based systems like our Linux VMs. Write about what you find below. Does this explain the behavior?


ANSWER HERE
