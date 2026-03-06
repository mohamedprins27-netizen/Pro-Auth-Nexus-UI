<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dev Mo Alaa | Pro UI v4.0</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@300;400;600;700;900&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root { --primary: #6366f1; --primary-glow: rgba(99, 102, 241, 0.4); --grad-to: #9333ea; }
        body { 
            font-family: 'Cairo', sans-serif; background-color: #03040a; color: #fff; margin: 0; overflow-x: hidden;
            background-image: linear-gradient(to bottom, rgba(3, 4, 10, 0.85), rgba(3, 4, 10, 0.95)), 
                              url('https://images.unsplash.com/photo-1635776062127-d379bfcba9f8?q=80&w=2000&auto=format&fit=crop');
            background-size: cover; background-position: center; background-attachment: fixed; transition: all 0.5s ease;
        }

        #preloader {
            position: fixed; top: 0; left: 0; width: 100%; height: 100%;
            background: #03040a; z-index: 10000; display: flex; flex-direction: column;
            align-items: center; justify-content: center; transition: opacity 0.6s ease;
        }

        @keyframes shake { 0%, 100% { transform: translateX(0); } 25% { transform: translateX(-8px); } 75% { transform: translateX(8px); } }
        .shake { animation: shake 0.3s ease-in-out; border-color: #ef4444 !important; }

        .avatar-glow {
            width: 80px; height: 80px; border-radius: 50%; background: rgba(255, 255, 255, 0.03);
            border: 2px solid rgba(255, 255, 255, 0.08); display: flex; align-items: center; justify-content: center;
            margin: 0 auto 20px; box-shadow: 0 0 20px var(--primary-glow); position: relative;
        }
        .avatar-glow::after {
            content: ""; position: absolute; inset: -4px; border-radius: 50%;
            border: 2px solid var(--primary); animation: pulse-glow 2s infinite;
        }
        @keyframes pulse-glow { 0% { transform: scale(1); opacity: 0.5; } 50% { transform: scale(1.15); opacity: 0; } 100% { transform: scale(1); opacity: 0; } }

        .form-container { transition: all 0.4s ease; }
        .form-hidden { opacity: 0; transform: translateY(15px); display: none; }
        .bento-card { background: rgba(10, 12, 18, 0.5); border: 1px solid rgba(255, 255, 255, 0.08); backdrop-filter: blur(25px); }

        .loading-bar { height: 1.5px; width: 100%; background: rgba(255, 255, 255, 0.03); position: absolute; bottom: 0; left: 0; overflow: hidden; }
        .loading-bar::after {
            content: ""; position: absolute; inset: 0; left: -100%;
            background: linear-gradient(90deg, transparent, var(--primary), var(--grad-to), transparent);
            animation: moveLoading 3s infinite linear;
        }
        @keyframes moveLoading { 0% { left: -100%; } 100% { left: 100%; } }

        .smart-input { background: rgba(255, 255, 255, 0.03); border: 1px solid rgba(255, 255, 255, 0.1); transition: 0.3s; color: white; outline: none; text-align: right; }
        .smart-input:focus { border-color: var(--primary); background: rgba(255, 255, 255, 0.06); }

        #theme-switcher { position: fixed; top: 20px; left: 20px; z-index: 1001; background: rgba(10,12,18,0.8); padding: 10px; border-radius: 50px; display: flex; gap: 8px; border: 1px solid rgba(255,255,255,0.1); }
        .color-dot { width: 18px; height: 18px; border-radius: 50%; cursor: pointer; border: 2px solid transparent; transition: 0.3s; }
        .color-dot.active { border-color: #fff; transform: scale(1.2); }
    </style>
</head>
<body class="min-h-screen flex flex-col items-center justify-center p-4">

    <div id="preloader">
        <div class="w-10 h-10 border-2 border-white/5 border-t-indigo-500 rounded-full animate-spin mb-4"></div>
        <span class="text-white/40 font-mono tracking-[0.3em] text-[9px] uppercase">جاري جلب البيانات</span>
    </div>

    <div id="theme-switcher">
        <div class="color-dot active" style="background: #6366f1;" onclick="setTheme('#6366f1', 'rgba(99, 102, 241, 0.4)', '#9333ea', this)"></div>
        <div class="color-dot" style="background: #00d2ff;" onclick="setTheme('#00d2ff', 'rgba(0, 210, 255, 0.4)', '#0062ff', this)"></div>
        <div class="color-dot" style="background: #10b981;" onclick="setTheme('#10b981', 'rgba(16, 185, 129, 0.4)', '#059669', this)"></div>
        <div class="color-dot" style="background: #f59e0b;" onclick="setTheme('#f59e0b', 'rgba(245, 158, 11, 0.4)', '#d97706', this)"></div>
    </div>

    <div class="w-full max-w-6xl grid grid-cols-12 gap-5 relative z-10 py-10">
        
        <div class="col-span-12 lg:col-span-7 bento-card rounded-[3rem] p-10 lg:p-16 hidden lg:flex flex-col justify-between min-h-[580px] relative overflow-hidden">
            <div class="relative z-10">
                <div class="inline-flex items-center gap-2 px-4 py-1.5 rounded-full bg-white/5 border border-white/10 text-[10px] font-bold mb-10 uppercase tracking-widest" style="color: var(--primary)">
                    <span class="w-1.5 h-1.5 rounded-full animate-pulse" style="background: var(--primary)"></span>
                    الخيار الحالي: واجهة احترافية
                </div>
                <div class="h-44">
                    <h1 id="dynamic-text" class="text-6xl lg:text-7xl font-black mb-6 leading-tight tracking-tighter transition-all duration-500">
                        نبني <br> <span id="gradient-span" class="text-transparent bg-clip-text">حلولاً</span> ذكية.
                    </h1>
                </div>
                <p id="dynamic-desc" class="text-slate-400 text-lg max-w-md font-light">تجارب رقمية تدمج بين قوة الأداء وجمال التصميم المتطور.</p>
            </div>
            <div class="flex gap-6 opacity-20 text-2xl">
                <i class="fab fa-react"></i><i class="fab fa-node-js"></i><i class="fab fa-laravel"></i><i class="fab fa-python"></i>
            </div>
            <div class="loading-bar"></div>
        </div>

        <div id="auth-card" class="col-span-12 lg:col-span-5 bento-card rounded-[3rem] p-8 lg:p-12 relative overflow-hidden shadow-2xl min-h-[580px] flex flex-col justify-center text-center">
            
            <div class="avatar-glow"><i class="fas fa-fingerprint text-3xl opacity-70" style="color: var(--primary)"></i></div>

            <div id="login-form" class="form-container w-full">
                <div class="mb-8 text-right">
                    <h2 class="text-3xl font-black mb-1 italic tracking-tighter">الولوج</h2>
                    <p class="text-slate-500 text-sm">أدخل بياناتك للمتابعة...</p>
                </div>
                <div class="space-y-4">
                    <input type="email" id="email" placeholder="البريد الإلكتروني" class="w-full smart-input rounded-2xl py-4 px-6">
                    <input type="password" id="password" placeholder="كلمة المرور" class="w-full smart-input rounded-2xl py-4 px-6">
                    <button onclick="validateLogin()" class="group w-full text-white font-black py-4 rounded-2xl shadow-lg active:scale-95 transition-all flex items-center justify-center gap-3" style="background: var(--primary)">
                        <span>دخول للمنصة</span>
                        <i class="fas fa-arrow-left text-xs transition-transform group-hover:-translate-x-2"></i>
                    </button>
                    <div class="flex justify-between px-2 pt-2 text-xs">
                        <button onclick="switchForm('forgot-form')" class="text-slate-500 hover:text-white">نسيت السر؟</button>
                        <button onclick="switchForm('reg-form')" class="font-bold" style="color: var(--primary)">إنشاء حساب</button>
                    </div>
                </div>
            </div>

            <div id="reg-form" class="form-container form-hidden w-full text-right">
                <h2 class="text-3xl font-black mb-6 italic tracking-tighter">عضوية جديدة</h2>
                <div class="space-y-4">
                    <input type="text" placeholder="الاسم الكامل" class="w-full smart-input rounded-2xl py-4 px-6">
                    <input type="email" placeholder="البريد الإلكتروني" class="w-full smart-input rounded-2xl py-4 px-6">
                    <input type="password" placeholder="كلمة المرور" class="w-full smart-input rounded-2xl py-4 px-6">
                    <button class="w-full text-white font-black py-4 rounded-2xl shadow-lg active:scale-95 transition-all" style="background: var(--primary)">تأكيد الحساب</button>
                    <button onclick="switchForm('login-form')" class="w-full text-slate-500 mt-2">لديك حساب؟ سجل دخول</button>
                </div>
            </div>

            <div id="forgot-form" class="form-container form-hidden w-full text-right">
                <h2 class="text-3xl font-black mb-6 italic tracking-tighter">استعادة</h2>
                <div class="space-y-4">
                    <input type="email" placeholder="بريدك الإلكتروني" class="w-full smart-input rounded-2xl py-4 px-6">
                    <button class="w-full text-white font-black py-4 rounded-2xl shadow-lg active:scale-95 transition-all" style="background: var(--primary)">إرسال الرابط</button>
                    <button onclick="switchForm('login-form')" class="w-full text-slate-500 mt-2">رجوع</button>
                </div>
            </div>

            <div class="loading-bar"></div>
        </div>
    </div>

    <footer class="mt-10 flex flex-col items-center group">
        <div class="h-6 w-px opacity-20 mb-3 group-hover:h-10 transition-all" style="background: var(--primary)"></div>
        <div class="px-8 py-2 rounded-full bg-black/40 border border-white/5 backdrop-blur-xl">
            <span class="text-[9px] text-slate-600 font-mono tracking-[0.4em] uppercase">Built by</span>
            <span class="text-xs font-black ml-2 tracking-widest" style="color: var(--primary)">DEV MO ALAA</span>
        </div>
    </footer>

    <script>
        window.addEventListener('load', () => { 
            setTimeout(() => { 
                const p = document.getElementById('preloader');
                if(p) { p.style.opacity = '0'; setTimeout(() => p.style.display = 'none', 600); }
            }, 1200);
        });

        function validateLogin() {
            const email = document.getElementById('email');
            const pass = document.getElementById('password');
            const card = document.getElementById('auth-card');

            if (!email.value || !pass.value) {
                card.classList.add('shake');
                setTimeout(() => card.classList.remove('shake'), 400);
            } else {
                alert('الخيار الحالي: جاري التحقق من البيانات...');
            }
        }

        function setTheme(p, g, t, dot) {
            document.documentElement.style.setProperty('--primary', p);
            document.documentElement.style.setProperty('--primary-glow', g);
            document.documentElement.style.setProperty('--grad-to', t);
            document.getElementById('gradient-span').style.backgroundImage = `linear-gradient(to right, ${p}, ${t})`;
            document.querySelectorAll('.color-dot').forEach(d => d.classList.remove('active'));
            dot.classList.add('active');
        }

        function switchForm(id) {
            document.querySelectorAll('.form-container').forEach(f => { f.classList.add('form-hidden'); f.style.display = 'none'; });
            const target = document.getElementById(id);
            target.style.display = 'block';
            setTimeout(() => target.classList.remove('form-hidden'), 50);
        }

        const content = [
            { t: 'نبني <br> <span class="text-transparent bg-clip-text">حلولاً</span> ذكية.', d: 'تجارب رقمية تدمج بين قوة الأداء وجمال التصميم.' },
            { t: 'كود <br> <span class="text-transparent bg-clip-text">نظيف</span> ومستقر.', d: 'نهتم بأدق التفاصيل لضمان استقرار مشاريعك للأبد.' },
            { t: 'واجهات <br> <span class="text-transparent bg-clip-text">تسبق</span> العصر.', d: 'استمتع بأحدث تريندات الـ UI/UX في متناول يدك.' }
        ];
        let idx = 0;
        setInterval(() => {
            const h1 = document.getElementById('dynamic-text');
            const p = document.getElementById('dynamic-desc');
            h1.style.opacity = '0';
            setTimeout(() => {
                idx = (idx + 1) % content.length;
                h1.innerHTML = content[idx].t;
                p.innerText = content[idx].d;
                h1.querySelector('span').style.backgroundImage = `linear-gradient(to right, var(--primary), var(--grad-to))`;
                h1.style.opacity = '1';
            }, 500);
        }, 4000);

        document.getElementById('gradient-span').style.backgroundImage = `linear-gradient(to right, #6366f1, #9333ea)`;


    document.addEventListener('contextmenu', event => event.preventDefault());

    
    document.onkeydown = function(e) {
        if (e.keyCode == 123) return false; // F12
        if (e.ctrlKey && e.shiftKey && e.keyCode == 'I'.charCodeAt(0)) return false;
        if (e.ctrlKey && e.shiftKey && e.keyCode == 'C'.charCodeAt(0)) return false;
        if (e.ctrlKey && e.shiftKey && e.keyCode == 'J'.charCodeAt(0)) return false;
        if (e.ctrlKey && e.keyCode == 'U'.charCodeAt(0)) return false; // Ctrl+U (View Source)
    };
    </script>
</body>
</html>