#flutter 

<div style="page-break-before: always">S62079</div>

## 1 Navigation of Screens
### 1.1 Creating a Flutter project

![](20231203172207.png)

a fresh project

### 1.2 Creating the UI for screen 1

![](20231203181240.png)

<div style="page-break-before: always">S62079</div>

### 1.3 Creating the UI for screen 2

![](20231203182106.png)

unlike screen1, this one is quite functional to begin with

> [!Editor's Note]
> there is in fact, an error here, note the `AppBar` title being 'Screen 1' instead of the supposed 'Screen 2', of course it is fixed shortly after

### 1.4 Creating the UI for screen 3

![](20231203183311.png)

### 1.5 Updating the main program

![](20231203184507.png)

![](20231203184530.png)

![](20231203184554.png)

> [!Editor's Note]
> have since then updated the color scheme's primary and secondary color, now brighter

### 1.6 Exercise

![](20231203233532.png)

![](20231203233828.png)

![](20231203233900.png)

9. Explain in details the differences between using `Navigator.pushNamed()` and `Navigator.push()`.

| `Navigator.pushNamed()` | `Navigator.push()` |
| - | - |
| takes `String` as parameter | takes `MaterialPageRoute` as parameter |
| rely on preset `routes` in main app | rely on `MaterialPageRoute`'s destination widget |

<div style="page-break-before: always">S62079</div>

## 2 Screens Navigation
### 2.1 Implementing Drawer widget with the `ListView` and `ListTile` widget

![](20231209002045.png)

Did it in `screen3.dart`, it is more cost efficient, wide banner is cool too so no sized box. 

### 2.2 Navigate to the next screen by invoking a `Navigator.push()` method inside the `ListTile` widget

![](20231211005728.png)

### 2.3 Exercise

oh, i have accidentally did 2.3 without realizing it

<div style="page-break-before: always">S62079</div>

### 3 Passing Data to the Next Screen
### 3.1 Create New Project
### 3.2 Define a Class Product

![](20231211130522.png)

### 3.3 Create a `ProductDetailsScreen` widget

![](20231211134018.png)

![](20231211134514.png)

![](20231211134530.png)

- what i have learned: you can pass data to other page with constructor of the other page
- also: android studio hedgehog's android emulator is bugged, cpu hogging (no pun) me 
