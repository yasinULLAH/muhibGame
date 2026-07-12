# Flappy Muhib 🐦

*(English Documentation follows below. اردو کی تفصیلات نیچے دی گئی ہیں۔)*

---

## 🇬🇧 English Documentation

### Overview
**Flappy Muhib** is a beautifully crafted, open-source web-based game inspired by the classic "Flappy Bird". It is built with a strong focus on modern web capabilities, seamless performance, and emotional value. 

### Dedication
This project is deeply personal and is **dedicated with love to my little brother, Muhib Ullah ❤️.** 
*"Keep flying high, little bro!"*

### Features & Functionalities

1. **Progressive Web App (PWA) Integration**
   - **Installable:** Users can install the game directly to their home screen on Android, iOS, or Desktop without using an app store.
   - **Offline Mode:** Thanks to Service Workers and Workbox, the game caches its assets and is fully playable without an internet connection.
   - **Fullscreen Experience:** Once installed, it launches in a native, immersive fullscreen mode, hiding the browser's URL bar and navigation buttons. An in-game Fullscreen toggle is also available for browser users.

2. **Responsive Canvas Design**
   - The game dynamically calculates the screen aspect ratio and resizes the HTML5 Canvas to fit any device perfectly, whether you are on a massive desktop monitor or a small smartphone.

3. **Multiple Difficulty Levels**
   - **EASY:** Wider gaps between pipes, slower movement speed, and lower gravity for a relaxed experience.
   - **MEDIUM:** The standard balanced mode.
   - **HARD:** Tighter gaps, faster pipe movement, and heavier gravity for a challenging experience.

4. **Scoring & Badges System**
   - Players earn points by successfully navigating through the pipes.
   - Based on the final score, players are awarded distinct badges:
     - 💎 **Platinum:** 100+ points
     - 🏆 **Gold:** 50 - 99 points
     - 🥈 **Silver:** 25 - 49 points
     - 🥉 **Bronze:** 10 - 24 points
     - 🥚 **Beginner:** 0 - 9 points

5. **Advanced Statistics & History Tracking**
   - The game utilizes the browser's `localStorage` to keep track of the player's performance.
   - **Best Score:** The highest score achieved is tracked separately for *each* difficulty mode.
   - **Top 10 History:** A dedicated "Stats" screen shows the 10 most recent games, detailing the Date, Game Mode, Score, and Badge earned. Users can clear this history at any time.

6. **Audio & Sound Effects**
   - Engaging sound effects for flapping wings, scoring points, hitting pipes, game over, and UI swooshes.
   - A global **Mute/Unmute** button that remembers the user's preference across sessions.

7. **Pause & Resume functionality**
   - Players can pause the game mid-flight using an on-screen pause button or keyboard shortcuts.

### How to Play (Controls)
- **Jump / Flap:** Tap the screen, Click the mouse, or press the `Spacebar` / `Up Arrow`.
- **Pause Game:** Click the Pause icon ⏸️, press the `Escape` key, or press `P`.

### Modules & Code Architecture
- **DOM & UI Management:** HTML overlays are used for Start, Game Over, Pause, and Stats screens to keep the Canvas rendering strictly for gameplay.
- **Game Engine Loop:** A custom `requestAnimationFrame` loop updates object physics (gravity, velocity, collisions) and draws them to the screen context.
- **Physics Module:** Handles gravity, jump velocity, and ceiling/floor/pipe collision detection.
- **Asset Loader:** Preloads all images and sounds before the game starts to prevent mid-game stuttering.
- **PWA Service Worker:** `sw.js` and `pwa-register.js` handle intercepting network requests, caching assets for offline play, and listening to the `beforeinstallprompt` to trigger the app installation flow.

---

## 🇵🇰 اردو (Urdu Documentation)

### جائزہ (Overview)
**فلیپی محب (Flappy Muhib)** ایک بہترین اور اوپن سورس ویب بیسڈ گیم ہے جو مشہور "Flappy Bird" سے متاثر ہو کر بنائی گئی ہے۔ اسے جدید ویب ٹیکنالوجی کا استعمال کرتے ہوئے بہترین پرفارمنس کے لیے ڈیزائن کیا گیا ہے۔

### انتساب (Dedication)
یہ پروجیکٹ میرے لیے بہت خاص ہے اور اسے میں اپنے **چھوٹے بھائی محب اللہ ❤️ کے نام** کرتا ہوں۔ 
*"Keep flying high, little bro!" (ہمیشہ اونچی اڑان اڑتے رہو، چھوٹے بھائی!)*

### خصوصیات اور فنکشنز (Features & Functionalities)

1. **پروگریسو ویب ایپ (PWA - Progressive Web App)**
   - **انسٹال کی سہولت:** صارفین اس گیم کو کسی بھی ایپ اسٹور کے بغیر اپنے اینڈرائیڈ، آئی او ایس (iOS)، یا کمپیوٹر کی ہوم اسکرین پر ایپ کے طور پر انسٹال کر سکتے ہیں۔
   - **آف لائن موڈ:** سروس ورکرز (Service Workers) کی مدد سے یہ گیم انٹرنیٹ کے بغیر بھی مکمل طور پر کھیلی جا سکتی ہے۔
   - **فل اسکرین تجربہ (Fullscreen):** پی ڈبلیو اے (PWA) کے طور پر انسٹال ہونے کے بعد، یہ گیم موبائل میں بغیر کسی نیویگیشن بار کے فل اسکرین پر چلتی ہے۔ عام براؤزر میں کھیلنے والوں کے لیے بھی ایک خاص "فل اسکرین" بٹن دیا گیا ہے۔

2. **رسپانسیو کینوس ڈیزائن (Responsive Canvas Design)**
   - یہ گیم آپ کے موبائل یا کمپیوٹر کی اسکرین کے سائز کو خودکار طور پر جانچ کر اپنے آپ کو اسکرین کے حساب سے ایڈجسٹ کر لیتی ہے تاکہ گرافکس بالکل واضح رہیں۔

3. **مشکل کی مختلف سطحیں (Difficulty Levels)**
   - **آسان (EASY):** پائپوں کے درمیان زیادہ فاصلہ، دھیمی رفتار، اور کم کشش ثقل تاکہ بچے اور نئے کھلاڑی آسانی سے کھیل سکیں۔
   - **درمیانہ (MEDIUM):** معیاری اور متوازن موڈ۔
   - **مشکل (HARD):** پائپوں کے درمیان کم فاصلہ، تیز رفتار، اور زیادہ کشش ثقل جو تجربہ کار کھلاڑیوں کے لیے ایک چیلنج ہے۔

4. **اسکورنگ اور بیجز کا نظام (Scoring & Badges System)**
   - پائپوں کے درمیان سے کامیابی سے گزرنے پر کھلاڑی کو پوائنٹس ملتے ہیں۔
   - حتمی اسکور کی بنیاد پر کھلاڑیوں کو مختلف بیجز (Badges) دیے جاتے ہیں:
     - 💎 **پلاٹینم (Platinum):** 100 یا اس سے زیادہ پوائنٹس
     - 🏆 **گولڈ (Gold):** 50 سے 99 پوائنٹس
     - 🥈 **سلور (Silver):** 25 سے 49 پوائنٹس
     - 🥉 **برونز (Bronze):** 10 سے 24 پوائنٹس
     - 🥚 **بگنر (Beginner):** 0 سے 9 پوائنٹس

5. **تفصیلی اعداد و شمار اور ہسٹری (Advanced Statistics)**
   - گیم براؤزر کی `localStorage` کا استعمال کرتے ہوئے کھلاڑی کی کارکردگی کو محفوظ رکھتی ہے۔
   - **بہترین اسکور (Best Score):** ہر مشکل (Difficulty) کے لیول کا بہترین اسکور الگ الگ محفوظ کیا جاتا ہے۔
   - **ٹاپ 10 ہسٹری:** "Stats" اسکرین پر کھلاڑی پچھلی 10 گیمز کی ہسٹری دیکھ سکتا ہے جس میں تاریخ، موڈ، اسکور اور بیج کی تفصیل شامل ہوتی ہے۔ اسے ڈیلیٹ (Clear) کرنے کا آپشن بھی موجود ہے۔

6. **آڈیو اور ساؤنڈ ایفیکٹس (Audio & Sound Effects)**
   - اڑنے، پوائنٹ ملنے، پائپ سے ٹکرانے اور گیم اوور ہونے کے لیے بہترین ساؤنڈ ایفیکٹس شامل کیے گئے ہیں۔
   - **میوٹ (Mute)** بٹن دیا گیا ہے جو آپ کی آڈیو سیٹنگ کو ہمیشہ کے لیے یاد رکھتا ہے۔

7. **گیم کو روکنے کی سہولت (Pause & Resume)**
   - کھیل کے دوران کھلاڑی کسی بھی وقت اسکرین پر موجود "Pause" بٹن دبا کر گیم کو روک سکتا ہے۔

### کھیلنے کا طریقہ (How to Play)
- **اڑنے کے لیے (Jump / Flap):** اسکرین پر ٹیپ کریں، ماؤس سے کلک کریں، یا کی بورڈ سے `Spacebar` / اوپر والا تیر (Up Arrow) دبائیں۔
- **گیم روکنے کے لیے (Pause Game):** ⏸️ آئیکن پر کلک کریں، یا کی بورڈ سے `Escape` یا `P` کا بٹن دبائیں۔

### کوڈ اور ماڈیولز کی ساخت (Modules & Architecture)
- **DOM & UI مینیجمنٹ:** گیم کے مینیو، گیم اوور اور اسٹیٹس کی اسکرینز کے لیے HTML اوورلیز (Overlays) کا استعمال کیا گیا ہے، جبکہ اصل گیم کینوس (Canvas) پر چلتی ہے۔
- **گیم انجن لوپ:** ایک کسٹم `requestAnimationFrame` لوپ فزکس (کشش ثقل، رفتار، ٹکراؤ) کو کنٹرول کرتا ہے اور اسکرین پر چیزوں کو ڈرا کرتا ہے۔
- **فزکس ماڈیول:** پرندے کے اڑنے، گرنے اور پائپوں سے ٹکرانے کا حساب لگاتا ہے۔
- **PWA سروس ورکر:** `sw.js` نیٹ ورک کی درخواستوں کو کنٹرول کرتا ہے، انٹرنیٹ کے بغیر کھیلنے کے لیے فائلز کو کیش (Cache) کرتا ہے، اور ایپ انسٹالیشن کو منظم کرتا ہے۔

---

### Open Source Contribution
This project is open-source. Feel free to explore the code, learn from the architecture, and contribute to making it even better.

**Client Notes:** 
*This comprehensive document outlines the full scope, scale, and feature completeness of the Flappy Muhib application. The application is completely deployment-ready, supports advanced offline PWA installations, dynamically handles all display resolutions, and possesses a modular, lightweight codebase.*
