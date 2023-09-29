#### 6. [2D transforms basics](#6)

#### 7. [CSS translate function](#7)

#### 8. [CSS scale function](#8)

#### 9. [CSS rotate function](#9)

#### 10.[ CSS skew function](#10)

#### 11.[ transform origin](#11)

---

<br>

### 6. 2D transforms basics<a id="6"></a>

> **_Business Objective: Layout_**

<img src="notes/6.gif">

| Technology    | Description     |
| ------------- | --------------- |
| `Language`    | html, css       |
| `Framework`   | -               |
| `Library`     | -               |
| `Text editor` | Vs code         |
| `Browser`     | Chrome, firefox |

---

<br>
Que: What are CSS transform what they can do for us. How they are different from CSS transition?

<br>

**CSS transition** : the transition allow to deal with css properties applied to specific element, and make those properties change smoothly over a specific period of time

like color, background-color, font-size, etc

<br>

**CSS transform** : control elements like div, images ..., changing element size, shape, position.

The transform property has four function

1. scale function
1. translate function
1. rotate function
1. skew function

<br>

---

- In index.html

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Transition</title>
    <style type="text/css">
      div {
        height: 150px;
        width: 150px;
        background-color: #40739e;
        color: white;
        line-height: 150px;
        text-align: center;
        font-size: 24px;
        margin: 20px;
        margin-right: auto;
        margin-left: auto;
        transition: transform 1s;
      }

      .scale:hover {
        transform: scale(1.2);
      }

      .translate:hover {
        transform: translateX(320px);
      }

      .rotate:hover {
        transform: rotate(180deg);
      }

      .skew:hover {
        transform: skew(20deg);
      }
    </style>
  </head>

  <body>
    <div class="scale">scale me</div>
    <div class="translate">translate me</div>
    <div class="rotate">rotate me</div>
    <div class="skew">skew me</div>
  </body>
</html>
```

<br>

### 7. CSS translate function<a id="7"></a>

> **_Business Objective: Layout_**

<img src="notes/7.gif">

| Technology    | Description     |
| ------------- | --------------- |
| `Language`    | html, css       |
| `Framework`   | -               |
| `Library`     | -               |
| `Text editor` | Vs code         |
| `Browser`     | Chrome, firefox |

---

- In index.html

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Transition</title>

    <style type="text/css">
      /* generic style */
      img {
        width: 300px;
        display: block;
        /* make it center of page */
        margin: auto;
        margin-top: 200px;

        /* 1️⃣ shorthand setup */
        transition: transform 2s;
      }

      img:hover {
        /* 2️⃣ translate function take two args: X-axis, Y-axis */
        /* move element from its original position */
        transform: translate(-500px, 200px);
      }
    </style>
  </head>

  <body>
    <img src="cat.jpg" alt="" />
  </body>
</html>

<!-- 

transfrom: translate(the value);

transform: translate(10px, 10px)

 -->
```

<br>

### 8. CSS scale function<a id="8"></a>

> **_Business Objective: Layout_**

<img src="notes/8.gif">

| Technology    | Description     |
| ------------- | --------------- |
| `Language`    | html, css       |
| `Framework`   | -               |
| `Library`     | -               |
| `Text editor` | Vs code         |
| `Browser`     | Chrome, firefox |

---

- In index.html

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Transition</title>
    <style type="text/css">
      /* generic style */
      img {
        width: 300px;
        display: block;
        margin: auto;
        margin-top: 200px;
        /* 1️⃣ setup */
        transition: transform 2s;
      }

      img:hover {
        /* 2️⃣ scale function takes two args */
        /* change the size of element */
        /* transform: scaleX(2); */
        /* transform: scaleY(0.5); */
        /* transform: scale(2, 2); */

        /* short hand */
        transform: scale(2);
      }
    </style>
  </head>

  <body>
    <img src="cat.jpg" alt="" />
  </body>
</html>
```

---

<br>

### 9. CSS rotate function<a id="9"></a>

> **_Business Objective: Layout_**

<img src="notes/9.gif">

| Technology    | Description     |
| ------------- | --------------- |
| `Language`    | html, css       |
| `Framework`   | -               |
| `Library`     | -               |
| `Text editor` | Vs code         |
| `Browser`     | Chrome, firefox |

---

- In index.html

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Transition</title>
    <style type="text/css">
      /* generic style */
      img {
        width: 300px;
        display: block;
        margin: auto;
        margin-top: 200px;

        /* 1️⃣ setup */
        transition: transform 2s;
      }

      img:hover {
        /* 2️⃣ rotate function takes one args in UNIT: degree, turn, gradian */
        /* clockwise: deg */
        /* transform: rotate(360deg); */

        /* counter clock-wise:deg */
        /* transform: rotate(-360deg); */

        /* clock-wise: turn */
        /* transform: rotate(1turn); */

        /* counter clock-wise: turn */
        /* transform: rotate(-1turn); */

        /* clock-wise:grad */
        transform: rotate(200grad);
      }
    </style>
  </head>

  <body>
    <img src="cat.jpg" alt="" />
  </body>
</html>
```

<br>

### 10. CSS skew function<a id="10"></a>

> **_Business Objective: Layout_**

<img src="notes/10.gif">

| Technology    | Description     |
| ------------- | --------------- |
| `Language`    | html, css       |
| `Framework`   | -               |
| `Library`     | -               |
| `Text editor` | Vs code         |
| `Browser`     | Chrome, firefox |

---

- In index.html

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Transition</title>
    <style type="text/css">
      /* generic style */
      img {
        width: 300px;
        display: block;
        margin: auto;
        margin-top: 200px;

        /* 1️⃣ setup */
        transition: transform 2s;
      }

      img:hover {
        /* 2️⃣ skew function takes two args in degree */
        /* skew horizontally */
        /* transform: skewX(30deg); */
        /* transform: skewX(-30deg); */

        /* skew vertically */
        /* transform: skewY(30deg); */
        /* transform: skewY(-30deg); */

        /* skew horizontally, Vertically at same time */
        transform: skew(20deg, 40deg);
      }
    </style>
  </head>

  <body>
    <img src="cat.jpg" alt="" />
  </body>
</html>
```

<br>

### 11. transform origin<a id="11"></a>

> **_Business Objective: Layout_**

CAT DEMO

<img src="notes/11a.gif">

| Technology    | Description     |
| ------------- | --------------- |
| `Language`    | html, css       |
| `Framework`   | -               |
| `Library`     | -               |
| `Text editor` | Vs code         |
| `Browser`     | Chrome, firefox |

---

- In index.html

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Transition</title>
    <style type="text/css">
      /* generic style */
      img {
        width: 300px;
        display: block;
        margin: auto;
        margin-bottom: 70px;
        margin-top: 70px;
        /* 1️⃣ setup */
        transition: transform 1s;
      }

      .second {
        /* 2️⃣ change origin or pivot point */
        transform-origin: top left;
        margin-bottom: 0;
      }

      /* 3️⃣ final state */
      .first:hover,
      .second:hover {
        /* rotate 30deg clock-wise */
        transform: rotate(30deg);
      }
    </style>
  </head>

  <body>
    <img src="cat.jpg" alt="" class="first" />
    <img src="cat.jpg" alt="" class="second" />
  </body>
</html>
```

---

> **_Business Objective: Layout_**

<img src="notes/11b.gif">

KEYWORD DEMO

| Technology    | Description     |
| ------------- | --------------- |
| `Language`    | html, css       |
| `Framework`   | -               |
| `Library`     | -               |
| `Text editor` | Vs code         |
| `Browser`     | Chrome, firefox |

---

| origin point                               | origin point                                     |
| ------------------------------------------ | ------------------------------------------------ |
| <img src="notes/1 top.png" width="200">    | <img src="notes/5 top right.png" width="200">    |
| <img src="notes/2 right.png" width="200">  | <img src="notes/6 bottom right.png" width="200"> |
| <img src="notes/3 bottom.png" width="200"> | <img src="notes/7 bottom left.png" width="200">  |
| <img src="notes/4 left.png" width="200">   | <img src="notes/8 top left.png" width="200">     |

---

- In index.html

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Transition</title>
    <link
      href="https://fonts.googleapis.com/css?family=Roboto+Slab"
      rel="stylesheet"
    />

    <!-- general style -->
    <style type="text/css">
      div {
        width: 150px;
        height: 150px;
        background-color: #27ae60;
        display: block;
        margin: auto;
        margin-bottom: 70px;
        color: white;
        font-size: 24px;
        font-family: "Roboto Slab", serif;
        text-align: center;
        line-height: 150px;
        /* 1️⃣setup */
        transition: transform 1s;
      }

      /* 3️⃣ final state */
      div:hover {
        transform: rotate(45deg);
      }

      /* 2️⃣ change origin/pivot point top centre*/
      .top {
        transform-origin: top;
      }

      /* 2️⃣ change origin/pivot point right centre*/
      .right {
        transform-origin: right;
      }

      /* 2️⃣ change origin/pivot point */
      .left {
        transform-origin: left;
      }

      /* 2️⃣ change origin/pivot point */
      .bottom {
        transform-origin: bottom;
      }

      /* 2️⃣ change origin/pivot point */
      .top-right {
        transform-origin: top right;
      }

      /* 2️⃣ change origin/pivot point */
      .top-left {
        transform-origin: top left;
      }

      /* 2️⃣ change origin/pivot point */
      .bottom-right {
        transform-origin: bottom right;
      }

      /* 2️⃣ change origin/pivot point */
      .bottom-left {
        transform-origin: bottom left;
      }
    </style>
  </head>

  <body>
    <div class="top">top</div>
    <div class="right">right</div>
    <div class="bottom">bottom</div>
    <div class="left">left</div>
    <div class="top-right">top right</div>
    <div class="bottom-right">bottom right</div>
    <div class="bottom-left">bottom left</div>
    <div class="top-left">top left</div>
  </body>
</html>
```

---

> **_Business Objective: Layout_**

X & Y OFFSETS

<img src="notes/11c.gif">

| Technology    | Description     |
| ------------- | --------------- |
| `Language`    | html, css       |
| `Framework`   | -               |
| `Library`     | -               |
| `Text editor` | Vs code         |
| `Browser`     | Chrome, firefox |

---

- In index.html

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Transition</title>
    <link
      href="https://fonts.googleapis.com/css?family=Roboto+Slab"
      rel="stylesheet"
    />
    <style type="text/css">
      div {
        width: 600px;
        height: 300px;
        background-color: #27ae60;
        display: block;
        margin: auto;
        margin-top: 150px;
        color: white;
        font-size: 28px;
        text-transform: capitalize;
        font-family: "Roboto Slab", serif;
        text-align: center;
        line-height: 300px;
        transition: transform 1s;
        transform-origin: 300px 150;
      }

      div:hover {
        transform: rotate(45deg);
      }
    </style>
  </head>

  <body>
    <div class="top">any html element</div>
  </body>
</html>
```

<br>
