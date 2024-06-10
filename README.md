# JavaScript-Operators-Operands-Order-Precedence
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grade Average Calculator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            text-align: center;
            margin-top: 50px;
        }
        h1 {
            color: #333;
        }
        #gradeInput {
            margin-bottom: 20px;
        }
        #calculateBtn {
            padding: 10px 20px;
            background-color: #4caf50;
            color: white;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }
        #result {
            font-size: 24px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <h1>Grade Average Calculator</h1>
    <div id="gradeInput">
        <label for="grade1">Subject 1 Grade:</label>
        <input type="number" id="grade1" min="0" max="100"><br>
        <label for="grade2">Subject 2 Grade:</label>
        <input type="number" id="grade2" min="0" max="100"><br>
        <label for="grade3">Subject 3 Grade:</label>
        <input type="number" id="grade3" min="0" max="100"><br>
        <label for="grade4">Subject 4 Grade:</label>
        <input type="number" id="grade4" min="0" max="100"><br>
        <label for="grade5">Subject 5 Grade:</label>
        <input type="number" id="grade5" min="0" max="100"><br>
        <button id="calculateBtn">Calculate Average</button>
    </div>
    <div id="result"></div>

    <script>
        document.getElementById('calculateBtn').addEventListener('click', function() {
            var grade1 = parseFloat(document.getElementById('grade1').value);
            var grade2 = parseFloat(document.getElementById('grade2').value);
            var grade3 = parseFloat(document.getElementById('grade3').value);
            var grade4 = parseFloat(document.getElementById('grade4').value);
            var grade5 = parseFloat(document.getElementById('grade5').value);

            var average = (grade1 + grade2 + grade3 + grade4 + grade5) / 5;

            document.getElementById('result').innerHTML = "Average Grade: " + average.toFixed(2);
        });
    </script>
</body>
</html>
