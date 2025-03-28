# پروژه کنترل صدا با تشخیص دست 🤚🎚️

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![OpenCV](https://img.shields.io/badge/OpenCV-4.5%2B-orange)
![MediaPipe](https://img.shields.io/badge/MediaPipe-0.8%2B-red)

## 📌 معرفی پروژه
این پروژه یک سیستم هوشمند برای تشخیص حرکات دست و کنترل صدا در ویندوز است که با استفاده از:
- **MediaPipe** برای تشخیص نقاط کلیدی دست
- **OpenCV** برای پردازش تصویر
- **pycaw** برای کنترل صدا در ویندوز

## ✨ قابلیت‌های کلیدی
- 👋 تشخیص لحظه‌ای دست در تصویر
- ✌️ شناسایی موقعیت انگشتان
- 🔊 کنترل صدا با حرکات دست
- 📊 نمایشگر بصری میزان صدا
- ⚡ عملکرد با سرعت بالا

## 📂 ساختار فایل‌ها
```
HandTrackingProject/
├── HandTrackingModule.py  # ماژول اصلی تشخیص دست
├── VolumeHandControl.py   # برنامه کنترل صدا
└── README.md             # همین فایل راهنما
```

## 🛠️ راه‌اندازی

### پیش‌نیازها
- پایتون 3.8 یا بالاتر
- وبکم

### نصب کتابخانه‌های مورد نیاز
```bash
pip install opencv-python mediapipe numpy comtypes pycaw
```

## 🚀 نحوه اجرا

### 1. ماژول تشخیص دست
برای اجرای دموی تشخیص دست:
```bash
python HandTrackingModule.py
```

### 2. برنامه کنترل صدا
برای اجرای برنامه کنترل صدا:
```bash
python VolumeHandControl.py
```

## 🎮 روش کنترل صدا
1. دست خود را مقابل وبکم قرار دهید
2. با تغییر فاصله بین **انگشت شست** و **سبابه** صدا را تنظیم کنید:
   - 👌 فاصله کم: صدا قطع
   - 🖐️ فاصله زیاد: حداکثر صدا
3. برای خروج کلید **'q'** را فشار دهید

## ⚙️ جزئیات فنی

### HandTrackingModule.py
- کلاس `handDetector` با متدهای:
  - `findHands()`: تشخیص دست در تصویر
  - `findPosition()`: دریافت مختصات نقاط دست
  - `fingersUp()`: تشخیص انگشتان باز
  - `findDistance()`: محاسبه فاصله بین نقاط

### VolumeHandControl.py
- تبدیل فاصله انگشتان (50-300 پیکسل) به محدوده صدا
- نمایش بصری شامل:
  - درصد صدا
  - نوار حجم صدا
  - شمارنده FPS

## 📝 نکات مهم
- بهترین عملکرد در نور مناسب
- بهینه‌شده برای تشخیص یک دست
- کنترل صدا در ویندوز نیاز به دسترسی admin دارد

## 🤝 مشارکت
پیشنهادات و اصلاحات شما باعث بهبود پروژه می‌شود!

## 📜 مجوز
[MIT](https://choosealicense.com/licenses/mit/)

---

ساخته شده با ❤️ و پایتون  
🔗 ارتباط با من: [GitHub](https://github.com/justbehrad) | [LinkedIn](https://linkedin.com/in/Behrad_ghasemi)
