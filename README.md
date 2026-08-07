/* HIGH TECH PS - Premium Neo-Dark Theme */
@import url('https://googleapis.com');

:root {
    --bg-main: #060a13;
    --bg-card: #0f1626;
    --border-glow: #00f0ff;
    --ps-blue: #0070d1;
    --gold-accent: #ffd700;
    --gold-glow: #ffa500;
    --text-white: #ffffff;
    --text-muted: #8a99ad;
    --success: #00ff66;
}

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    font-family: 'Cairo', sans-serif;
    user-select: none;
    -webkit-user-select: none;
}

body {
    background-color: var(--bg-main);
    color: var(--text-white);
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    overflow-x: hidden;
    padding: 20px;
}

/* الهيدر الاحترافي */
header {
    width: 100%;
    max-width: 1100px;
    text-align: center;
    padding: 40px 20px;
    background: radial-gradient(circle at top, rgba(0,240,255,0.15) 0%, rgba(6,10,19,0) 70%);
}

.logo {
    font-size: 3rem;
    font-weight: 900;
    letter-spacing: 3px;
    color: var(--text-white);
    text-shadow: 0 0 10px var(--ps-blue), 0 0 20px var(--border-glow);
    animation: pulseGlow 3s infinite alternate;
}

.subtitle {
    font-size: 1.2rem;
    color: var(--text-muted);
    font-weight: 600;
    margin-top: 10px;
}

.container {
    width: 100%;
    max-width: 1100px;
    display: flex;
    flex-direction: column;
    gap: 25px;
}

/* حالة الويب كيت والكاش */
.status-bar {
    background-color: var(--bg-card);
    border: 1px solid rgba(0, 240, 255, 0.2);
    border-radius: 12px;
    padding: 15px 25px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    font-weight: 600;
    box-shadow: inset 0 0 10px rgba(0, 240, 255, 0.05);
}

.status-indicator {
    color: var(--success);
    display: flex;
    align-items: center;
    gap: 8px;
    text-shadow: 0 0 8px var(--success);
}

.status-indicator::before {
    content: '';
    width: 10px;
    height: 10px;
    background-color: var(--success);
    border-radius: 50%;
    box-shadow: 0 0 10px var(--success);
}

/* لوحة تفعيل GoldHEN */
.main-exploit-box {
    background: linear-gradient(145deg, #131c33 0%, #090e1a 100%);
    border: 2px solid var(--gold-accent);
    box-shadow: 0 0 25px rgba(255, 215, 0, 0.15);
    border-radius: 20px;
    padding: 35px;
    text-align: center;
    position: relative;
}

.main-exploit-box h3 {
    color: var(--gold-accent);
    font-size: 1.6rem;
    font-weight: 800;
    text-shadow: 0 0 10px rgba(255, 215, 0, 0.3);
}

.badge {
    display: inline-block;
    background: rgba(255, 215, 0, 0.08);
    color: var(--gold-accent);
    padding: 4px 14px;
    border-radius: 6px;
    font-size: 0.9rem;
    font-weight: 800;
    margin: 15px 0 25px 0;
    border: 1px solid rgba(255, 215, 0, 0.25);
}

/* زر التفعيل الذهبي الفاخر مع حركة السهم التفاعلية */
.btn-goldhen {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    gap: 18px;
    background: linear-gradient(45deg, var(--gold-accent), var(--gold-glow));
    color: #000000;
    font-size: 1.8rem;
    font-weight: 900;
    padding: 18px 55px;
    border: none;
    border-radius: 50px;
    cursor: pointer;
    box-shadow: 0 0 25px rgba(255, 215, 0, 0.35);
    transition: all 0.3s cubic-bezier(0.175, 0.885, 0.32, 1.275);
}

.btn-goldhen:hover {
    transform: scale(1.04);
    box-shadow: 0 0 40px rgba(255, 215, 0, 0.6);
}

.arrow {
    font-size: 2rem;
    animation: pointToText 0.6s infinite alternate cubic-bezier(0.455, 0.03, 0.515, 0.955);
}

@keyframes pointToText {
    from { transform: translateX(0); }
    to { transform: translateX(-12px); }
}

/* مصفوفة وجداول الأجهزة السوفت وير */
.grid-layout {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 25px;
}

@media (max-width: 800px) {
    .grid-layout { grid-template-columns: 1fr; }
}

.console-panel {
    background-color: var(--bg-card);
    border: 1px solid rgba(255, 255, 255, 0.06);
    border-radius: 18px;
    padding: 30px;
    transition: all 0.3s ease;
}

.console-panel:hover {
    border-color: var(--border-glow);
    box-shadow: 0 0 15px rgba(0, 240, 255, 0.1);
}

.panel-title {
    font-size: 1.6rem;
    font-weight: 900;
    margin-bottom: 20px;
    letter-spacing: 1px;
}

.panel-title span {
    color: var(--border-glow);
    text-shadow: 0 0 8px rgba(0, 240, 255, 0.4);
}

.fw-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(85px, 1fr));
    gap: 12px;
    list-style: none;
    margin-top: 20px;
}

.fw-btn {
    background: rgba(255, 255, 255, 0.03);
    border: 1px solid rgba(255, 255, 255, 0.08);
    padding: 12px 5px;
    text-align: center;
    border-radius: 10px;
    font-weight: 700;
    color: #e2e8f0;
    cursor: pointer;
    transition: all 0.2s ease;
}

.fw-btn:hover {
    background: var(--ps-blue);
    color: var(--text-white);
    border-color: var(--border-glow);
    box-shadow: 0 0 10px rgba(0, 112, 209, 0.5);
    transform: translateY(-2px);
}

/* شاشة التحميل المعتمة والـ Overlay */
.overlay-loader {
    display: none;
    position: fixed;
    top: 0; left: 0; width: 100%; height: 100%;
    background: rgba(6, 10, 19, 0.98);
    z-index: 10000;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    gap: 25px;
}

.spinner-ring {
    width: 70px;
    height: 70px;
    border: 6px solid rgba(0, 240, 255, 0.05);
    border-top: 6px solid var(--border-glow);
    border-radius: 50%;
    animation: spin 0.8s linear infinite;
    box-shadow: 0 0 15px rgba(0, 240, 255, 0.2);
}

@keyframes spin {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
}

@keyframes pulseGlow {
    from { text-shadow: 0 0 10px var(--ps-blue), 0 0 20px var(--border-glow); }
    to { text-shadow: 0 0 15px var(--ps-blue), 0 0 35px var(--border-glow), 0 0 40px var(--border-glow); }
}

footer {
    margin-top: auto;
    width: 100%;
    text-align: center;
    padding: 30px;
    color: #475569;
    font-size: 0.9rem;
    border-top: 1px solid rgba(255,255,255,0.03);
}
# 🎮 HIGH TECH PS - PlayStation Exploit & Maintenance Host

موقع استضافة وتفعيل تعديلات أجهزة البلاي ستيشن (PS4 / PS5) مصمم ببرمجيات حديثة فائقة الأداء، مهيأ ليعمل بشكل مستقل وخفيف على متصفحات البلاي ستيشن ومزود بميزة التخزين المؤقت أوفلاين بالكامل لحماية الأجهزة من شبكات سوني.
