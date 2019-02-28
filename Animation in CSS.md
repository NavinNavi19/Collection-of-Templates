# Animation in CSS using `animation` and `@keyframe` elements.

```html
<!DOCTYPE html>
<html>
    <head>
        <title>CSS Animation</title>
        <link rel="stylesheet" type="text/css" href="shape.css">
    </head>
    <body>
        <div></div>
    </body>
</html>
```

```css
div {
    margin: 40vh auto;
    width: 200px;
    height: 200px;
    background-color: coral;
    animation: square-to-circle 2s 1s infinite  alternate;
}

@keyframes square-to-circle {
    0%  {
      border-radius:0 0 0 0;
      background:coral;
      transform:rotate(0deg);
    }
    25%  {
      border-radius:50% 0 0 0;
      background:darksalmon;
      transform:rotate(45deg);
    }
    50%  {
      border-radius:50% 50% 0 0;
      background:indianred;
      transform:rotate(90deg);
    }
    75%  { 
      border-radius:50% 50% 50% 0;
      background:lightcoral;
      transform:rotate(135deg);
    }
    100% {  
      border-radius:50%;
      background:darksalmon;
      transform:rotate(180deg);
    }
  }
```
