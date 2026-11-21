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

8. **Multiple Game Modes**
   - **Arcade Mode:** Packed with collectible Gold Coins, Ruby Gems (+5 coins), Power-Ups, and a dynamic 2× Score Fever Mode triggered by 5-hit combos or close calls.
   - **Classic Mode:** Authentic, pure skill-based gameplay with traditional physics and no power-ups.
   - **Blitz 45s Mode:** A frantic race against a 45-second clock where navigating pipes and collecting Clock orbs restores precious seconds.
   - **Zen Practice Mode:** A tranquil, no-death practice mode where the bird gently bounces off obstacles and ground without ending the flight.

9. **Expanded Hangar & Shop System**
   - **28 Collectible Bird Skins:** Spanning Classic, Rare, Epic, Legendary, and Mythic rarity tiers:
     - *Muhib Gold, Sky Jay, Phoenix, Emerald, Cyber Wing, Galaxy Owl, Dragon, Royal Crown, Shadow Ninja, Archangel, Lava Demon, Ice Blizzard, Steampunk, Biohazard, Vaporwave, Void Walker, Thunderbird, Mecha Titan, Bubblegum, Vampire Bat, Ronin Warrior, 8-Bit Retro, Solar Flare, Deep Abyss, Peppermint King, Dark Knight, Prism Bird, and God Muhib*.
     - Dynamic visual accessories rendered in real-time: Royal Crowns, Holy Halos, Demon Horns, Crimson Ninja Bandanas, Aviator Goggles, and Cyber Visors.
   - **14 Particle Wing Trails:** *Classic, Rainbow, Stars, Embers, Neon, Bubbles, Sakura Petals, Plasma Spark, Gold Treasure, Matrix Code, Acid Slime, Ice Shards, Love Hearts, and Void Essence*.
   - **8 Permanent RPG Upgrades:**
     - *Shield Mastery:* Starting shield chance and longer guard protection.
     - *Chrono Feather:* Extended Slow-Mo power-up duration.
     - *Super Magnet:* Wider coin pull radius and longer attraction time.
     - *Lucky Treasure:* Boosts spawn rates of Ruby Gems (+5 coins) and 2× Score orbs.
     - *Gold Rush:* Grants up to +100% extra coins on every collection and raises coin spawn frequency.
     - *Fever Surge:* Lengthens Fever Mode duration and accelerates combo building.
     - *Aerodynamics:* Softens peak gravity for smoother maneuvering.
     - *Wide Horizon:* Permanently widens the clearance gap between pipes across all modes.
   - **Revive Hearts:** Buyable consumable items enabling a second-chance continuation on crash.
   - **8 Sky Environments & Themes:** *Sunny Day, Sunset, Night, Neon Cyber, Aurora Borealis, Fiery Volcano, Deep Cosmos, and Desert Oasis* with automated cycle options.
   - **8 Dynamic Weather Conditions:** *Clear, Falling Petals, Rain, Snow, Fireflies, Floating Embers, and Stardust*.

10. **Daily Missions & Streak Rewards**
    - Tracks consecutive daily login streaks with accumulating coin gifts.
    - Three daily challenges deterministically seeded per calendar day offering coin bounties.

11. **In-Game Achievements & Trophies**
    - 12 comprehensive achievement milestones (*First Flight, Bronze/Silver/Gold pilot ranks, Ace Pilot, Daredevil close calls, Fever Master, and Style Icon*) awarding coin rewards.

12. **Procedural Web Audio Engine**
    - Zero external sound files required. All flaps, coin jingles, gem chimes, power-up hums, crashes, and fanfare melodies are synthesized on-the-fly via the Web Audio API with volume and haptic controls.

13. **Cross-Platform Standalone Builds via GitHub Actions**
    - **Standalone Android APK (`Flappy-Muhib.apk`):** Native WebViewAssetLoader integration, portrait lock, hardware acceleration, sticky immersive fullscreen, and 100% offline functionality.
    - **Portable Windows Executable (`Flappy-Muhib-Portable.exe`):** Single standalone executable with embedded Chromium, borderless fullscreen, F11 toggle, and 100% offline execution.
    - **Cloud CI/CD Workflow:** Automatically compiles, packages, and attaches releases on every commit without consuming local disk space or battery.

14. **Secret 10-Second God Mode Cheat**
    - Tap and hold the **Settings** dock button for 10 continuous seconds.
    - An animated golden progress bar fills along the button border.
    - Upon completion, God Mode triggers: sets coins to 999,999,999, grants 999 revive hearts, unlocks all 28 skins, unlocks all 14 trails, maxes out all 8 upgrades, completes all achievements, and sets 999 high scores with screen shake and celebration.

15. **Copyright & Attribution**
    - Author: **Yasin Ullah**
    - All rights reserved. Unauthorized copying, cloning, modification, redistribution, or reuse without original author attribution is strictly prohibited.

### How to Play (Controls)
- **Jump / Flap:** Tap the screen, Click the mouse, or press `Spacebar` / `Up Arrow` / `W`.
- **Pause Game:** Click the Pause icon ⏸️, press `Escape`, or press `P`.
- **Quick Restart:** Press `R`.
- **Mute / Unmute:** Click the Speaker icon 🔊 or press `M`.
- **Fullscreen Toggle:** Click the Fullscreen button or press `F11`.

### Modules & Code Architecture
- **DOM & UI Management:** HTML overlays are used for Start, Game Over, Pause, Hangar, Missions, Stats, Achievements, and Settings screens to keep Canvas rendering dedicated to gameplay.
- **Game Engine Loop:** A custom `requestAnimationFrame` loop updates object physics (gravity, velocity, collisions) and draws them to the screen context.
- **Physics Module:** Handles gravity, jump velocity, hitbox scaling, and ceiling/floor/pipe collision detection.
- **Asset Loader:** Preloads all images and sounds before the game starts to prevent mid-game stuttering.
- **PWA Service Worker:** `sw.js` and `pwa-register.js` handle intercepting network requests, caching assets for offline play, and listening to the `beforeinstallprompt` to trigger the app installation flow.
- **Procedural Synthesizer:** Pure mathematical Web Audio oscillators creating lightweight sound effects.
- **CI/CD Build Pipeline:** `.github/workflows/build.yml` orchestrating Android Gradle and Electron Builder jobs.

---

## 🇵🇰 اردو (Urdu Documentation)

### جائزہ (Overview)
**فلیپی محب (Flappy Muhib)** ایک بہترین اور جدید ویب بیسڈ گیم ہے جو مشہور "Flappy Bird" سے متاثر ہو کر بنائی گئی ہے۔ اسے جدید ترین ویب ٹیکنالوجی کا استعمال کرتے ہوئے بہترین پرفارمنس اور دلکش ڈیزائن کے ساتھ تیار کیا گیا ہے۔

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

8. **نئے گیم موڈز (New Game Modes)**
   - **آرکیڈ موڈ (Arcade):** سکے، روبی ہیرے، پاور اپس اور 2 گنا اسکور دینے والا فیور موڈ (Fever Mode)۔
   - **کلاسک موڈ (Classic):** پرانی کلاسیک فلیپی برڈ کا خالص مہارت پر مبنی تجربہ۔
   - **بلٹز موڈ (Blitz 45s):** 45 سیکنڈ کے وقت کے خلاف ریس جس میں پائپوں سے گزرنے پر اضافی وقت ملتا ہے۔
   - **زین موڈ (Zen):** بغیر ہارے پریکٹس کرنے کا موڈ جس میں پرندہ پائپوں سے ٹکرا کر واپس اچھلتا ہے۔

9. **ہینگر اور شاپ کی وسعت (Expanded Hangar & Shop)**
   - **28 منفرد برڈ اسکنز:** کلاسک، ریئر، ایبک، لیجنڈری اور میتھک درجوں کے پرندے۔ ان میں شاہی تاج، فرشتے کا ہالہ، شیطان کے سینگ، ننجا بینڈ، ایوی ایٹر عینک اور سائبر وائزر کے اینیمیشنز شامل ہیں۔
   - **14 ٹریل اسٹائلز:** قوس قزح، ستارے، شعلے، نیون، بلبلے، ساکورا، پلازما، سونے کے سکے، میٹرکس کوڈ، تیزابی سلائم، برف کے ذرات، دل اور تاریک خلا۔
   - **8 مستقل اپ گریڈز:** شیلڈ، سلو موشن، میگنیٹ، لکی ٹریژر، گولڈ رش، فیور سرج، ایروڈائنامکس اور وسیع پائپ گیپ۔
   - **ریوائیو ہارٹس (Revive Hearts):** گرنے کے بعد اسی جگہ سے دوبارہ اڑان شروع کرنے کی سہولت۔
   - **8 آسمانی ماحول اور 8 موسمی اثرات:** دن، غروب، رات، نیون، شفق قطبی (Aurora)، آتش فشاں، کہکشاں اور صحرائی نخلستان۔

10. **روزانہ مشنز اور لاگ ان انعامات (Daily Missions & Streaks)**
    - روزانہ لاگ ان کرنے پر اسٹریک اور سکے کا انعام۔
    - ہر دن کے 3 مختلف چیلنجز جنہیں پورا کر کے کھلاڑی انعامات جیت سکتے ہیں۔

11. **گیم کامیابیاں اور ٹرافیاں (Achievements)**
    - کھیل کے دوران مختلف اہداف مکمل کرنے پر 12 خصوصی اعزازات اور انعامی سکے حاصل ہوتے ہیں۔

12. **خودکار اینڈرائیڈ اور کمپیوٹر فائلز (APK & EXE via GitHub Actions)**
    - **اینڈرائیڈ اے پی کے (Flappy-Muhib.apk):** بغیر انٹرنیٹ کے چلنے والی فل اسکرین موبائل ایپ۔
    - **پورٹیبل ای ایکس ای (Flappy-Muhib-Portable.exe):** کمپیوٹر پر بغیر انسٹال کیے چلنے والی سنگل پورٹیبل گیم۔
    - گٹ ہب ایکشنز کی مدد سے ہر تبدیلی پر خودکار طریقے سے بنتی ہیں۔

13. **10 سیکنڈ کا خفیہ چیٹ کوڈ (Secret God Mode Cheat)**
    - سیٹنگز (Settings) کے بٹن کو 10 سیکنڈ تک دبا کر رکھنے پر چیٹ کوڈ ایکٹو ہو جاتا ہے۔
    - 999,999,999 سکے، 999 ریوائیو ہارٹس، تمام 28 اسکنز، تمام 14 ٹریلز، تمام 8 اپ گریڈز اور تمام مشنز خودکار طریقے سے ان لاک ہو جاتے ہیں۔

14. **کاپی رائٹ اور قانونی ملکیت (Copyright Notice)**
    - مصنف: **یاسین اللہ (Yasin Ullah)**
    - جملہ حقوق بحق یاسین اللہ محفوظ ہیں۔ مصنف کی پیشگی تحریری اجازت اور نام (Attribution) کے بغیر کوڈ یا گیم کو کاپی کرنا، تبدیل کرنا، یا فروخت کرنا سختی سے منع ہے۔

### کھیلنے کا طریقہ (How to Play)
- **اڑنے کے لیے (Jump / Flap):** اسکرین پر ٹیپ کریں، ماؤس سے کلک کریں، یا کی بورڈ سے `Spacebar` / اوپر والا تیر (Up Arrow) / `W` دبائیں۔
- **گیم روکنے کے لیے (Pause Game):** ⏸️ آئیکن پر کلک کریں، یا کی بورڈ سے `Escape` یا `P` کا بٹن دبائیں۔
- **دوبارہ شروع کرنے کے لیے (Quick Restart):** کی بورڈ سے `R` دبائیں۔
- **آواز بند کرنے کے لیے (Mute):** سپیکر کا بٹن دبائیں یا `M` دبائیں۔
- **فل اسکرین کرنے کے لیے (Fullscreen):** اسکرین پر موجود فل اسکرین بٹن دبائیں یا `F11` دبائیں۔

### کوڈ اور ماڈیولز کی ساخت (Modules & Architecture)
- **DOM & UI مینیجمنٹ:** گیم کے مینیو، گیم اوور اور اسٹیٹس کی اسکرینز کے لیے HTML اوورلیز (Overlays) کا استعمال کیا گیا ہے، جبکہ اصل گیم کینوس (Canvas) پر چلتی ہے۔
- **گیم انجن لوپ:** ایک کسٹم `requestAnimationFrame` لوپ فزکس (کشش ثقل، رفتار، ٹکراؤ) کو کنٹرول کرتا ہے اور اسکرین پر چیزوں کو ڈرا کرتا ہے۔
- **فزکس ماڈیول:** پرندے کے اڑنے، گرنے اور پائپوں سے ٹکرانے کا حساب لگاتا ہے۔
- **PWA سروس ورکر:** `sw.js` نیٹ ورک کی درخواستوں کو کنٹرول کرتا ہے، انٹرنیٹ کے بغیر کھیلنے کے لیے فائلز کو کیش (Cache) کرتا ہے، اور ایپ انسٹالیشن کو منظم کرتا ہے۔
- **پروسیجرل آڈیو سنتھیسائزر:** ریاضیاتی طریقوں سے بغیر کسی ایکسٹرنل آڈیو فائل کے حقیقی آوازیں بناتا ہے۔
- **سی آئی ڈی سی بلڈ پائپ لائن:** `.github/workflows/build.yml` کلاؤڈ میں خودکار طریقے سے اے پی کے اور ای ایکس ای فائلز تیار کرتی ہے۔

---

### Open Source Contribution
This project is open-source. Feel free to explore the code, learn from the architecture, and contribute to making it even better.

**Client Notes:** 
*This comprehensive document outlines the full scope, scale, and feature completeness of the Flappy Muhib application. The application is completely deployment-ready, supports advanced offline PWA installations, dynamically handles all display resolutions, and possesses a modular, lightweight codebase.*
