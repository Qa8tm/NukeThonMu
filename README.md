# NukeThon [Music]
**NukeThon MusicBot** is a telegram userbot for playing songs in telegram voice calls based on Pyrogram and PyTgCalls.

## الاوامر
<details>

### !الاوامر / !اوامري
**Desc:** `رؤيه الاوامر`  
**e.g.**  `!help`  

### ! [اسم الاغنيه | رابط يوتيوب]
**Desc:** `تشغيل اغنيه داخل الاتصال اذا كانت هنالك واحده يوضع في الانتظار`  
**Note:** `او يمكنك الرد على اغنيه بـ !تشغيل, `  
**e.g.**  `!تشغيل ساجده عبيد`, `!تشغيل https://www.youtube.com/watch?v=eIc4mqyN1Q8`   

### !بث [رابط البث]
**Desc:** `تشغيل بث في الاتصال , اذا كان هنالك واحد يوضع في الانتظار`  
**e.g.**  `!بث http://a.files.bbci.co.uk/media/live/manifesto/audio/simulcast/hls/nonuk/sbr_low/ak/bbc_world_service.m3u8`   

### !تخطي / !التالي
**Desc:** `لتخطي الاغنيه`  
**e.g.**  `!تخطي`  

### !انهاء
**Desc:** `انهاء الاغنيه الحاليه`  
**e.g.**  `!انهاء`  

### !الانتظار
**Desc:** `رؤيه الاغاني التي في الانتظار`  
**e.g.**  `!انتظار`  

### !خلط
**Desc:** `لخلط الاغاني في قائمه الانتظار`  
**e.g.**  `!خلط`  

### !الان
**Desc:** `رؤيه الاغنيه الحاليه`  
**e.g.**  `!الان`  

### !تحويل
**Desc:** `تحويل الوضع من (صوت/فيديو)`
**e.g.**  `!تحويل`

### !كتم
**Desc:** `كتم الاغنيه`
**e.g.**  `!كتم`

### !الغاء كتم
**Desc:** `لالغاء كتم الاغنيه`
**e.g.**  `!الغاء كتم`

### !ايقاف 
**Desc:** `لايقافف الاغنيه مؤقتا`
**e.g.**  `!ايقاف`

### !استئناف 
**Desc:** `لاستئناف الاغنيه الحاليه`
**e.g.**  `!استئناف`

### !تكرار
**Desc:** `لتشغيل النكرار`  
**e.g.**  `!تكرار`  

### !هادئ
**Desc:** `لتشغيل الوضع الهادئ`  
**e.g.**  `!هادئ`  

### !اللغه [lang code]
**Desc:** `لوضع لغه البوت`  
**e.g.**  `!اللغه en`  

### !حظر [user id]
**Desc:** `لحظر شخص ما`  
**Note:** `او بالرد !حظر الشخص الذي تريد حظره`  
**e.g.**  `!حظر 111111111`, `!حظر (بالرد)`  

### !الغاء حظر [user id]
**Desc:** `لالغاء حظر شخص ما`  
**Note:** `او بالرد عليه !الغاء حظر الشخص الذي تريد الغاء حظره`  
**e.g.**  `!الغاء حظر 111111111`, `!الغاء حظر (بالرد)`  

### !المحظورين
**Desc:** `لرؤيه المحظورين`  
**e.g.**  `!المحظورين`  

### !استخراج
**Desc:** `لاستخراد  (قائمه )`  
**Note:** `حفظ الملف`  
**e.g.**  `!استخراج`  

### !اضافه
**Desc:** `لاضافه الاغنيه الى قائمه`  
**Note:** `بالرد على المللف`  
**e.g.**  `!اضافه (يالرد)`  

### !قائمه [رابط القائمه]
**Desc:** `لاضافه قائمه من يوتيوب/سبوتيفاي`  
**Note:** `الامر يحتوي على اخطاء`  
**e.g.**  `!قائمه https://open.spotify.com/playlist/3ZgmfR6lsnCwdffZUan8EA`  
</details>

# المميزات
- يمكنك تشغيل فيديوهات يوتيوب فيديوهات, راديو, يوتيوب/سبوتيفاي قوائم او ملفات صوتيه!
- لا انتظار او تاخير!
- قائمه انتظار لا نهائيا!
- تشغيل الاغاني في اكثر ن كروب . اكثر من كروب في الانتظار!

## التشغيل

### On Local
> **يحتاج:**  
> Python3.7+  
> Node.js15+  
> FFmpeg

```bash
git clone github.com/kursadHD/TgMusicBot.git
cd TgMusicBot
mv config.env.example config.env
nano config.env # edit your config file
pip(3) install -r requirements.txt -U
python(3) main.py
```
### على هيروكو
[![Deploy To Heroku](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/Qa8tm/NukeThonMu)

## الفارات 
VARIABLE | DESCRIPTION | REQUIRED/OPTIONAL
------------ | ------------ | -------------
SESSION | كودد بايروكرام. (run `python(3) session.py` or [Generate Session String](https://replit.com/@kursadHD/Pyrogram-String-Session-Generator) ) | مهم
API_ID | ايبي ايدي  (من https://my.telegram.org) | مهم
API_HASH | ايبيهاش  (من https://my.telegram.org) | مهم
SUDO | ايدي الادمن (اذا كان اكثر من ادمن ضع مسافه ثم الايدي الاخر) | اختياري (الاعتيادي: ايدي البوت)
LOG_LEVEL | Log level | Optional (default: error)
DEFAULT_LANG | اللغه | مهم (الاعتيادي: عربي)
DEFAULT_STREAM_MODE | وضع البث يفضل audio (صوت او فيديو) | اختياري (الاعتيادي: audio)

## الاخطاء 
اذا وجدت اي خلل تفضل الى [تلكرام](https://t.me/NukeThonSupport) راسلني
