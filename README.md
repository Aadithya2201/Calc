# Ex.08 Design of a Standard Calculator
## Date:26.04.2024

## AIM:
To design a web application for a standard calculator with minimum five operations.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
calc.html

<html>
<head>
    <title>Standard Calculator</title>
    <link rel="stylesheet" href="style.css">
    <script src="working.js"></script>
</head>
<body bgcolor="AQUA">
    <center>
    <table border="10" bgcolor="cyan" style="border-color: red;">
        <caption> <H2><b>AADITHYA R 212223240001</b></H2></caption>
        <tr>
            <td colspan="4">
                <input type="text" id="result">
            </td>
        </tr>
        <tr>
            <td>
                <input type="button" value="(" onclick="dis()">
            </td>
            <td>
                <input type="button" value=")" onclick="dis()">
            </td>
            <td>
                <input type="button" value="C" onclick="clr()">
            </td>
            <td>
                <input type="button" value="%" onclick="percent()">
            </td>
        </tr>
        <tr>
            <td>
                <input type="button" value="7" onclick="dis('7')">
            </td>
            <td>
                <input type="button" value="8" onclick="dis('8')">
            </td>
            <td>
                <input type="button" value="9" onclick="dis('9')">
            </td>
            <td>
                <input type="button" value="X" onclick="dis('/')">
            </td>
        </tr>
        <tr>
            <td>
                <input type="button" value="4" onclick="dis('4')">
            </td>
            <td>
                <input type="button" value="5" onclick="dis('5')">
            </td>
            <td>
                <input type="button" value="6" onclick="dis('6')">
            </td>
            <td>
                <input type="button" value="-" onclick="dis('-')">
            </td>
        </tr>
        <tr>
            <td>
                <input type="button" value="1" onclick="dis('1')">
            </td>
            <td>
                <input type="button" value="2" onclick="dis('2')">
            </td>
            <td>
                <input type="button" value="3" onclick="dis('3')">
            </td>
            <td>
                <input type="button" value="+" onclick="dis('+')">
            </td>
        </tr>
        <tr>
            <td>
                <input type="button" value="0" onclick="dis('0')">
            </td>
            <td>
                <input type="button" value="." onclick="dis('0')">
            </td>
            <td>
                <input type="button" value="=" onclick="solve()">
            </td>
            <td>
                <input type="button" value="*" onclick="dis('*')">
            </td>
        </tr>
    </table>
</center>
</body>
</html>

style.css

input[type="text"]{
    background-color: white;
    border: solid brown 2px;
    width:100%;
}
input[type="button"]{
    background-color: orange;
    color: black;
    border-radius: 10px;
    width: 100%;
}

working.js

function percent() {
    x = document.getElementById("result").value;
    y = eval(x);
    percentage = y / 100;
    document.getElementById("result").value = percentage;
}
function solve() {
    x = document.getElementById("result").value;
    y = eval(x);
    document.getElementById("result").value = y;
}

function clr() {
    document.getElementById("result").value = "";
}
function dis(val) {
    document.getElementById("result").value += val;
}


```

## OUTPUT:
![alt text](<Screenshot (35).png>)
![alt text](<Screenshot (36).png>)
## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
