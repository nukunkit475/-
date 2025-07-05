<head>
  <style>
    body {
      margin: 0;
      padding: 0;
      background: linear-gradient(#fff5e6, #ffd6e0);
      font-family: 'Sriracha', cursive;
      text-align: center;
      color: #b03e65;
      overflow-x: hidden;
      min-height: 100vh;
    }
    h1 {
      font-size: 3em;
      margin-top: 250px;
      color: #d63384;
    }
    p {
      font-size: 1em;
      padding: 0 20px;
      line-height: 1.8;
    }
    .sticker {
      margin: 20px auto;
      width: 300px;
      border-radius: 20px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    }
    button {
      margin-top: 30px;
      padding: 10px 25px;
      font-size: 1em;
      background: #ffa6c9;
      border: none;
      border-radius: 15px;
      color: white;
      cursor: pointer;
      transition: 0.3s;
    }
    button:hover {
      background: #ff7fbf;
    }
    #secret {
      display: none;
      margin-top: 20px;
      font-size: 1.4em;
      color: #6f42c1;
    }

    /* floating hearts */
    .heart {
      position: absolute;
      width: 20px;
      height: 20px;
      background: red;
      transform: rotate(45deg);
      animation: float 5s infinite;
      opacity: 0.8;
    }
    .heart::before,
    .heart::after {
      content: "";
      position: absolute;
      width: 20px;
      height: 20px;
      background: red;
      border-radius: 50%;
    }
    .heart::before {
      top: -10px;
      left: 0;
    }
    .heart::after {
      top: 0;
      left: -10px;
    }
    @keyframes float {
      0% { transform: translateY(0) rotate(45deg); opacity: 1; }
      100% { transform: translateY(-800px) rotate(45deg); opacity: 0; }
    }
  </style>
</head>
<body>

  <h1>🎂🎉</h1>


  <button onclick="document.getElementById('secret').style.display='block'">
   กดได้นะครับ👆
  </button>
  <div id="secret">
  <p>วันเกิดปีนี้ผมอยากจะบอกว่า</p>
  <img class="sticker" src="put-your-image-link-here.png" alt="หารูปก่อนใจเย็น">
  <p>ผมอยากให้พี่สมหวัง<br>
     กับทุกสิ่งที่พี่ปรารถนา</p>
  <img class="sticker" src="put-your-image-link-here.png" alt="หารูปก่อนใจเย็น">
  <p>ไม่อยากให้มีเรื่องทุกข์ใจ</p>
  <img class="sticker" src="put-your-image-link-here.png" alt="หารูปก่อนใจเย็น"> 
  <p>อยากให้มีความสุข</p>
  <img class="sticker" src="put-your-image-link-here.png" alt="หารูปก่อนใจเย็น"> 
  <p>และใกล้สุดท้าย</p>
  <img class="sticker" src="put-your-image-link-here.png" alt="หารูปก่อนใจเย็น"> 
  <p>อยากให้ยิ้มเยอะๆ</p>
  <img class="sticker" src="put-your-image-link-here.png" alt="หารูปก่อนใจเย็น"> 
  <p>สุดท้ายละครับ</p>
  <img class="sticker" src="put-your-image-link-here.png" alt="หารูปก่อนใจเย็น"> 
  <p>ขอคุณที่ยังอยู่ด้วยกันครับ</p>
  <img class="sticker" src="put-your-image-link-here.png" alt="หารูปก่อนใจเย็น"> 
  </div>

 <script>
    for (let i = 0; i < 25; i++) {
      let heart = document.createElement("div");
      heart.className = "heart";
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.animationDuration = 3 + Math.random() * 2 + "s";
      document.body.appendChild(heart);
    }
  </script>

</body>
