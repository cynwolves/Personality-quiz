<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Personality Snapshot Quiz</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      padding: 40px;
      background-color: #f9f9f9;
      max-width: 700px;
      margin: auto;
    }
    h1 {
      text-align: center;
    }
    .question {
      margin-bottom: 25px;
    }
    label {
      display: block;
      margin: 6px 0;
    }
    button {
      margin-top: 20px;
      padding: 10px 15px;
      font-size: 16px;
    }
    #result {
      margin-top: 30px;
      font-size: 20px;
      font-weight: bold;
      color: #2b2b2b;
      padding: 20px;
      background-color: #e4f0e2;
      border-left: 6px solid #4caf50;
    }
  </style>
</head>
<body>
  <h1>🧠 Personality Snapshot Quiz</h1>
  <form id="quizForm">
    <div class="question">
      <strong>1. How often do you reflect on your actions?</strong><br>
      <label><input type="radio" name="q1" value="3"> A. Daily</label>
      <label><input type="radio" name="q1" value="2"> B. Occasionally</label>
      <label><input type="radio" name="q1" value="1"> C. Rarely</label>
    </div>

    <div class="question">
      <strong>2. When you promise something, how likely are you to follow through?</strong><br>
      <label><input type="radio" name="q2" value="3"> A. Always</label>
      <label><input type="radio" name="q2" value="2"> B. Most of the time</label>
      <label><input type="radio" name="q2" value="1"> C. Depends on the situation</label>
    </div>

    <div class="question">
      <strong>3. Do you believe people are inherently good?</strong><br>
      <label><input type="radio" name="q3" value="3"> A. Yes</label>
      <label><input type="radio" name="q3" value="2"> B. Somewhat</label>
      <label><input type="radio" name="q3" value="1"> C. Not really</label>
    </div>

    <div class="question">
      <strong>4. Have you ever cheated on a current partner?</strong><br>
      <label><input type="radio" name="q4" value="yes"> A. Yes</label>
      <label><input type="radio" name="q4" value="no"> B. No</label>
    </div>

    <div class="question">
      <strong>5. Are you open to feedback, even if it's hard to hear?</strong><br>
      <label><input type="radio" name="q5" value="3"> A. Yes, I welcome it</label>
      <label><input type="radio" name="q5" value="2"> B. Sometimes</label>
      <label><input type="radio" name="q5" value="1"> C. I usually get defensive</label>
    </div>

    <div class="question">
      <strong>6. How do you handle guilt?</strong><br>
      <label><input type="radio" name="q6" value="3"> A. I confront it and try to make things right</label>
      <label><input type="radio" name="q6" value="2"> B. I try to move on</label>
      <label><input type="radio" name="q6" value="1"> C. I ignore it</label>
    </div>

    <div class="question">
      <strong>7. Do you lie to avoid conflict?</strong><br>
      <label><input type="radio" name="q7" value="3"> A. No</label>
      <label><input type="radio" name="q7" value="2"> B. Occasionally</label>
      <label><input type="radio" name="q7" value="1"> C. Frequently</label>
    </div>

    <div class="question">
      <strong>8. When faced with temptation, you are:</strong><br>
      <label><input type="radio" name="q8" value="3"> A. Strong and grounded</label>
      <label><input type="radio" name="q8" value="2"> B. It depends on the situation</label>
      <label><input type="radio" name="q8" value="1"> C. Easily swayed</label>
    </div>

    <div class="question">
      <strong>9. How would your closest friend describe your integrity?</strong><br>
      <label><input type="radio" name="q9" value="3"> A. Solid and trustworthy</label>
      <label><input type="radio" name="q9" value="2"> B. Mostly reliable</label>
      <label><input type="radio" name="q9" value="1"> C. Unpredictable</label>
    </div>

    <div class="question">
      <strong>10. Do you take responsibility when you hurt someone?</strong><br>
      <label><input type="radio" name="q10" value="3"> A. Yes, always</label>
      <label><input type="radio" name="q10" value="2"> B. Sometimes</label>
      <label><input type="radio" name="q10" value="1"> C. Not really</label>
    </div>

    <button type="button" onclick="calculateScore()">Submit</button>
  </form>

  <div id="result"></div>

  <script>
    function calculateScore() {
      const form = document.forms["quizForm"];
      const resultDiv = document.getElementById("result");
      let totalScore = 0;
      let cheated = false;

      for (let i = 1; i <= 10; i++) {
        const q = form["q" + i];
        if (!q.value) {
          alert("Please answer all questions.");
          return;
        }
        if (i === 4 && q.value === "yes") {
          cheated = true;
        } else if (i !== 4) {
          totalScore += parseInt(q.value);
        }
      }

      if (cheated) {
        resultDiv.innerHTML = "👉 Your final score is <strong>19 out of 30</strong>";
      } else {
        resultDiv.innerHTML = "👉 Your final score is <strong>" + totalScore + " out of 30</strong>";
      }
    }
  </script>
</body>
</html>
