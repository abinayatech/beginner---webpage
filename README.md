<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>FOSS PROJECT</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      margin: 0;
      padding: 0;
      background: linear-gradient(-45deg, #e3f2fd, #cfd8dc, #e1bee7, #bbdefb);
      background-size: 400% 400%;
      animation: bgAnimation 10s ease infinite;
    }

    header {
      background: #35424a;
      color: #fff;
      padding: 40px 0;
      text-align: center;
    }

    header h1 {
      font-size: 2.5rem;
      white-space: nowrap;
      overflow: hidden;
      border-right: 3px solid #ffffff;
      width: 0;
      animation: typing 4s steps(30, end) forwards, blink 0.7s step-end infinite;
    }

    main {
      padding: 30px;
      animation: fadeIn 1.2s ease-in;
    }

    h2 {
      color: #333;
      margin-top: 20px;
    }

    ul {
      padding-left: 20px;
    }

    li {
      margin-bottom: 8px;
    }

    .input-field {
      padding: 10px;
      margin: 10px 0;
      width: 250px;
      border: 1px solid #ccc;
      border-radius: 5px;
      display: block;
      margin-left: auto;
      margin-right: auto;
    }

    .button {
      background-color: #35424a;
      color: #fff;
      border: none;
      padding: 10px 20px;
      border-radius: 25px;
      cursor: pointer;
      display: block;
      margin: 10px auto;
      font-weight: bold;
      box-shadow: 0 0 10px #35424a;
      transition: all 0.3s ease-in-out;
      animation: bounce 2s infinite;
    }

    .button:hover {
      background-color: #1a1a1a;
      box-shadow: 0 0 15px #00e676;
      transform: scale(1.05);
    }

    #message {
      text-align: center;
      font-weight: bold;
      margin-top: 10px;
    }

    footer {
      text-align: center;
      padding: 15px 0;
      background: #35424a;
      color: #ffffff;
      position: relative;
      bottom: 0;
      width: 100%;
      margin-top: 40px;
    }

    /* Advanced Animations */
    @keyframes typing {
      from { width: 0; }
      to { width: 100%; }
    }

    @keyframes blink {
      50% { border-color: transparent; }
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: scale(0.95); }
      to { opacity: 1; transform: scale(1); }
    }

    @keyframes bounce {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-5px); }
    }

    @keyframes bgAnimation {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }
  </style>
</head>
<body>

  <header>
    <h1>Welcome to My FOSS Project</h1>
  </header>

  <main>
    <h2>About This Page</h2>
    <p>This page provides resources for learning web development using HTML, CSS, and JavaScript.</p>

    <h2>Skills</h2>
    <ul>
      <li>HTML</li>
      <li>CSS</li>
      <li>JavaScript</li>
      <li>Practical Knowledge</li>
    </ul>

    <h2>Contact Me</h2>
    <p>If you have any queries, feel free to contact me at <a href="mailto:example@example.com">example@example.com</a>.</p>

    <h2>KNOWLEDGE IS POWER! 💡</h2>

    <h2>Login</h2>
    <input type="text" id="username" class="input-field" placeholder="Enter your Username" />
    <input type="password" id="password" class="input-field" placeholder="Enter your Password" />
    <button class="button" onclick="login()">Login</button>
    <p id="message"></p>
  </main>

  <footer>
    &copy; 2025 Abinaya S | FOSS Project
  </footer>

  <script>
    function login() {
      const username = document.getElementById("username").value;
      const password = document.getElementById("password").value;
      const message = document.getElementById("message");

      if (username && password) {
        message.style.color = "green";
        message.textContent = "Login successful! ✨";
      } else {
        message.style.color = "red";
        message.textContent = "Please enter both username and password.";
      }
    }
  </script>

</body>
</html>
