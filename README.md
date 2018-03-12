# Intro to chessboardjs

## What are we doing?

Chessboard js is an awesome tool we can use to simulate a chess board! Note that this will NOT simulate chess on its own, we'd need a separate library for that. 

A major purpose of this lesson will be to learn about javascript objects, and importing new tools. 

## Getting started

To get started, we need to download the chessboardjs files from [here](http://chessboardjs.com/). It'll download as a zip file, but we should unzip it, and then put the unzipped folder somewhere we can use it -- this is going to be our main folder.

Inside the folder, we need to add two new files - `index.html`, which will store our html, and `script.js`, where we'll be putting our own custom javascript.

To get started in `index.html`, use the below code. (Obviously, you can ignore the commented out portions.)
```
<html>
<head>
<!--  Including the chessboardjs files:-->
    <script src="./js/chessboard-0.3.0.js"></script>
    <link rel="stylesheet" href="css/chessboard-0.3.0.min.css">

<!--  Including jQuery, another tool chessboardjs uses:-->
    <script src="https://code.jquery.com/jquery-1.12.4.min.js"></script>
  
  </head>
<body>
  <div id="board1" style="width: 400px"></div>
  </body>

  
  
<!--
  Now including our own custom JS
  Note that we could write JS directly in between the script tags if you'd 
  rather, but i didn't want to so i put it in a new file. 
-->
  <script src="./script.js"></script>
</html>

```

And here's a good starting template for script.js: 

```
var config = {
  position: 'start',
  draggable: true
}


var board1 = ChessBoard('board1', config);
```
