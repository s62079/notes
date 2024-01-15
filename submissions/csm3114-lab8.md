#flutter 

<div style="page-break-before: always">S62079</div>

## 1 Passing Data to Previous Screen
### 1.1 The use of async, wait and Future for asynchronous execution of code in Dart programming - Case 1

![](20231215225747.png)

1. print something
2. run and **wait** for async function
3. get the return value as output
4. print the output
5. print something

> [!async in my opinion (imo)]
> we all want to multitask, but realistically there is only one you, so you cant actually multitask. but you said you multitask before, how? well, in reality, you are just constantly swapping task from task A to task B then other tasks, and keep the tasks looping which feels seamless enough for you to think that you are multitasking. but no, you are not multitasking, you are just fast at switching context. and that is how async works, in simple. 

<div style="page-break-before: always">S62079</div>

### 1.2 The use of async, wait and Future for asynchronous execution of code in Dart programming - Case 2

![](20231215231036.png)

- `async` tells you that a function is allowed to run asynchronously
- `await` blocks the whole process until said async function finished running

<div style="page-break-before: always">S62079</div>

### 1.3 Passing data to the previous screen.

![](20231218102057.png)

the magic starts around line 35, it turns out the `Navigator.pop()` actually takes another argument(s?) that will be returned as value when popped, therefore you could technically pass data back to last page without putting a variable on 2nd page constructor.

<div style="page-break-before: always">S62079</div>

### 1.4 Exercise

that's it, i will build 1.4 on top of 1.3

![](20231218104414.png)

<div style="page-break-before: always">S62079</div>

## 2 Retrieving Data From Web Service
### 2.1 Register to web service the Movie Database API

![](20231210112830.png)

### 2.7 Create a main widget for the app

2.2 - 2.7 is one thing

![](20231218120816.png)

<div style="page-break-before: always">S62079</div>

nice movie btw

![](20231218121801.png)

search works too

![](20231218122055.png)