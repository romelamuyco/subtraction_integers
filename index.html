<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Integer Subtraction Digital Game</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #ADD8E6;
            text-align: center;
            margin: 0;
            padding: 0;
        }

        #gameContainer {
            display: block;
        }

        #endGameContainer {
            display: none;
        }

        #title {
            font-size: 20px;
            font-weight: bold;
            color: blue;
            margin-top: 20px;
        }

        #author {
            color: blue;
        }

        #question {
            font-size: 32px;
            font-weight: bold;
            margin: 20px 0;
        }

        #answer {
            font-size: 24px;
            font-weight: bold;
            padding: 10px;
            margin-top: 8px;
            text-align: center;
            display: block;
            margin-left: auto;
            margin-right: auto;
            width: 80%; /* Adjust the width for mobile responsiveness */
            max-width: 250px; /* Set a maximum width */
        }

        #result {
            font-size: 14x;
            font-weight: bold;
            color: red;
            margin-top: 10px;
        }

        #statistics {
            font-size: 15px;
            margin-top: 20px;
        }

        #timer {
            font-size: 20px;
            margin-top: 10px;
        }

        #buttons {
            margin-top: 20px;
            display: flex;
            justify-content: center; /* Center horizontally */
            align-items: center; /* Center vertically */
        }

        button {
            font-size: 14px;
            font-weight: bold;
            padding: 10px;
            margin: 10px;
            cursor: pointer;
            border-radius: 50%; /* Make the buttons circular */
            width: 80px; /* Set a fixed width for circular buttons */
            height: 80px; /* Set a fixed height for circular buttons */
            color: black; /* Set the font color to black */
        }

        #submitBtn {
            background-color: #9370DB; /* Green */
            color: white;
            border: none;
        }

        #newGameBtn {
            background-color: #008CBA; /* Blue */
            color: white;
            border: none;
        }

        #exitBtn {
            background-color: #00008B; /* Red */
            color: white;
            border: none;
        }

        #newGameBtnEnd {
            background-color: green; /* Green */
            color: black;
            border: none;
        }

        #exitBtnEnd {
            background-color: gold; /* Gold */
            color: black;
            border: none;
        }

        #newGameBtnEnd,
        #exitBtnEnd {
            width: 80px; /* Adjust width as needed */
        }

        #endGameMessage {
            margin-top: 20px;
            font-size: 18px;
            font-weight: bold;
            color: green;
        }

        #endGameButtons {
            display: flex;
            justify-content: center; /* Center horizontally */
            align-items: center; /* Center vertically */
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div id="gameContainer">
        <div id="title">Integer Subtraction Digital Game</div>
        <div id="author">Romela A. Muyco</div>
        <div id="question"></div>
        <input type="text" id="answer" placeholder="Your answer" autocomplete="off" onblur="restorePlaceholder()">
        <div id="result"></div>
        <div id="statistics">Statistics: Correct Answers - 0, Wrong Answers - 0, Total Answered - 0</div>
        <div id="timer">Time Left: 600 seconds</div>
        <div id="buttons">
            <button id="submitBtn" onclick="checkAnswer()">Submit</button>
            <button id="newGameBtn" onclick="startNewGame()">New Game</button>
            <button id="exitBtn" onclick="exitGame()">Exit</button>
        </div>
    </div>
    <div id="endGameContainer">
        <div id="endGameMessage"></div>
        <div id="endGameButtons">
            <button id="newGameBtnEnd" onclick="startNewGame()">Play Again</button>
            <button id="exitBtnEnd" onclick="exitGame()">Exit</button>
        </div>
    </div>
    <script>
        let correctAnswers;
        let wrongAnswers;
        let totalAnswered;
        let timeLeft;
        let timerInterval;
        let questions;

        function generateQuestions() {
            const generatedQuestions = [];
            for (let i = 0; i < 40; i++) {
                const num1 = getRandomInt(-9, 9); // Single-digit integers
                const num2 = getRandomInt(-9, 9);
                generatedQuestions.push({ num1, num2 });
            }
            return generatedQuestions;
        }

        function getRandomInt(min, max) {
            return Math.floor(Math.random() * (max - min + 1)) + min;
        }

        function displayQuestion() {
            const questionElement = document.getElementById('question');
            const num1 = questions[0].num1;
            const num2 = questions[0].num2 < 0 ? `(${questions[0].num2})` : questions[0].num2;
            questionElement.textContent = `${num1} - ${num2} =`;
        }

        function clearPlaceholder() {
            const answerInput = document.getElementById('answer');
            if (answerInput.value === '') {
                answerInput.placeholder = '';
            }
        }

        function restorePlaceholder() {
            document.getElementById('answer').placeholder = 'Your answer';
        }

        function checkAnswer() {
            totalAnswered++;

            const userAnswer = parseInt(document.getElementById('answer').value, 10);
            const correctAnswer = questions[0].num1 - questions[0].num2;

            if (userAnswer === correctAnswer) {
                correctAnswers++;
                document.getElementById('result').textContent = 'Correct!';
            } else {
                wrongAnswers++;
                const specificRule = getSpecificRule(questions[0].num1, questions[0].num2);
                document.getElementById('result').textContent = `Incorrect! The correct answer is ${correctAnswer}. ${specificRule}`;
            }

            document.getElementById('statistics').textContent = `Statistics: Correct Answers - ${correctAnswers}, Wrong Answers - ${wrongAnswers}, Total Answered - ${totalAnswered}`;

            questions.shift(); // Remove the first question

            document.getElementById('answer').value = '';

            if (questions.length > 0) {
                displayQuestion();
            } else {
                endGame();
            }
        }

        function getSpecificRule(num1, num2) {
            // Provide specific rules based on the values of num1 and num2
            if (num1 > 0 && num2 < 0) {
                return 'When subtracting a negative number, it is the same as adding its positive counterpart.';
            } else if (num1 < 0 && num2 > 0) {
                return 'When subtracting a positive number, it is the same as adding its negative counterpart.';
            } else {
                // Add more rules based on specific conditions if needed
                return 'When subtracting integers, subtract the second number from the first number.';
            }
        }

        function endGame() {
            clearInterval(timerInterval);
            const percentageCorrect = (correctAnswers / totalAnswered) * 100;
            const completionMessage = `Congratulations! You completed the game. Your score: ${correctAnswers}/${totalAnswered} (${percentageCorrect.toFixed(2)}% correct).`;
            document.getElementById('endGameMessage').textContent = completionMessage;

            // Toggle visibility of game and end game containers
            document.getElementById('gameContainer').style.display = 'none';
            document.getElementById('endGameContainer').style.display = 'block';
        }

        function updateTimer() {
            timeLeft--;
            document.getElementById('timer').textContent = `Time Left: ${timeLeft} seconds`;
            if (timeLeft <= 0) {
                endGame();
            }
        }

        function startNewGame() {
            // Reset game variables
            correctAnswers = 0;
            wrongAnswers = 0;
            totalAnswered = 0;
            timeLeft = 601; // Set timeLeft to 600 seconds
            clearInterval(timerInterval);
            questions = generateQuestions();

            // Display game container and hide end game container
            document.getElementById('gameContainer').style.display = 'block';
            document.getElementById('endGameContainer').style.display = 'none';

            // Reset game elements
            displayQuestion();
            document.getElementById('answer').value = '';
            document.getElementById('result').textContent = ''; // Clear the result message
            document.getElementById('answer').style.display = 'block';
            document.getElementById('result').style.display = 'block';
            document.getElementById('timer').style.display = 'block';
            document.getElementById('question').style.fontWeight = 'bold'; // Set font weight to bold
            document.getElementById('statistics').textContent = 'Statistics: Correct Answers - 0, Wrong Answers - 0, Total Answered - 0';

            // Update timer immediately
            updateTimer();
            
            // Start timer
            timerInterval = setInterval(updateTimer, 1000);

            // Change button colors after 40th item
            if (totalAnswered >= 40) {
                document.getElementById('newGameBtnEnd').style.backgroundColor = 'green';
                document.getElementById('exitBtnEnd').style.backgroundColor = 'gold';
            }
        }

        function exitGame() {
            // Hide game container and display end game container
            document.getElementById('gameContainer').style.display = 'none';
            document.getElementById('endGameContainer').style.display = 'block';
            document.getElementById('endGameMessage').textContent = 'Thanks for playing!';
        }

        // Initial setup
        startNewGame();
    </script>
</body>
</html>
