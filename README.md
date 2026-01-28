#<!DOCTYPE html>
<html>
<head>
  <title>Secret Premium Apps</title>
  <style>
    body { font-family: Arial; background:#111; color:#fff; text-align:center; padding-top:50px; }
    input, button { padding:10px 15px; margin:10px; font-size:16px; }
    a { display:block; padding:12px 20px; background:#00ff99; color:#000; text-decoration:none; font-weight:bold; margin:10px auto; width:250px; border-radius:5px; }
    #dashboard { display:none; }
    h2 { margin-bottom:20px; }
  </style>
</head>
<body>

<!-- LOGIN SECTION -->
<div id="login">
  <h2>Private Access Only 🔒</h2>
  <p>Enter your access key</p>
  <input type="password" id="key" placeholder="Access key">
  <br>
  <button onclick="login()">Enter</button>
</div>

<!-- DASHBOARD SECTION -->
<div id="dashboard">
  <h2>Welcome, Insider 👀</h2>
  <p>Select your app to download:</p>
  
  <!-- Free apps -->
  <h3>Free Apps</h3>
  
  <a href="https://play.google.com/store/apps/details?id=ch.protonvpn.android" target="_blank">
  <button>Proton VPN</button>
</a><br>
  <a href="https://en.softonic.com/download/capcut/android/post-download/v/16.3.0" target="_blank"><button>capcut</button></a><br>
  <a href="https://f-droid.org/packages/com.termux"><button>Termux</button></a><br>
  <a href="https://f-droid.org/" target="_blank"><button>F-droid(kali linux)</button></a><br>
  <a href="https://termux.en.softonic.com/android"><button>Termux</button></a><br>
  <a href=""><button>IR Blaster Remote</button></a><br>
  <a href="https://play.google.com/store/apps/details?id=com.openai.chatgpt"><button>Chat gpt</button></a><br>
  <a href="https://play.google.com/
    <a href="https://honista.com/en/" target="_blank"><button>Honista(instagram pro)</button></a><br>
  <a href="https://play.google.com/store/apps/details?id=com.foxdebug.acodefree"><button>Acode</button></a><br>
  <a href="https://play.google.com/store/apps/details?id=com.deepseek.chat"><button>Deepseek</button></a><br>
  <a href="https://android.izzysoft.de/repo/apk/org.elnix.dragonlauncher"><button>Dragon launcher</button></a><br>
  <a href="https://watchanimeworld.net/"><button>Free anime</button></a><
   <!-- Footer Info -->
  <footer style="margin-top:20px; font-size:14px; color:#aaa;">
    Siddharth Tiwari | Phone: <a href="tel:+918291988158">+91 8291988158</a> | Email: <a href="mailto:sidveil52@gmail.com">sidveil52@gmail.com</a> | Instagram: <a href="https://www.instagram.com/sidveil" target="_blank">@sidveil</a>
  </footer>
</section>
 
  
   <button onclick="logout()">Logout</button>
</div>

<script>
  // Check if already logged in
  if(localStorage.getItem("access") === "true") {
    showDashboard();
  }

  // LOGIN FUNCTION
  function login() {
    const key = document.getElementById("key").value;
    if(key === "SID") {  // Change this key
      localStorage.setItem("access","true");
      showDashboard();
    } else {
      alert("Access denied 🚫");
    }
  }

  // SHOW DASHBOARD
  function showDashboard() {
    document.getElementById("login").style.display = "none";
    document.getElementById("dashboard").style.display = "block";
  }

  // LOGOUT FUNCTION
  function logout() {
    localStorage.removeItem("access");
    document.getElementById("dashboard").style.display = "none";
    document.getElementById("login").style.display = "block";
  }
</script>
  
 
  <footer>©By SID 2026 </footer>
  <footer>Sidharth Tiwari</footer>
</body>
</html>
