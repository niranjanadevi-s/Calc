# Ex.08 Design of a Standard Calculator
## Date: 25.04.2024
## AIM:
To design a web application for a standard calculator with minimum five operations.
## DESIGN STEPS:
Step 1: Clone the github repository and create Django admin interface.

Step 2: Change settings.py file to allow request from all hosts.

Step 3: Use CSS for creating attractive colors.

Step 4: Write JavaScript program for implementing five different operations.

Step 5: Validate the HTML and CSS code.
## PROGRAM :
## index.html
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
    <link rel="stylesheet" href="style.css">
    <script src="index.js" defer></script>
</head>
<body>
    <div class="name">
        <h1>&nbsp;&nbsp;&nbsp;&nbsp;Calculator</h1>
        <h2>Niranjana devi S[212221220036]</h2>
    </div>
<div id="calculator">
    <input type="button" value="7" onclick="addToDisplay('7')">
    <input type="button" value="8" onclick="addToDisplay('8')">
    <input type="button" value="9" onclick="addToDisplay('9')">
    <input type="button" value="/" onclick="addToDisplay('/')">
    <br>
    <input type="button" value="4" onclick="addToDisplay('4')">
    <input type="button" value="5" onclick="addToDisplay('5')">
    <input type="button" value="6" onclick="addToDisplay('6')">
    <input type="button" value="-" onclick="addToDisplay('-')">
    <br>
    <input type="button" value="1" onclick="addToDisplay('1')">
    <input type="button" value="2" onclick="addToDisplay('2')">
    <input type="button" value="3" onclick="addToDisplay('3')">
    <input type="button" value="+" onclick="addToDisplay('+')">
</div>
</body>
</html>
## style.css
body {
    font-family: Arial, sans-serif;
    display: flex;
    align-items: center;
    justify-content: center;
}
#calculator {
    border: 2px solid #b616a6;
    border-radius: 5px;
    padding: 60px;
}
input[type="text"] {
    width: 100%;
    padding: 10px;
    margin-bottom: 10px;
    font-size: 18px;
}
input[type="button"] {
    width: 60px;
    height: 60px;
    font-size: 25px;
~~~
~~~
    margin: 5px;
}input[type="button"]:hover {
    background-color: #eee;}
#clear {
    background-color: rgb(22, 46, 231);
    color: #fff;
}
## index.js
function addToDisplay(value) {
    document.getElementById('display').value += value;
}
function calculate() {
    try {
        document.getElementById('display').value = eval(document.getElementById('display').value);
    } catch (error) {
        document.getElementById('display').value = 'Error';
    }
}
~~~
## OUTPUT:
![image](https://github.com/niranjanadevi-s/Calc/assets/141748873/af0eeba0-efcc-4468-a99d-8f109fddbef8)
![image](https://github.com/niranjanadevi-s/Calc/assets/141748873/d7d1a90b-bb6c-43a9-9dcc-a44f59c92aa2)
## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
