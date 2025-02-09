<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: white; /* White background */
            margin: 0;
        }

        .calc-container {
            background: #000; /* Black background for calculator */
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 8px 30px rgba(0, 0, 0, 0.2);
            text-align: center;
            width: 360px;
        }

        #output {
            width: 90%;
            height: 60px;
            font-size: 2.2rem;
            text-align: right;
            padding: 15px;
            border-radius: 8px;
            background: #333; /* Dark background for input */
            color: #fff; /* White text */
            border: 2px solid #444;
            margin-bottom: 25px;
        }

        .button-container {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 15px;
        }

        button {
            width: 75px;
            height: 75px;
            font-size: 1.6rem;
            border: none;
            border-radius: 12px;
            background: #e74c3c; /* Red buttons */
            color: #fff;
            cursor: pointer;
            transition: all 0.3s ease-in-out;
        }

        button:hover {
            background: #c0392b; /* Darker red for hover */
        }

        .action-btn {
            background: #d35400; /* Orange-red for actions like C, operators */
        }

        .action-btn:hover {
            background: #e67e22; /* Darker orange-red for hover */
        }

        button:nth-child(19), button:nth-child(21), button:nth-child(22), button:nth-child(23) {
            background: #e74c3c; /* Red for these special buttons */
        }

        button:nth-child(17) {
            background: #2980b9; /* Blue for equal sign */
        }

        button:nth-child(17):hover {
            background: #3498db; /* Lighter blue for hover */
        }

        button:last-child {
            background: #27ae60; /* Green for "=" button */
            grid-column: span 1;
        }

        button:last-child:hover {
            background: #2ecc71; /* Lighter green for hover */
        }

        button:first-child {
            background: #e74c3c; /* Red for clear button */
        }

        .special-btn {
            background: #9b59b6; /* Purple for special buttons */
        }

        .special-btn:hover {
            background: #8e44ad; /* Darker purple for hover */
        }
    </style>
</head>
<body>
    <div class="calc-container">
        <input type="text" id="output" placeholder="0">
        <div class="button-container">
            <button class="action-btn" onclick="clearDisplay()">C</button>
            <button class="special-btn" onclick="appendValue('(')">(</button>
            <button class="special-btn" onclick="appendValue(')')">)</button>
            <button class="action-btn" onclick="eraseLast()">&larr;</button>

            <button onclick="appendValue('7')">7</button>
            <button onclick="appendValue('8')">8</button>
            <button onclick="appendValue('9')">9</button>
            <button class="action-btn" onclick="appendValue('/')">/</button>

            <button onclick="appendValue('4')">4</button>
            <button onclick="appendValue('5')">5</button>
            <button onclick="appendValue('6')">6</button>
            <button class="action-btn" onclick="appendValue('*')">*</button>

            <button onclick="appendValue('1')">1</button>
            <button onclick="appendValue('2')">2</button>
            <button onclick="appendValue('3')">3</button>
            <button class="action-btn" onclick="appendValue('-')">-</button>

            <button onclick="appendValue('.')">.</button>
            <button onclick="appendValue('0')">0</button>
            <button class="special-btn" onclick="calculateSquareRoot()">&radic;</button>
            <button class="action-btn" onclick="appendValue('+')">+</button>

            <button class="special-btn" onclick="calculatePercentage()">%</button>
            <button class="special-btn" onclick="calculateSquare()">x²</button>
            <button class="special-btn" onclick="toggleNegate()">±</button>
            <button onclick="calculateResult()">=</button>
        </div>
    </div>

    <script>
        function appendValue(value) {
            document.getElementById('output').value += value;
        }

        function clearDisplay() {
            document.getElementById('output').value = '';
        }

        function calculatePercentage() {
            let output = document.getElementById('output');
            output.value = parseFloat(output.value) / 100;
        }

        function calculateSquareRoot() {
            let output = document.getElementById('output');
            let value = parseFloat(output.value);
            if (value >= 0) {
                output.value = Math.sqrt(value);
            } else {
                output.value = 'Error';
            }
        }

        function calculateSquare() {
            let output = document.getElementById('output');
            let value = parseFloat(output.value);
            output.value = value * value;
        }

        function toggleNegate() {
            let output = document.getElementById('output');
            let value = parseFloat(output.value);
            if (output.value !== "") {
                output.value = -value;
            }
        }

        function eraseLast() {
            let output = document.getElementById('output');
            output.value = output.value.slice(0, -1);
        }

        function calculateResult() {
            try {
                document.getElementById('output').value = eval(document.getElementById('output').value);
            } catch (error) {
                document.getElementById('output').value = 'Error';
            }
        }
    </script>
</body>
</html>
