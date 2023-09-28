#### 1. [Creative Advanced CSS Animations - Create 100 Projects!](#1)

#### 2. [what is CSS transitions ?](#2)

#### 3. [CSS transitions options](#3)

#### 4. [different ways to write the transition property](#4)

#### 5. [what properties can be transitioned ?](#5)

---

<br>

### 1. Creative Advanced CSS Animations - Create 100 Projects!<a id="1"></a>

<br>

### 2. what is CSS transitions ?<a id="2"></a>

> **_Business Objective: Layout_**

<img src="notes/2.gif" >

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
<html lang="en-US">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>CSS animation, transitions and transforms</title>

    <!-- OUR STYLESHEET -->
    <link rel="stylesheet" href="style.css" type="text/css" media="all" />
  </head>

  <body>
    <button>css transition</button>
  </body>
</html>
```

---

- In style.css

```css
button {
  height: 90px;
  width: 290px;
  font-size: 28px;
  color: white;
  border: none;
  background-color: blue;
  transition-property: background-color;
  transition-duration: 3000ms;
}

button:hover {
  background-color: green;
}
```

<br>

### 3. CSS transitions options<a id="3"></a>

> **_Business Objective: Layout_**

<img src="notes/3.gif" >

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
<html lang="en-US">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>CSS animatin, transitions and transforms</title>

    <!-- OUR STYLESHEET -->
    <link rel="stylesheet" href="style.css" type="text/css" media="all" />
  </head>

  <body>
    <div class="container">
      <div id="ease" class="move">Ease (Default)</div>
      <div id="linear" class="move">Linear</div>
      <div id="ease-in" class="move">Ease-In</div>
      <div id="ease-out" class="move">Ease-Out</div>
      <div id="ease-in-out" class="move">Ease-In-Out</div>
    </div>
  </body>
</html>
```

---

- In style.css

```css
.container {
  width: 960px;
}

.move {
  margin: 2em;
  width: 150px;
  height: 50px;
  padding: 10px 15px;
  background-color: red;
  color: #fff;
  line-height: 50px;
  text-align: center;
  border-radius: 0.5em;
  font-size: 20px;
  transition-property: translate();
  transition-duration: 3s;
}

#ease {
  transition-timing-function: ease;
}

#linear {
  transition-timing-function: linear;
}

#ease-in {
  transition-timing-function: ease-in;
}

#ease-out {
  transition-timing-function: ease-out;
}

#ease-in-out {
  transition-timing-function: ease-in-out;
}

.move:hover {
  transform: translate(900px, 0);
}
```

<br>

### 4. different ways to write the transition property<a id="4"></a>

> **_Business Objective: Layout_**

<img src="notes/4.gif" >

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
<html lang="en-US">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>CSS animatin, transitions and transforms</title>

    <!-- OUR STYLESHEET -->
    <link rel="stylesheet" href="style.css" type="text/css" media="all" />
  </head>

  <body>
    <button>css transition</button>
  </body>
</html>
```

---

- In style.css

```css
button {
  height: 90px;
  width: 290px;
  font-size: 28px;
  color: white;
  border: none;
  background-color: blue;
  transition: all 3s ease-in 2s;
}

button:hover {
  background-color: green;
  color: black;
  border-radius: 50%;
}
```

<br>

### 5. what properties can be transitioned ?<a id="5"></a>

> **_Business Objective: Layout_**

<img src="notes/5.gif" >

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
<html lang="en-US">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>CSS animatin, transitions and transforms</title>

    <!-- OUR STYLESHEET -->
    <link rel="stylesheet" href="style.css" type="text/css" media="all" />
  </head>

  <body>
    <div class="background">background</div>
    <div class="color">color</div>
    <div class="font-size">font-size</div>
    <div class="height">height</div>
    <div class="width">width</div>
    <div class="letter-spacing">letter-spacing</div>
    <div class="line-height">line-height</div>
    <div class="margin-top">margin-top</div>
    <div class="margin-bottom">margin-bottom</div>
    <div class="opacity">opacity</div>
    <div class="padding">padding</div>
    <div class="border-color">border-color</div>
    <div class="border-width">border-width</div>
  </body>
</html>
```

---

- In style.css

```css
div {
  height: 90px;
  width: 290px;
  font-size: 28px;
  margin: 20px;
  color: white;
  border: none;
  background-color: blue;
  line-height: 90px;
  text-align: center;
  transition: all 1s;
}

.background:hover {
  background-color: green;
}

.color:hover {
  color: red;
}

.font-size:hover {
  font-size: 32px;
}

.height:hover {
  height: 120px;
}

.width:hover {
  width: 340px;
}

.letter-spacing:hover {
  letter-spacing: 5px;
}

.line-height:hover {
  line-height: 120px;
}

.margin-bottom:hover {
  margin-bottom: 50px;
}

.margin-top:hover {
  margin-top: 50px;
}

.opacity:hover {
  opacity: 0.3;
}

.padding:hover {
  padding: 20px;
}

.border-color,
.border-width {
  border: 6px solid green;
}

.border-color:hover {
  border-color: red;
}

.border-width:hover {
  border-width: 12px;
}
```

<br>
