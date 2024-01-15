#flutter

<div style="page-break-before: always">S62079</div>

## 1 Flutter Form
### 1.1 The construction of form inputs and applying the relevant theme to the UI and the form inputs

![](20231217110452.png)

> [! lesson of the day (lab)]
> 1. styling `TextField`
> 2. doing `TextEditingController`

<div style="page-break-before: always">S62079</div>

### 1.2 Exercise

![](20231217114503.png)

> [!learned]
> - `TextFormField` is `TextField`, but better. it has built-in form function, allow developer to do some verifying stuff (TL;DR implemented with `Form`, which makes it optional) 
> - `GlobalKey` can be used to store all kind of widget state, depending on how you use it. usually being put at top of hierarchy

<div style="page-break-before: always">S62079</div>

### 1.3 Implementing focus on the form fields

> [!learned]
> - `dispose()` for garbage cleaning when changing/closing page maybe
> - `autofocus` can be used to set the first focused widget in a page, probably accessibility friendly 
> - `FocusNode` can be used to control the focus state of widget, note that there can only be one focused widget at a time (probably)

![](20231217152540.png)

<div style="page-break-before: always">S62079</div>

### 1.4 Handling the data changes through `TextField` by implementing the ActionListener to the `TextEditController`

i will chain it with `1.3`, for the sake of seamless flow. also, it allows me to actually explore about what actually happened and implement it myself instead of just copying code, that'd be boring. 

![](20231217154450.png)

cons: slow job, if anything, i should have just copied the code to finish the job ASAP

<div style="page-break-before: always">S62079</div>

### 1.5 Retrieve value from `TextField` when user make a request

![](20231217231245.png)

<div style="page-break-before: always">S62079</div>

### 1.6 Implementing Form validation

you probably realized that back in 1.2 i have accidentally did an hour worth of research of `TextFormField`. so, instead of wrapping the data in form with `GlobalKey<FormState>`, you can actually assign `GlobalKey<FormFieldState>` to the field instead, for individual state monitoring. 

![](20231218000136.png)

<div style="page-break-before: always">S62079</div>

### 1.7 Exercise

now this is a good use case for `Form`

![](20231218093918.png)

![](20231218095619.png)

<div style="page-break-before: always">S62079</div>

### 1.8 Bonus

oh yeah, and the grocery list app

![](20231218100345.png)
