1.

<img width="500" src="https://user-images.githubusercontent.com/96529477/224511062-c5aabb94-f3f0-4031-9641-ea4c8aae763f.png">

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body {
            padding : 20px;
            text-align: center;
        }
        .grid-container {
            display: grid;
            grid-template: repeat(4, 1fr) / repeat(8, 1fr); 
            gap: 1rem;
        }
        .grid-container div {
            background-color: skyblue;
            padding: 40px;
            border: 1px solid black;
        }
        .item-1 {
            grid-column-start: 1;
            grid-column: span 8;
        }
        .item-2 {
            grid-column: 1 / 2;
        }
        .item-3 {
            grid-column: 2 / 7;
        }
        .item-4 {
            grid-column: 7 / 9;
        }
        .item-5 {
            grid-column: 1 / 5;
        }
        .item-6 {
            grid-column: 5 / 9;
        }
        .item-7 {
            grid-column-start: 1;
            grid-column: span 8;
        }
    </style>
</head>
<body>
    <div class="grid-container">
        <div class="item-1">1</div>
        <div class="item-2">2</div>
        <div class="item-3">3</div>
        <div class="item-4">4</div>
        <div class="item-5">5</div>
        <div class="item-6">6</div>
        <div class="item-7">7</div>
    </div>
</body>
</html>

```
