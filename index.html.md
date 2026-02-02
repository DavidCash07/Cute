<!DOCTYPE html>  
<html lang="en">  
<head>  
  <meta charset="UTF-8">  
  <title>Be My Valentine 💘</title>  
  <style>  
    body {  
      height: 100vh;  
      margin: 0;  
      display: flex;  
      justify-content: center;  
      align-items: center;  
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);  
      font-family: 'Comic Sans MS', cursive;  
      overflow: hidden;  
    }  
  
    .card {  
      background: white;  
      padding: 40px;  
      border-radius: 20px;  
      text-align: center;  
      box-shadow: 0 10px 25px rgba(0,0,0,0.2);  
    }  
  
    h1 {  
      color: #ff4d6d;  
      margin-bottom: 30px;  
    }  
  
    button {  
      padding: 12px 30px;  
      font-size: 18px;  
      border: none;  
      border-radius: 30px;  
      cursor: pointer;  
      position: absolute;  
    }  
  
    #yes {  
      background: #ff4d6d;  
      color: white;  
      position: relative;  
      margin-right: 20px;  
    }  
  
    #no {  
      background: #ccc;  
      color: black;  
    }  
  </style>  
</head>  
<body>  
  
  <div class="card">  
    <h1>Will you be my Valentine? 💖</h1>  
    <button id="yes" onclick="yesClicked()">Yes 😍</button>  
    <button id="no">No 🙄</button>  
  </div>  
  
  <script>  
    const noBtn = document.getElementById("no");  
  
    noBtn.addEventListener("mouseover", () => {  
      const x = Math.random() * (window.innerWidth - noBtn.clientWidth);  
      const y = Math.random() * (window.innerHeight - noBtn.clientHeight);  
      noBtn.style.left = x + "px";  
      noBtn.style.top = y + "px";  
    });  
  
    function yesClicked() {  
      document.body.innerHTML = `  
        <div style="  
          display:flex;  
          justify-content:center;  
          align-items:center;  
          height:100vh;  
          background:linear-gradient(135deg,#ff9a9e,#fad0c4);  
          font-family:'Comic Sans MS',cursive;  
          text-align:center;  
        ">  
          <h1 style="color:#ff4d6d;">  
            Yayyy!!! 💕😍<br>  
            Best Valentine Ever 💖  
          </h1>  
        </div>  
      `;  
    }  
  </script>  
  
</body>  
</html>  
