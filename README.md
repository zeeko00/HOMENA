<!doctype html>
<html lang="ar" dir="rtl">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="theme-color" content="#961E1E">
<title>هومنا | Homena Group</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700;800&display=swap" rel="stylesheet">
<style>
:root{--red:#961E1E;--red-dark:#6E1414;--red-light:#B02A2A;--red-soft:#F8EEEE;--red-pale:#FFF8F8;--bg:#FAF8F8;--ink:#2A1A1A;--muted:#6B5A5A}
*{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--ink);font-family:'Cairo',Tahoma,Arial,sans-serif;-webkit-tap-highlight-color:transparent}
main{width:min(100% - 28px,520px);margin:18px auto 40px}

header{position:relative;overflow:hidden;background:linear-gradient(160deg,var(--red-dark),var(--red) 60%,var(--red-light));color:#fff;border-radius:28px;padding:38px 22px 34px;text-align:center}
header::before,header::after{content:"";position:absolute;border-radius:50%;border:1px solid rgba(255,255,255,.25);pointer-events:none}
header::before{width:260px;height:260px;top:-120px;left:-90px}
header::after{width:200px;height:200px;bottom:-110px;right:-60px;border-color:rgba(255,255,255,.18)}
.logo{position:relative;display:block;width:min(74%,250px);height:auto;margin:0 auto}
header p{position:relative;margin:14px 0 0;font-size:20px;font-weight:800;line-height:1.7;color:#fff}
header .subline{margin:3px 0 0;font-size:14px;font-weight:600;line-height:1.7;color:rgba(255,255,255,.9)}
.pill{position:relative;display:block;width:46px;height:5px;border-radius:3px;background:var(--red-light);margin:16px auto 0}

section{background:#fff;border-radius:22px;padding:18px;margin-top:14px;box-shadow:0 1px 0 rgba(150,30,30,.05),0 8px 24px -18px rgba(110,20,20,.35)}
h2{display:flex;align-items:center;gap:10px;font-size:17px;font-weight:800;color:var(--red);margin:0 0 14px}
h2::before{content:"";width:6px;height:20px;border-radius:3px;background:var(--red-light)}

.ic{width:22px;height:22px;flex:none;fill:none;stroke:currentColor;stroke-width:1.8;stroke-linecap:round;stroke-linejoin:round}
.tile{width:44px;height:44px;flex:none;border-radius:14px;background:var(--red-soft);color:var(--red);display:grid;place-items:center}
.brand-logo{display:block;width:34px;height:34px;object-fit:contain}

a{color:inherit;text-decoration:none}
a:focus-visible{outline:3px solid #D9A7A7;outline-offset:2px}
.stack{display:grid;gap:10px}

.row{display:flex;align-items:center;gap:12px;padding:10px 12px;border:1px solid #EFE4E4;border-radius:16px;background:#fff;transition:transform .15s,border-color .15s,background .15s}
.row:hover{border-color:#D9A7A7;background:var(--red-pale)}
.row:active{transform:scale(.985)}
.row .txt{flex:1;min-width:0;display:flex;flex-direction:column;line-height:1.35}
.row b{font-size:15px;font-weight:700;color:var(--red-dark)}
.row small{font-size:12px;color:var(--muted)}
.row .val{direction:ltr;font-size:14px;font-weight:600;color:var(--ink);white-space:nowrap}
.row .go{width:18px;height:18px;color:#B9A8A8;flex:none;fill:none;stroke:currentColor;stroke-width:2;stroke-linecap:round;stroke-linejoin:round}
.contact-row{display:grid;grid-template-columns:minmax(0,1fr) auto;align-items:center;gap:8px;padding:8px 10px;border:1px solid #EADADA;border-radius:14px;background:linear-gradient(110deg,#fff 0%,#FFFAFA 100%);transition:border-color .15s,box-shadow .15s}
.contact-row:hover{border-color:#C98A8A;box-shadow:0 4px 12px -10px rgba(110,20,20,.5)}
.contact-row .contact-info{display:flex;align-items:center;gap:8px;min-width:0}
.contact-row .contact-info .tile{width:36px;height:36px;border-radius:11px;background:#F8EEEE;color:var(--red)}
.contact-row .contact-info .tile .ic{width:18px;height:18px}
.contact-row .txt{display:flex;flex-direction:column;line-height:1.3;min-width:0;gap:2px}
.contact-row .txt b{font-size:13px;color:var(--red-dark);font-weight:800}
.contact-row .val{direction:ltr;font-size:13px;font-weight:700;letter-spacing:.15px;color:var(--ink);white-space:nowrap}
.contact-actions{display:flex;gap:5px;align-items:center}
.contact-action{display:inline-flex;align-items:center;justify-content:center;gap:4px;padding:7px 9px;border:1px solid transparent;border-radius:9px;font-size:11px;font-weight:800;white-space:nowrap;min-width:61px}
.contact-action.call{background:var(--red);color:#fff}
.contact-action.whatsapp{background:#fff;border-color:#D9B5B5;color:var(--red-dark)}
.contact-action .ic{width:14px;height:14px}
@media(max-width:360px){.contact-row{grid-template-columns:minmax(0,1fr);gap:7px}.contact-actions{justify-content:flex-end}.contact-action{padding:6px 10px}}

.stores{display:grid;grid-template-columns:1fr 1fr;gap:10px}
.store{display:flex;align-items:center;gap:10px;padding:12px;border-radius:18px;background:linear-gradient(160deg,var(--red-dark),var(--red));color:#fff;transition:transform .15s}
.store:active{transform:scale(.985)}
.bic{width:28px;height:28px;flex:none;display:block}
.store .tile{width:44px;height:44px;background:#fff;border-radius:14px}
.store .bic{width:28px;height:28px}
.social .bic{width:54px;height:54px;border-radius:16px;box-shadow:0 6px 14px -8px rgba(0,0,0,.45)}
.store .txt{display:flex;flex-direction:column;line-height:1.3;min-width:0}
.store small{font-size:11px;color:#F3DCDC}
.store b{font-size:15px;font-weight:800;direction:ltr;text-align:right}

.socials{display:grid;grid-template-columns:repeat(3,1fr);gap:10px}
.social{display:flex;flex-direction:column;align-items:center;gap:6px;padding:14px 6px 12px;border:1px solid #EFE4E4;border-radius:18px;text-align:center;transition:transform .15s,border-color .15s}
.social:hover{border-color:#F3DCDC}
.social:active{transform:scale(.97)}
.social .tile{width:50px;height:50px;border-radius:16px}
.social .tile .ic{width:24px;height:24px}
.social b{font-size:14px;font-weight:700;color:var(--red-dark)}
.social small{font-size:11px;color:var(--muted);direction:ltr}

.address{display:flex;gap:12px;align-items:flex-start;margin:0 0 12px}
.address p{margin:0;font-size:14px;line-height:1.9;color:var(--ink)}
.maps{display:flex;align-items:center;justify-content:center;gap:8px;height:50px;border-radius:16px;background:linear-gradient(110deg,#F8EEEE,#F1DCDC);color:var(--red-dark);font-weight:800;font-size:15px;transition:transform .15s}
.maps:active{transform:scale(.985)}
.maps .ic{width:20px;height:20px}

footer{text-align:center;color:#8A7A7A;font-size:12px;padding:22px 8px 0;line-height:1.7}

/* دخول ناعم وتحسين التفاعل */
header{animation:hero-in .7s ease both}
section{animation:section-in .55s ease both}
.row,.contact-row,.store,.social,.maps,.contact-action{transition:transform .2s ease,box-shadow .2s ease,border-color .2s ease,background .2s ease}
.store:hover,.maps:hover{transform:translateY(-2px);box-shadow:0 8px 18px -12px rgba(110,20,20,.55)}
.contact-action:hover{transform:translateY(-1px);box-shadow:0 5px 12px -9px rgba(110,20,20,.6)}
.reveal-ready section{animation:none;opacity:0;transform:translateY(14px);transition:opacity .55s ease,transform .55s ease}
.reveal-ready section.is-visible{opacity:1;transform:translateY(0)}
@keyframes hero-in{from{opacity:0;transform:translateY(-12px)}to{opacity:1;transform:translateY(0)}}
@keyframes section-in{from{opacity:0;transform:translateY(10px)}to{opacity:1;transform:translateY(0)}}
@media(max-width:420px){main{width:calc(100% - 22px);margin:11px auto}header{padding:31px 17px 28px;border-radius:23px}.logo{width:min(76%,230px)}header p{font-size:19px}section{padding:15px;border-radius:19px;margin-top:11px}.stores{gap:8px}.store{padding:10px;gap:8px}.store .tile{width:39px;height:39px}.store b{font-size:13px}.store small{font-size:10px}.socials{gap:7px}.social{padding:12px 4px 10px}.social .bic{width:46px;height:46px}.contact-row{gap:6px;padding:8px}.contact-actions{gap:5px}.contact-action{min-width:58px;padding:7px 8px}.row{gap:9px;padding:9px}.row .val{font-size:12px}.address p{font-size:13px}}
@media(max-width:340px){.stores{grid-template-columns:1fr}.socials{grid-template-columns:repeat(3,minmax(0,1fr))}.social b{font-size:12px}.social small{font-size:10px}.contact-row .val{font-size:12px}.contact-action{min-width:54px;font-size:10px}}
@media(prefers-reduced-motion:reduce){*,*::before,*::after{scroll-behavior:auto!important;animation-duration:.01ms!important;animation-iteration-count:1!important;transition-duration:.01ms!important}}

/* ===== أنيميشن محسّن ===== */
.logo{animation:logo-float 5s ease-in-out infinite}
@keyframes logo-float{0%,100%{transform:translateY(0)}50%{transform:translateY(-6px)}}
header::after{animation:ring-drift 9s ease-in-out infinite alternate}
@keyframes ring-drift{from{transform:translate(0,0)}to{transform:translate(-14px,-10px)}}
header p,header .subline,.pill{animation:rise .7s cubic-bezier(.2,.7,.2,1) backwards}
header p{animation-delay:.25s}header .subline{animation-delay:.4s}.pill{animation-delay:.55s}
@keyframes rise{from{opacity:0;transform:translateY(14px)}to{opacity:1;transform:none}}

/* ظهور متدرج لعناصر كل قسم */
.reveal-ready section:not(.is-visible) .item{opacity:0}
.reveal-ready section.is-visible .item{animation:item-in .6s cubic-bezier(.2,.7,.2,1) backwards;animation-delay:calc(var(--i,0)*80ms + 120ms)}
@keyframes item-in{from{opacity:0;transform:translateY(16px) scale(.97)}to{opacity:1;transform:none}}
.reveal-ready section h2{opacity:0;transform:translateX(14px);transition:opacity .5s ease .05s,transform .5s ease .05s}
.reveal-ready section.is-visible h2{opacity:1;transform:none}

/* تفاعل الضغط */
.store,.row,.social,.maps,.contact-action{position:relative;overflow:hidden;-webkit-user-select:none;user-select:none}
.store:active,.row:active,.social:active,.maps:active{transform:scale(.96);transition-duration:.08s}
.contact-action:active{transform:scale(.92);transition-duration:.08s}
.ripple{position:absolute;border-radius:50%;pointer-events:none;background:rgba(150,30,30,.22);transform:scale(0);animation:ripple .6s ease-out forwards}
.store .ripple,.contact-action.call .ripple{background:rgba(255,255,255,.4)}
@keyframes ripple{to{transform:scale(1);opacity:0}}

/* نبض أزرار واتساب */
.contact-action.whatsapp{animation:wa-pulse 2.4s ease-out infinite}
.contact-row:nth-child(2) .whatsapp{animation-delay:.4s}
.contact-row:nth-child(3) .whatsapp{animation-delay:.8s}
.contact-row:nth-child(4) .whatsapp{animation-delay:1.2s}
.contact-row:nth-child(5) .whatsapp{animation-delay:1.6s}
@keyframes wa-pulse{0%{box-shadow:0 0 0 0 rgba(37,211,102,.5)}70%,100%{box-shadow:0 0 0 10px rgba(37,211,102,0)}}

/* شريط فتح في Chrome */
.chrome-bar{display:none;align-items:center;gap:10px;margin:0 0 12px;padding:10px 12px;border-radius:16px;background:#fff;border:1px solid #EFE4E4;box-shadow:0 8px 24px -18px rgba(110,20,20,.35);font-size:13px;font-weight:700;color:var(--red-dark);animation:rise .5s ease both}
.chrome-bar.show{display:flex}
.chrome-bar span{flex:1;line-height:1.5}
.chrome-bar button{font:inherit;font-size:13px;font-weight:800;border:0;border-radius:11px;padding:9px 14px;background:var(--red);color:#fff;cursor:pointer}
.chrome-bar button.x{background:transparent;color:#999;padding:6px 8px;font-size:16px}

.platform-tagline{margin:0 0 14px;padding:12px 14px;border:1px solid rgba(102,0,0,.14);border-radius:14px;background:linear-gradient(135deg,#fff 0%,#fbf5f5 100%);color:#660000;text-align:center;font-size:14px;font-weight:800;line-height:1.8;box-shadow:0 5px 16px -13px rgba(102,0,0,.35)}
@media(max-width:420px){.platform-tagline{font-size:13px;padding:10px 11px;margin-bottom:12px}}
</style></head><body>

<svg width="0" height="0" style="position:absolute" aria-hidden="true">
<defs>
<symbol id="i-globe" viewBox="0 0 24 24"><circle cx="12" cy="12" r="10"/><path d="M12 2a14.5 14.5 0 0 0 0 20 14.5 14.5 0 0 0 0-20"/><path d="M2 12h20"/></symbol>
<symbol id="i-play" viewBox="0 0 24 24"><polygon points="6 3 20 12 6 21 6 3"/></symbol>
<symbol id="i-apple" viewBox="0 0 24 24"><path d="M12 20.94c1.5 0 2.75 1.06 4 1.06 3 0 6-8 6-12.22A4.91 4.91 0 0 0 17 5c-2.22 0-4 1.44-5 2-1-.56-2.78-2-5-2a4.9 4.9 0 0 0-5 4.78C2 14 5 22 8 22c1.25 0 2.5-1.06 4-1.06Z"/><path d="M10 2c1 .5 2 2 2 5"/></symbol>
<symbol id="i-insta" viewBox="0 0 24 24"><rect width="20" height="20" x="2" y="2" rx="5" ry="5"/><path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"/><line x1="17.5" x2="17.51" y1="6.5" y2="6.5"/></symbol>
<symbol id="i-fb" viewBox="0 0 24 24"><path d="M18 2h-3a5 5 0 0 0-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z"/></symbol>
<symbol id="i-tiktok" viewBox="0 0 24 24"><circle cx="8" cy="18" r="4"/><path d="M12 18V2l7 4"/></symbol>
<symbol id="i-phone" viewBox="0 0 24 24"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"/></symbol>
<symbol id="i-mail" viewBox="0 0 24 24"><rect width="20" height="16" x="2" y="4" rx="2"/><path d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7"/></symbol>
<symbol id="i-pin" viewBox="0 0 24 24"><path d="M20 10c0 6-8 12-8 12s-8-6-8-12a8 8 0 0 1 16 0Z"/><circle cx="12" cy="10" r="3"/></symbol>
<symbol id="i-chev" viewBox="0 0 24 24"><path d="m15 18-6-6 6-6"/></symbol>

<linearGradient id="g-insta" x1="0" y1="1" x2="1" y2="0"><stop offset="0" stop-color="#FEDA75"/><stop offset=".28" stop-color="#FA7E1E"/><stop offset=".52" stop-color="#D62976"/><stop offset=".76" stop-color="#962FBF"/><stop offset="1" stop-color="#4F5BD5"/></linearGradient>
<linearGradient id="g-store" x1="0" y1="0" x2="0" y2="1"><stop offset="0" stop-color="#18BFFF"/><stop offset="1" stop-color="#0D5CF0"/></linearGradient>

<symbol id="b-insta" viewBox="0 0 24 24"><rect width="24" height="24" rx="6" fill="url(#g-insta)"/><rect x="5.6" y="5.6" width="12.8" height="12.8" rx="4" fill="none" stroke="#fff" stroke-width="1.7"/><circle cx="12" cy="12" r="3.1" fill="none" stroke="#fff" stroke-width="1.7"/><circle cx="16.2" cy="7.8" r="1" fill="#fff"/></symbol>

<symbol id="b-fb" viewBox="0 0 24 24"><rect width="24" height="24" rx="6" fill="#1877F2"/><path fill="#fff" d="M13.4 20.5v-7.4h2.5l.4-2.9h-2.9V8.4c0-.8.3-1.4 1.5-1.4h1.6V4.4c-.3 0-1.2-.1-2.3-.1-2.3 0-3.8 1.4-3.8 3.9v2H7.9v2.9h2.5v7.4z"/></symbol>

<symbol id="b-tiktok" viewBox="0 0 24 24"><rect width="24" height="24" rx="6" fill="#000"/>
<path transform="translate(5.4 5.3) scale(.5)" fill="#25F4EE" d="M12.525.02c1.31-.02 2.61-.01 3.91-.02.08 1.53.63 3.09 1.75 4.17 1.12 1.11 2.7 1.62 4.24 1.79v4.03c-1.44-.05-2.89-.35-4.2-.97-.57-.26-1.1-.59-1.62-.93-.01 2.92.01 5.84-.02 8.75-.08 1.4-.54 2.79-1.35 3.94-1.31 1.92-3.58 3.17-5.91 3.21-1.43.08-2.86-.31-4.08-1.03-2.02-1.19-3.44-3.37-3.65-5.71-.02-.5-.03-1-.01-1.49.18-1.9 1.12-3.72 2.58-4.96 1.66-1.44 3.98-2.13 6.15-1.72.02 1.48-.04 2.96-.04 4.44-.99-.32-2.15-.23-3.02.37-.63.41-1.11 1.04-1.36 1.75-.21.51-.15 1.07-.14 1.61.24 1.64 1.82 3.02 3.5 2.87 1.12-.01 2.19-.66 2.77-1.61.19-.33.4-.67.41-1.06.1-1.79.06-3.57.07-5.36.01-4.03-.01-8.05.02-12.07z"/>
<path transform="translate(6.6 6.5) scale(.5)" fill="#FE2C55" d="M12.525.02c1.31-.02 2.61-.01 3.91-.02.08 1.53.63 3.09 1.75 4.17 1.12 1.11 2.7 1.62 4.24 1.79v4.03c-1.44-.05-2.89-.35-4.2-.97-.57-.26-1.1-.59-1.62-.93-.01 2.92.01 5.84-.02 8.75-.08 1.4-.54 2.79-1.35 3.94-1.31 1.92-3.58 3.17-5.91 3.21-1.43.08-2.86-.31-4.08-1.03-2.02-1.19-3.44-3.37-3.65-5.71-.02-.5-.03-1-.01-1.49.18-1.9 1.12-3.72 2.58-4.96 1.66-1.44 3.98-2.13 6.15-1.72.02 1.48-.04 2.96-.04 4.44-.99-.32-2.15-.23-3.02.37-.63.41-1.11 1.04-1.36 1.75-.21.51-.15 1.07-.14 1.61.24 1.64 1.82 3.02 3.5 2.87 1.12-.01 2.19-.66 2.77-1.61.19-.33.4-.67.41-1.06.1-1.79.06-3.57.07-5.36.01-4.03-.01-8.05.02-12.07z"/>
<path transform="translate(6 5.9) scale(.5)" fill="#fff" d="M12.525.02c1.31-.02 2.61-.01 3.91-.02.08 1.53.63 3.09 1.75 4.17 1.12 1.11 2.7 1.62 4.24 1.79v4.03c-1.44-.05-2.89-.35-4.2-.97-.57-.26-1.1-.59-1.62-.93-.01 2.92.01 5.84-.02 8.75-.08 1.4-.54 2.79-1.35 3.94-1.31 1.92-3.58 3.17-5.91 3.21-1.43.08-2.86-.31-4.08-1.03-2.02-1.19-3.44-3.37-3.65-5.71-.02-.5-.03-1-.01-1.49.18-1.9 1.12-3.72 2.58-4.96 1.66-1.44 3.98-2.13 6.15-1.72.02 1.48-.04 2.96-.04 4.44-.99-.32-2.15-.23-3.02.37-.63.41-1.11 1.04-1.36 1.75-.21.51-.15 1.07-.14 1.61.24 1.64 1.82 3.02 3.5 2.87 1.12-.01 2.19-.66 2.77-1.61.19-.33.4-.67.41-1.06.1-1.79.06-3.57.07-5.36.01-4.03-.01-8.05.02-12.07z"/></symbol>

<symbol id="b-appstore" viewBox="0 0 24 24"><rect width="24" height="24" rx="6" fill="url(#g-store)"/><g fill="none" stroke="#fff" stroke-width="1.9" stroke-linecap="round"><path d="M12.6 5.6 7.9 17.4"/><path d="M12.6 5.6 17.4 17.4"/><path d="M8 14.4h8.2"/></g></symbol>

<symbol id="b-play" viewBox="0 0 24 24"><g stroke-linejoin="round" stroke-width=".6"><path fill="#00C8FF" stroke="#00C8FF" d="M3.6 2.4v19.2l9.7-9.6z"/><path fill="#00F076" stroke="#00F076" d="M3.6 2.4 16.6 9.9l-3.3 2.1z"/><path fill="#FF3D4A" stroke="#FF3D4A" d="M3.6 21.6 16.6 14.1l-3.3-2.1z"/><path fill="#FFD400" stroke="#FFD400" d="M16.6 9.9 20.6 12l-4 2.1-3.3-2.1z"/></g></symbol>

<symbol id="b-pin" viewBox="0 0 24 24"><path fill="#EA4335" d="M12 1.8a7.8 7.8 0 0 0-7.8 7.8c0 5.6 7.8 12.6 7.8 12.6s7.8-7 7.8-12.6A7.8 7.8 0 0 0 12 1.8z"/><circle cx="12" cy="9.6" r="3" fill="#fff"/></symbol>
</defs>
</svg>

<main>
<div class="chrome-bar" id="chromeBar"><span>للحصول على أفضل تجربة، افتح الصفحة في Google Chrome</span><button type="button" id="chromeBtn">فتح في Chrome</button><button type="button" class="x" id="chromeX" aria-label="إغلاق">✕</button></div>

<header>
<img class="logo" src="data:image/png;base64,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
