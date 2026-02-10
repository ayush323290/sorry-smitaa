<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>For You ❤️</title>
  <style>
    body {
      background: linear-gradient(to right, #ff758c, #ff7eb3);
      font-family: Arial, sans-serif;
      text-align: center;
      color: white;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .card {
      background: rgba(0,0,0,0.25);
      padding: 25px;
      border-radius: 20px;
      width: 340px;
    }

    img {
      width: 100%;
      border-radius: 15px;
      margin: 10px 0;
    }

    button {
      padding: 10px 20px;
      margin: 10px;
      font-size: 16px;
      border: none;
      border-radius: 20px;
      cursor: pointer;
    }

    #yesBtn {
      background: #00e676;
      color: black;
    }

    #noBtn {
      background: #ff1744;
      color: white;
      position: relative;
    }
  </style>
</head>
<body>

<div class="card" id="content">
  <h1>Hey ❤️</h1>

  <!-- Cute intro GIF -->
  <img src="https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExZDV6cWY5ZDY4c3N4empudThkNXNlancyeTBvb3RrZDRkbDQ2Zm9mOCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/iseq9MQgxo4aQ/giphy.gif" alt="cute gif">

  <p>
    I might not be perfect,  
    but my feelings for you are real.  
    We are bestfriends i know but we know eachother very well.
    It will help us to be more than bestfriends.
        I want to be with you and make you happy.  
        Will you give us a chance? 🥺
  </p>

  <p>Would you like to be with me? 🥺</p>

  <button id="yesBtn" onclick="yesClicked()">Yes 💖</button>
  <button id="noBtn" onmouseover="moveButton()">No 💔</button>
</div>

<script>
  function yesClicked() {
    document.getElementById("content").innerHTML = `
      <h1>YAAAY 🥹❤️</h1>

      <!-- Celebration GIF -->
      <img src="https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExMnJmcXY1MGh5Z3lteHBuMjltZXZnZjdlbnV5MTlycG50N2Z5Y3gyayZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/14hm2SwqjG5pkI/giphy.gif" alt="happy gif">

      <p>
        You just made me the happiest person ever.  
        I promise to respect you, care for you,  
        and always be honest with my feelings.
        I can’t wait to create amazing memories together and make you smile every day.
        I will always love you and cherish every moment we share.
      </p>

      <p>❤️ Forever grateful ❤️</p>
    `;
  }

  function moveButton() {
    const btn = document.getElementById("noBtn");
    const x = Math.floor(Math.random() * 120) - 60;
    const y = Math.floor(Math.random() * 120) - 60;
    btn.style.transform = `translate(${x}px, ${y}px)`;
  }
</script>

</body>
</html>
