<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Maths Learning Hub</title>

    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            background: #f4f4f4;
        }

        header {
            background: #1e88e5;
            color: white;
            padding: 20px;
            text-align: center;
        }

        nav {
            background: #1565c0;
            padding: 10px;
            text-align: center;
        }

        nav a {
            color: white;
            margin: 10px;
            text-decoration: none;
            font-weight: bold;
        }

        section {
            padding: 20px;
        }

        .card {
            background: white;
            padding: 15px;
            margin: 10px 0;
            border-radius: 8px;
        }

        input, button {
            padding: 10px;
            margin: 5px;
        }

        button {
            background: #1e88e5;
            color: white;
            border: none;
            cursor: pointer;
        }
    </style>
</head>

<body>

<header>
    <h1>📘 Mathematics Learning Hub</h1>
    <p>Learn Maths Easily & Quickly</p>
</header>

<nav>
    <a href="#topics">Topics</a>
    <a href="#calculator">Calculator</a>
</nav>

<section id="topics">
    <h2>📚 Topics</h2>

    <div class="card">
        <h3>Algebra</h3>
        <p>Equations, expressions, and formulas.</p>
    </div>

    <div class="card">
        <h3>Geometry</h3>
        <p>Shapes, angles, and measurements.</p>
    </div>

    <div class="card">
        <h3>Statistics</h3>
        <p>Mean, median, mode, and graphs.</p>
    </div>
</section>

<section id="calculator">
    <h2>🧮 Simple Calculator</h2>

    <input type="number" id="num1" placeholder="First number">
    <input type="number" id="num2" placeholder="Second number">

    <br>

    <button onclick="add()">Add</button>
    <button onclick="subtract()">Subtract</button>
    <button onclick="multiply()">Multiply</button>
    <button onclick="divide()">Divide</button>

    <h3 id="result">Result: </h3>
</section>

<script>
    function add() {
        let a = Number(document.getElementById("num1").value);
        let b = Number(document.getElementById("num2").value);
        document.getElementById("result").innerText = "Result: " + (a + b);
    }

    function subtract() {
        let a = Number(document.getElementById("num1").value);
        let b = Number(document.getElementById("num2").value);
        document.getElementById("result").innerText = "Result: " + (a - b);
    }

    function multiply() {
        let a = Number(document.getElementById("num1").value);
        let b = Number(document.getElementById("num2").value);
        document.getElementById("result").innerText = "Result: " + (a * b);
    }

    function divide() {
        let a = Number(document.getElementById("num1").value);
        let b = Number(document.getElementById("num2").value);

        if (b === 0) {
            document.getElementById("result").innerText = "Cannot divide by zero";
        } else {
            document.getElementById("result").innerText = "Result: " + (a / b);
        }
    }
</script>

</body>
</html>
