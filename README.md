
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#080d20">
<title>شات مساعد حقيقي</title>
<style>
*{box-sizing:border-box}
body{margin:0;background:#080d20;color:#fff;font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",sans-serif;min-height:100vh}
header{padding:22px 18px;border-bottom:1px solid #26345f;display:flex;align-items:center;gap:12px}
.logo{width:48px;height:48px;border-radius:16px;background:linear-gradient(135deg,#176cff,#853cff);display:grid;place-items:center;font-size:27px;box-shadow:0 0 22px #345dff66}
.brand{font-size:19px;font-weight:800}
.sub{font-size:12px;color:#9daed5;margin-top:4px}
main{max-width:700px;margin:auto;padding:24px 17px 120px}
.hero{text-align:center;margin:30px 0}
.robot{font-size:76px;filter:drop-shadow(0 0 20px #397bff)}
h1{font-size:29px;margin:10px 0;background:linear-gradient(90deg,#49d8ff,#a77aff);background-clip:text;color:transparent}
.hero p{color:#aab7d6;line-height:1.8}
.grid{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin:25px 0}
.tile{background:#111c39;border:1px solid #293d70;border-radius:17px;padding:17px 12px;text-align:center;color:#e8edff;font-size:14px;line-height:1.8}
.tile span{display:block;font-size:25px;margin-bottom:5px}
.chat{background:#101a35;border:1px solid #344a83;border-radius:20px;padding:16px;margin-top:25px;min-height:180px}
.message{line-height:1.9;color:#e5eaff;white-space:pre-wrap}
#messages{display:flex;flex-direction:column;gap:14px}
.user{background:#263b70;padding:12px 15px;border-radius:16px 16px 4px 16px;align-self:flex-start;max-width:90%;line-height:1.8}
.bot{background:#172443;padding:12px 15px;border-radius:16px 16px 16px 4px;align-self:flex-end;max-width:95%;line-height:1.8}
.inputbar{position:fixed;bottom:0;left:0;right:0;padding:12px;background:#080d20ee;border-top:1px solid #26345f;display:flex;gap:9px}
.inputbar input{flex:1;min-width:0;background:#121e3b;border:1px solid #40558c;border-radius:25px;padding:15px;color:white;font-size:15px;outline:none}
button{border:0;border-radius:50%;width:52px;background:linear-gradient(135deg,#287cff,#843dff);color:white;font-size:22px}
.note{text-align:center;color:#8796ba;font-size:11px;margin-top:17px}
</style>
</head>
<body>
<header>
<div class="logo">🤖</div>
<div><div class="brand">شات مساعد حقيقي</div><div class="sub">مساعدك الذكي في كل شيء 💙</div></div>
</header>
<main>
<section class="hero">
<div class="robot">🤖</div>
<h1>مرحباً بك!</h1>
<p>اسأل، اكتشف، تعلم، وابدأ رحلتك مع مساعدك الذكي.</p>
</section>
<div class="grid">
<div class="tile"><span>💻</span>اكتب الأكواد واشرحها</div>
<div class="tile"><span>🎓</span>ساعدني في الدراسة</div>
<div class="tile"><span>🔎</span>ابحث عن المعلومات</div>
<div class="tile"><span>📄</span>ساعدني في الملفات</div>
</div>
<section class="chat">
<div id="messages">
<div class="bot">أهلاً بك! 👋 أنا شات مساعد حقيقي. كيف أقدر أساعدك اليوم؟</div>
</div>
<div class="note">الإصدار الأول · سيتم ربط الذكاء الاصطناعي لاحقاً</div>
</section>
</main>
<div class="inputbar">
<input id="prompt" placeholder="اكتب رسالتك هنا..." autocomplete="off">
<button onclick="send()" aria-label="إرسال">➤</button>
</div>
<script>
function send(){
 const input=document.getElementById('prompt');
 const value=input.value.trim();
 if(!value)return;
 const messages=document.getElementById('messages');
 const user=document.createElement('div');
 user.className='user';user.textContent=value;
 messages.appendChild(user);
 const bot=document.createElement('div');
 bot.className='bot';
 bot.textContent='وصلت رسالتك! 💙 هذه نسخة تجريبية من الموقع. سنربط محرك الذكاء الاصطناعي في الخطوة القادمة.';
 messages.appendChild(bot);
 input.value='';
 window.scrollTo({top:document.body.scrollHeight,behavior:'smooth'});
}
document.getElementById('prompt').addEventListener('keydown',e=>{
 if(e.key==='Enter')send();
});
</script>
</body>
</html>
# chat-mosaed-haqiqii