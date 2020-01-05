# Insp3ct0r
**Points:** 50

## Category
Web Exploitation

## Task
Kishor Balan tipped us off that the following code may need inspection: ```https://2019shell1.picoctf.com/problem/9509/``` ([link](https://2019shell1.picoctf.com/problem/9509/)) or http://2019shell1.picoctf.com:9509

## Solution
The first thing that I usually do in these situations is look at the page source. Different sublink's page source gives different parts of the flag.

URL: ```view-source:https://2019shell1.picoctf.com/problem/9509/```
```html
<!-- Html is neat. Anyways have 1/3 of the flag: picoCTF{tru3_d3 -->
```

URL: ```view-source:https://2019shell1.picoctf.com/problem/9509/mycss.css```
```css
/* You need CSS to make pretty pages. Here's part 2/3 of the flag: t3ct1ve_0r_ju5t */
```

URL: ```view-source:https://2019shell1.picoctf.com/problem/9509/myjs.js```
```javascript
/* Javascript sure is neat. Anyways part 3/3 of the flag: _lucky?8a7e3144} */
```

## Flag
> picoCTF{tru3_d3t3ct1ve_0r_ju5t_lucky?8a7e3144}
