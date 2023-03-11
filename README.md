1.

<img width="500" src="https://user-images.githubusercontent.com/96529477/224511062-c5aabb94-f3f0-4031-9641-ea4c8aae763f.png">
<details>

  <summary>css</summary>
  
  ```css
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
  ```
</details>
