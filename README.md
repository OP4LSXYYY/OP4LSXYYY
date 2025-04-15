<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>For My Love</title>
  <link href="https://fonts.googleapis.com/css2?family=Itim&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Itim', cursive;
      background: linear-gradient(to right, #ffecd2, #fcb69f);
      text-align: center;
      padding: 50px;
      color: #444;
    }

    h1 {
      font-size: 3em;
      color: #ff69b4;
      margin-bottom: 20px;
    }

    p {
      font-size: 1.3em;
      margin-bottom: 30px;
    }

    button {
      background-color: #ff8fab;
      border: none;
      padding: 15px 30px;
      font-size: 1.2em;
      border-radius: 30px;
      color: white;
      cursor: pointer;
      transition: 0.3s;
    }

    button:hover {
      background-color: #f06292;
    }

    .popup {
      display: none;
      position: fixed;
      background-color: white;
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.2);
      width: 80%;
      max-width: 300px;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      z-index: 1000;
    }

    .overlay {
      display: none;
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background-color: rgba(0, 0, 0, 0.3);
      z-index: 999;
    }
  </style>
</head>
<body>

  <h1>สวัสดีที่รักของเค้า</h1>
  <p>มีบางอย่างอยากบอกนะ… กดปุ่มข้างล่างสิ!</p>

  <button onclick="showPopup()">คลิกดูความลับ</button>

  <div class="overlay" id="overlay" onclick="hidePopup()"></div>
  <div class="popup" id="popup">
    <h2>รักเธอนะ!</h2>
    <p>ขอบคุณที่อยู่ด้วยกันในทุกวัน <br> เธอคือคนพิเศษที่สุดของเราเลย</p>
    <button onclick="hidePopup()">ปิด</button>
  </div>

  <script>
    function showPopup() {
      document.getElementById('popup').style.display = 'block';
      document.getElementById('overlay').style.display = 'block';
    }

    function hidePopup() {
      document.getElementById('popup').style.display = 'none';
      document.getElementById('overlay').style.display = 'none';
    }
  </script>

</body>
</html>
