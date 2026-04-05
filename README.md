<!DOCTYPE html><html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>King Cypha VIP Pro</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet"><style>
*{margin:0;padding:0;box-sizing:border-box}
body{
 font-family:'Poppins',sans-serif;
 background:linear-gradient(135deg,#020617,#0f172a);
 color:white;
}
header{
 text-align:center;
 padding:20px;
 background:#020617;
 border-bottom:1px solid #1e293b;
}
header h1{font-size:22px}
header p{color:#94a3b8;font-size:13px}
nav{
 display:flex;
 justify-content:space-around;
 padding:12px;
 background:#020617;
 border-bottom:1px solid #1e293b;
}
nav a{color:#94a3b8;text-decoration:none;font-size:14px}
nav a:hover{color:white}
.container{padding:20px}
.card{
 background:#1e293b;
 padding:18px;
 margin-bottom:15px;
 border-radius:15px;
 box-shadow:0 5px 15px rgba(0,0,0,0.3);
 animation:fadeIn 0.6s ease;
}
@keyframes fadeIn{
 from{opacity:0;transform:translateY(10px)}
 to{opacity:1;transform:translateY(0)}
}
input{
 width:100%;
 padding:10px;
 border:none;
 border-radius:8px;
 margin-top:10px;
}
button{
 width:100%;
 padding:12px;
 margin-top:10px;
 border:none;
 border-radius:8px;
 font-weight:bold;
 cursor:pointer;
}
.primary{background:#22c55e;color:white}
.whatsapp{background:#25D366;color:white}
.vip{background:#f59e0b;color:black}
button:hover{opacity:0.9}
.hidden{display:none}
#vipContent{display:none}
.badge{
 display:inline-block;
 padding:4px 10px;
 background:#22c55e;
 border-radius:20px;
 font-size:11px;
 margin-bottom:8px;
}
.urgency{
 color:#f87171;
 font-size:12px;
 margin-top:5px;
}
</style></head><body><header>
<h1>👑 KING CYPHA VIP PRO</h1>
<p>Smart Hacks • Make Money • Exclusive Secrets</p>
</header><nav>
<a href="#">Home</a>
<a href="#">Free</a>
<a href="#">VIP</a>
</nav><div class="container"><!-- HOOK SECTION --><div class="card">
<span class="badge">🔥 TRENDING</span>
<h2>⚠️ You’re using your phone wrong…</h2>
<p>I started making money using only my phone 😳💰</p>
<p class="urgency">Only serious people should continue...</p>
</div><!-- AUTH --><div class="card" id="authBox">
<h2>🔐Register</h2>
<input type="text" id="Fist name/Middle name/Last name" placeholder="First name/Middle name/Last name">
<input type="text" id="username" placeholder="Username">
<input type="password" id="password" placeholder="Password">
<input type="email" id="email" placeholder="Email">
<button class="primary" onclick="register()">Register</button>
<h2>🔑Login</h2>
<input type="text" id="username" placeholder="Username">
<input type="password" id="password" placeholder="Password">
<button class="primary" onclick="login()">Login</button>
</div><!-- FREE CONTENT --><div class="card hidden" id="mainContent">
<h2>💡 Free Tips</h2>
<p>✔ Use WhatsApp to store business ideas</p>
<p>✔ Share links and earn commissions</p>
<p>✔ Turn your phone into income tool</p>
</div><!-- ENGAGEMENT --><div class="card">
<h3>Do you want to learn this? 🤔</h3>
<button onclick="engage('YES')" class="primary">YES</button>
<button onclick="engage('NO')" class="vip">NO</button>
</div><!-- VIP --><div class="card hidden" id="vipBox">
<h2>🔒 VIP Access</h2>
<p>Unlock full money-making system 🔥</p>
<input type="password" id="vipPassword" placeholder="Enter VIP Code">
<button class="vip" onclick="unlockVIP()">Unlock VIP</button>
<p class="urgency">⚠️ Limited VIP slots available</p>
</div><div id="vipContent" class="card">
<h2>🔥 VIP Content</h2>
<p>✔ Step-by-step money guide</p>
<p>✔ WhatsApp earning secrets</p>
<p>✔ Hidden online income methods</p>
</div><!-- PAYMENT --><div class="card hidden" id="paymentBox">
<h2>💳 Payment</h2>
<p>Send MoMo to: <b>0595814126</b></p>
<p>After payment, click below 👇</p>
<button class="whatsapp" onclick="contactWhatsApp()">Contact on WhatsApp</button>
</div></div><script>
function register(){
 let u=username.value;
 let p=password.value;
 let e=email.value
 if(u && p && e){localStorage.setItem(u,p,e);alert('Registered! Login now');}
}

function login(){
 let u=username.value;
 let p=password.value;
 let e=email.value;
 if(localStorage.getItem(u)===p===e){
  alert('Welcome back 🔥');
  authBox.classList.add('hidden');
  mainContent.classList.remove('hidden');
  vipBox.classList.remove('hidden');
  paymentBox.classList.remove('hidden');
 }else{alert('Wrong login');}
}

function unlockVIP(){
 let code=vipPassword.value;
 if(code==='KING123'){
  vipContent.style.display='block';
  alert('VIP Unlocked 🔥');
 }else{alert('Wrong VIP Code');}
}

function contactWhatsApp(){
 let num='233595814126';
 let msg='Hello, I have paid for VIP. Please send my code.';
 window.open(`https://wa.me/${num}?text=${encodeURIComponent(msg)}`,'_blank');
}

function engage(ans){
 alert('You selected '+ans+' 🔥 Continue below');
}
</script></body>
</html>
