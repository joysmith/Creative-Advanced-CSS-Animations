#### 12. [translate in 3D](#12)

#### 13. [rotate in 3D](#13)

---

<br>

### 12. translate in 3D<a id="12"></a>

> **_Business Objective: Layout_**

<img src="notes/12.gif" >

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
    <title>translate in 3D</title>
    <style type="text/css">
      body {
        perspective: 500px;
      }

      img {
        width: 300px;
        display: block;
        margin: auto;
        margin-top: 200px;
        transition: transform 1s;
      }

      img:hover {
        transform: translateZ(800px);
      }
    </style>
  </head>

  <body>
    <img src="cat.jpg" alt="" />
  </body>
</html>
```

<br>

### 13. rotate in 3D<a id="13"></a>

> **_Business Objective: Layout_**

<img src="notes/13.gif" >

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
    <title>translate in 3D</title>
    <style type="text/css">
      body {
        perspective: 500px;
      }

      img {
        width: 300px;
        display: block;
        margin: auto;
        margin-top: 200px;
        transition: transform 1s;
      }

      img:hover {
        transform: rotateY(60deg);
      }
    </style>
  </head>

  <body>
    <img src="cat.jpg" alt="" />
  </body>
</html>
```

<br>
