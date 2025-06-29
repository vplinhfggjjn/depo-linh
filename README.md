
<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Liên hệ - Trường Đại học Chí Đức</title>
  <style>
    body {
      padding: 20px;
      text-align: left;
    }

    .text-block p {
      margin: 5px 0 0 0;
      font-size: 1.3em;
      color: midnightblue;
    }

    .logo-row {
      display: flex;
      align-items: center;
      gap: 20px;
      padding: 20px;
    }

    .logo-img {
      width: 150px;
      height: 150px;
      flex-shrink: 0;
    }

    .text-block {
      flex: 1;
    }

    .text-block h1 {
      margin: 0;
      font-size: 2.5em;
      color: midnightblue;
    }

    .slogan-lang {
      display: flex;
      justify-content: space-between;
      align-items: center;
      width: 100%;
      box-sizing: border-box;
    }

    .slogan-lang p {
      margin: 0;
      font-size: 1.3em;
      color: midnightblue;
    }
    nav {
      background-color: midnightblue;
      padding: 10 20px;
      display: flex;
      justify-content: space-evenly;
    }
    nav a {
      color: #ffffff;
      text-decoration: none;
      font-size: 20px;
      transition: color 0.3s;
    }
    nav a:hover {
      color: #888;
    }
    .intro {
      background-color: #ffffff;
      color: midnightblue;
      text-align: center;
      padding: 40px;
      font-size: 22px;
      animation: slide 10s linear infinite;
    }
    @keyframes slide {
      0% { letter-spacing: 1px; }
      50% { letter-spacing: 4px; }
      100% { letter-spacing: 1px; }
    }
    .contact-section {
      display: flex;
      justify-content: center;
      align-items: flex-start;
      padding: 20px;
      gap: 20px;
    }
    .map img {
      width: 100%;
      max-width: 900px;
      border: 1px solid #ccc;
    }
    .branches {
      background-color: #f0f0f0;
      padding: 35px;
      border-radius: 6px;
      width: 70%;
      max-width: 400px;
    }
    .branches input {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border: 1px solid #ccc;
    }
    .branches button {
      background-color: #ff9933;
      border: none;
      padding: 10px 20px;
      cursor: pointer;
      color: white;
      transition: background 0.3s;
      border-radius: 20px;
    }
    .branches button:hover {
      background-color: #888;
    }
    .contact-form-section {
      padding: 20px;
      background-color: #f0f0f0;
      text-align: center;
    }
    .contact-info {
      margin-bottom: 20px;
    }
    form input, form textarea {
      display: block;
      width: 80%;
      max-width: 500px;
      margin: 10px auto;
      padding: 10px;
      border: 1px solid #ccc;
    }
    .submit-button {
      background-color: #ff9933;
      color: white;
      padding: 10px 20px;
      border: none;
      cursor: pointer;
      border-radius: 20px;
    }
    .submit-button:hover {
      background-color: #888;
    }
footer {
  background-color:midnightblue;
  padding: 20px 40px;
  border-top: 1px solid #ccc;
  font-size: 0.95em;
  color:#ccc;
}

.footer-container {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}

.footer-left {
  text-align: left;
}

.footer-right {
  text-align: right;
    }
    .fixed-icons {
      position: fixed;
      bottom: 20px;
      right: 20px;
      display: flex;
      flex-direction: column;
      gap: 10px;
      z-index: 999;
    }
    .fixed-icons img {
      width: 40px;
      height: 40px;
      cursor: pointer;
      animation: pulse 2s infinite;
      border-radius: 50%;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.2);
    }
    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.1); }
      100% { transform: scale(1); }
    }
  </style>
</head>
<body>
  <header>
  <div class="logo-row">
      <img src="https://demo-web-iota.vercel.app/assest/logo-removebg-preview.png" alt="Logo" class="logo-img">
  <div class="text-block">
      <h1 id="title">TRƯỜNG ĐẠI HỌC CHÍ ĐỨC</h1>
      <div class="slogan-lang">
        <p id="slogan">Kiến thức vững vàng - Đạo đức trọn vẹn</p>
      </div>
    </div>
  </div>
</header>

<nav>
  <a href="#">Trang chủ</a>
  <a href="#">Trợ giúp</a>
  <a href="#">Thêm</a>
  <a href="login.html">Đăng nhập</a>
  <a href="register.html">Đăng ký</a>
</nav>
  <header>

  <div class="intro">
    Liên hệ (Contact) để đội ngũ chúng tôi tư vấn cho bạn
  </div>

  <section class="contact-section">
    <div class="map">
      <img src="https://www.umt.edu.vn/vi-vn/images/resize-770x0/upload/media/M63b391f5b767c/du-hoc-la-gi.png?v=1.31" alt="Hình ảnh trường">
    </div>
    <div class="branches">
      <h3>Tra cứu chi nhánh</h3>
      <input type="text" placeholder="Nhập tên chi nhánh...">
      <button><span>&#128269;</span> Tìm kiếm</button>
      <div class="contact-info">
        <p><strong>Hotline:</strong> 0912111822</p>
        <p><strong>Email:</strong> cdu@edu.vn</p>
      </div>
    </div>
  </section>

  <section class="contact-form-section">
    <div class="contact-info">
      <strong>Liên hệ với chúng tôi</strong><br />
    </div>
    <form onsubmit="return submitForm(event)">
      <input type="text" placeholder="Họ và tên" id="name" required />
      <input type="email" placeholder="Email" id="email" required />
      <textarea rows="4" placeholder="Nội dung" id="message" required></textarea>
      <button class="submit-button">Gửi liên hệ</button>
    </form>
    <p id="result"></p>
  </section>

  <footer>
        <div class="footer-container">
            <div class="footer-left">
                <p>Trụ sở chính:</p>
                <p>70 Nguyễn Quang, Phường 13, Quận Tân Bình, TP.HCM</p>
            </div>
            <div class="footer-right">
                <p>Hotline: 0912111822</p>
                <p>Email: cdu@edu.vn</p>
            </div>
        </div>
  </footer>

  <div class="fixed-icons">
    <img src="https://png.pngtree.com/element_our/20200702/ourlarge/pngtree-vector-phone-sign-image_2289768.jpg" alt="Gọi điện">
    <img src="https://png.pngtree.com/png-clipart/20190613/original/pngtree-information-icon-png-image_3581490.jpg" alt="Thông tin">
  </div>

  <script>
    function submitForm(event) {
      event.preventDefault();
      const name = document.getElementById("name").value;
      const email = document.getElementById("email").value;
      const message = document.getElementById("message").value;
      const result = document.getElementById("result");
      if (name && email && message) {
        result.style.color = 'green';
        result.textContent = "Liên hệ thành công!";
      } else {
        result.style.color = 'red';
        result.textContent = "Vui lòng điền đầy đủ thông tin.";
      }
    }
  </script>
</body>
</html>

