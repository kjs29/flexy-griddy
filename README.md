1.

<img width="500" src="https://user-images.githubusercontent.com/96529477/224511062-c5aabb94-f3f0-4031-9641-ea4c8aae763f.png">
<details>

  <summary>html, css</summary>
  
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
</details>

2.

<img width="500" src="https://user-images.githubusercontent.com/96529477/224519480-e8aecdd0-2e99-4d1f-80c6-9a31405b2bf5.png">


<details>

  <summary>html, css</summary>
  
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
              grid-template: repeat(4, 1fr) / repeat(4, 1fr); 
              gap: 1rem;
          }
          .grid-container div {
              background-color: skyblue;
              padding: 40px;
              border: 1px solid black;
          }
          .item-1 {
              grid-column: 1/2;
              grid-row: 1/3;

          }
          .item-2 {
              grid-column: 2/5;

          }
          .item-3 {
              grid-column: 2/4;
              grid-row: 2/4;
          }
          .item-4 {
              grid-column: 4/5;
          }
          .item-5 {
          }
          .item-6 {

          }
          .item-7 {
              grid-column: 1/3;
          }
          .item-8 {
              grid-column: 3/5;
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
          <div class="item-8">8</div>
      </div>
  </body>
  </html>

  ```
</details>

3.

<img width="500" src="https://user-images.githubusercontent.com/96529477/224521318-1dbf8223-0730-44b4-9f77-dbc6a9290055.png">

<details>

  <summary>html, css</summary>
  
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
        padding: 30px;
      }
      .grid {
        display: grid;
        margin: 10px;
        grid-gap: 1rem;
        grid-template: repeat(4, 1fr) / repeat(4, 1fr);
      }
      .grid div{
        background-color: skyblue;
        padding: 40px;
        display: flex;
        justify-content: center;
        align-items: center;
      }
      .item-1 {
        grid-column: 1 / 4;
      }
      .item-2 {
        grid-column: 4 / 5;
        grid-row: 1 / 4;
      }
      .item-3 {
        grid-column: 2 / 4;
        grid-row: 2 / 4;
      }
      .item-4 {
        grid-column: 1 / 2;
        grid-row: 2 / 5;
      }
      .item-5 {
        grid-column: 2 / 5;
      }
    </style>
  </head>
  <body>
    <div class="grid">
      <div class="item-1">1</div>
      <div class="item-2">2</div>
      <div class="item-3">3</div>
      <div class="item-4">4</div>
      <div class="item-5">5</div>

    </div>
  </body>
  </html>

  ```
</details>

4.
![flex1 (1)](https://user-images.githubusercontent.com/96529477/225457036-5c77d312-5480-4867-85c3-fa24a02bdc73.gif)



<details>

  <summary>answer</summary>

  ```html
  <!DOCTYPE html>
  <html>
    <head>
      <style>
      .flex {
        display: flex;
        text-align: center;
        gap: 10px;
      }
      .flex div {
        background-color: skyblue;
        padding: 10px;
      }
      .first {
        flex: 0 0 100px;
      }
      .second {
        flex: 1 1 auto;
      }
      .third {
        flex: 0 0 100px;
      }
      </style>
    </head>
  <body>
    <div class="flex">
      <div class="first">1</div>
      <div class="second">2</div>
      <div class="third">3</div>
    </div>
  </body>
  </html>
  ```
</details>
