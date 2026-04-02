<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Login Form Cute</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
<style>
  * { margin:0; padding:0; box-sizing:border-box; font-family:'Poppins', sans-serif; }
  body {
    height:100vh;
    background: linear-gradient(135deg, #f98da7, #ffe26e);
    display:flex;
    justify-content:center;
    align-items:center;
  }
  .login-card {
    background:#fff;
    display:flex;
    border-radius:15px;
    box-shadow: 0 10px 30px rgba(0,0,0,0.1);
    overflow:hidden;
    max-width:800px;
    width:90%;
  }
  .login-card .left {
    width:50%;
    background:url('https://images.unsplash.com/photo-1604908177523-6fdf1f47c9a1?auto=format&fit=crop&w=600&q=80') center/cover no-repeat;
  }
  .login-card .right {
    width:50%;
    padding:40px;
    display:flex;
    flex-direction:column;
    justify-content:center;
  }
  .login-card h2 {
    font-weight:600;
    font-size:28px;
    color:#ff4d4d;
    margin-bottom:30px;
    white-space:nowrap;
    overflow:hidden;
    border-right:3px solid #ff4d4d;
    width:0;
    animation: typing 2s steps(20) forwards, blink .75s step-end infinite;
  }
  @keyframes typing {
    from { width:0; }
    to { width: 120px; } /* adjust based on text length */
  }
  @keyframes blink {
    50% { border-color: transparent; }
  }
  .login-card input {
    margin-bottom:20px;
    padding:12px 15px 12px 40px;
    border:1px solid #ff4d4d;
    border-radius:25px;
    width:100%;
    outline:none;
    font-size:16px;
  }
  .login-card input::placeholder { color:#ff7f7f; }
  .login-card .icon { position:absolute; margin-left:12px; color:#ff4d4d; }
  .login-card .btn {
    padding:12px;
    border:none;
    border-radius:25px;
    cursor:pointer;
    font-weight:600;
    font-size:16px;
    margin-bottom:15px;
  }
  .login-card .login-btn { background:#ff4d4d; color:#fff; }
  .login-card .register-btn { background:#ccc; color:#333; }
  .login-card .links { font-size:14px; color:#ff4d4d; display:flex; justify-content:space-between; margin-bottom:15px; }
</style>
</head>
<body>
  <div class="login-card">
    <div class="left"></div>
    <div class="right">
      <h2>Login</h2>
      <div style="position:relative;">
        <span class="icon">👤</span>
        <input type="email" placeholder="Email">
      </div>
      <div style="position:relative;">
        <span class="icon">🔒</span>
        <input type="password" placeholder="Password">
      </div>
      <div class="links">
        <a href="#">forget password?</a>
        <a href="#">change password</a>
      </div>
      <button class="btn login-btn">Login</button>
      <button class="btn register-btn">Register</button>
    </div>
  </div>
</body>
</html>
