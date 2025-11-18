# 🔧 دليل التعديلات السريعة - Modern Shot Media

هذا الملف يحتوي على جميع التعديلات التي قد تحتاجها بشكل مباشر ومبسط.

---

## 1️⃣ تغيير رقم الهاتف

### البحث عن: `07718885300`

**في index.html** - استبدل في 4 أماكن:
```html
<!-- 1. في قسم Contact -->
<a href="tel:07718885300">07718885300</a>

<!-- 2. في معلومات الاتصال -->
<a href="https://wa.me/9647718885300">07718885300</a>

<!-- 3. في الفوتر -->
<a href="tel:07718885300">07718885300</a>

<!-- 4. في زر الواتساب -->
<a href="https://wa.me/9647718885300">
```

**في script.js** - استبدل في مكان واحد:
```javascript
const whatsappURL = `https://wa.me/9647718885300?text=${encodedMessage}`;
```

**ملاحظة**: عند تغيير رقم الواتساب، تأكد من إضافة كود الدولة:
- العراق: `964` + رقم الهاتف بدون الصفر
- مثال: `9647718885300`

---

## 2️⃣ تغيير الأسعار

### في index.html - ابحث عن `pricing-price`

**باقة ستارتر**:
```html
<div class="pricing-price">
    <span class="price-amount">250,000</span>  <!-- عدّل هنا -->
    <span class="price-currency">دينار عراقي</span>
</div>
```

**باقة برو**:
```html
<div class="pricing-price">
    <span class="price-amount">350,000 - 400,000</span>  <!-- عدّل هنا -->
    <span class="price-currency">دينار عراقي</span>
</div>
```

**باقة المنهج الكامل**:
```html
<div class="pricing-price">
    <span class="price-amount">حسب الاتفاق</span>  <!-- عدّل هنا -->
    <span class="price-currency">تواصل معنا</span>
</div>
```

---

## 3️⃣ تغيير النسبة المئوية للخصم

### في index.html - ابحث عن `pricing-note`

```html
<div class="pricing-note">
    <i class="fas fa-gift"></i>
    <span>عرض خاص: خصم 50% على أول شهر للمدرسين الجدد</span>
    <!-- عدّل 50% إلى النسبة المطلوبة -->
</div>
```

---

## 4️⃣ إضافة أو تعديل الخدمات

### في index.html - ابحث عن `services-grid`

**نموذج خدمة جديدة**:
```html
<div class="service-card">
    <div class="service-icon">
        <i class="fas fa-star"></i>  <!-- غيّر الأيقونة -->
    </div>
    <h3 class="service-title">اسم الخدمة</h3>
    <p class="service-description">
        وصف الخدمة هنا
    </p>
</div>
```

**أيقونات Font Awesome المتاحة**:
- `fas fa-camera` - كاميرا
- `fas fa-cut` - مقص (مونتاج)
- `fab fa-youtube` - يوتيوب
- `fas fa-search` - بحث (SEO)
- `fas fa-video` - فيديو
- `fas fa-lightbulb` - فكرة
- `fas fa-chart-line` - إحصائيات

**شاهد المزيد**: [fontawesome.com/icons](https://fontawesome.com/icons)

---

## 5️⃣ إضافة أو تعديل روابط السوشيال ميديا

### في index.html - ابحث عن `social-links`

```html
<div class="social-links">
    <!-- فيسبوك -->
    <a href="https://facebook.com/yourpage" class="social-link" title="Facebook">
        <i class="fab fa-facebook-f"></i>
    </a>
    
    <!-- انستقرام -->
    <a href="https://instagram.com/yourprofile" class="social-link" title="Instagram">
        <i class="fab fa-instagram"></i>
    </a>
    
    <!-- يوتيوب -->
    <a href="https://youtube.com/@yourchannel" class="social-link" title="YouTube">
        <i class="fab fa-youtube"></i>
    </a>
    
    <!-- تيك توك -->
    <a href="https://tiktok.com/@yourusername" class="social-link" title="TikTok">
        <i class="fab fa-tiktok"></i>
    </a>
    
    <!-- تويتر (X) - اختياري -->
    <a href="https://twitter.com/yourhandle" class="social-link" title="Twitter">
        <i class="fab fa-twitter"></i>
    </a>
    
    <!-- سناب شات - اختياري -->
    <a href="https://snapchat.com/add/yourusername" class="social-link" title="Snapchat">
        <i class="fab fa-snapchat"></i>
    </a>
</div>
```

---

## 6️⃣ تغيير الألوان الأساسية

### في styles.css - أول 10 أسطر

```css
:root {
    --primary-yellow: #F9C80E;  /* غيّر لون الأصفر هنا */
    --primary-green: #00B67A;   /* غيّر لون الأخضر هنا */
    --dark-bg: #000000;         /* لون الخلفية الداكنة */
    --light-bg: #ffffff;        /* لون الخلفية الفاتحة */
    --text-dark: #1a1a1a;       /* لون النص الداكن */
    --text-light: #666666;      /* لون النص الفاتح */
}
```

**اختيار ألوان**:
- [Coolors.co](https://coolors.co/) - مولد ألوان
- [Color Hunt](https://colorhunt.co/) - لوحات ألوان جاهزة

---

## 7️⃣ تعديل النصوص الأساسية

### العنوان الرئيسي (Hero Title):
```html
<h1 class="hero-title">
    حوّل منهجك إلى محتوى احترافي على يوتيوب
    <!-- عدّل النص هنا -->
</h1>
```

### الوصف (Hero Description):
```html
<p class="hero-description">
    Modern Shot Media تساعد مدرّسي السادس الإعدادي...
    <!-- عدّل النص هنا -->
</p>
```

### نص "من نحن":
```html
<p class="about-description">
    Modern Shot Media فريق متخصص...
    <!-- عدّل النص هنا -->
</p>
```

---

## 8️⃣ إضافة أو حذف أسئلة من FAQ

### في index.html - ابحث عن `faq-item`

**نموذج سؤال جديد**:
```html
<div class="faq-item">
    <button class="faq-question">
        <span>السؤال هنا؟</span>
        <i class="fas fa-chevron-down"></i>
    </button>
    <div class="faq-answer">
        <p>الإجابة هنا.</p>
    </div>
</div>
```

**لحذف سؤال**: احذف كامل كتلة `<div class="faq-item">` إلى `</div>`

---

## 9️⃣ تعديل آراء المدرسين

### في index.html - ابحث عن `testimonial-card`

**نموذج رأي جديد**:
```html
<div class="testimonial-card">
    <div class="testimonial-quote">
        <i class="fas fa-quote-right"></i>
    </div>
    <p class="testimonial-text">
        "نص الرأي هنا..."
    </p>
    <div class="testimonial-author">
        <div class="author-avatar">
            <i class="fas fa-user-tie"></i>
        </div>
        <div class="author-info">
            <h4 class="author-name">اسم المدرس</h4>
            <p class="author-title">مدرس المادة - المرحلة</p>
        </div>
    </div>
    <div class="testimonial-rating">
        <i class="fas fa-star"></i>
        <i class="fas fa-star"></i>
        <i class="fas fa-star"></i>
        <i class="fas fa-star"></i>
        <i class="fas fa-star"></i>
    </div>
</div>
```

**لتغيير التقييم**: احذف أو أضف نجوم `<i class="fas fa-star"></i>`

---

## 🔟 تغيير الخطوط

### في index.html - في قسم `<head>`

```html
<!-- الخط الحالي: Cairo -->
<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@300;400;600;700;900&display=swap" rel="stylesheet">

<!-- خطوط بديلة -->
<!-- Tajawal -->
<link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@300;400;500;700;900&display=swap" rel="stylesheet">

<!-- Almarai -->
<link href="https://fonts.googleapis.com/css2?family=Almarai:wght@300;400;700;800&display=swap" rel="stylesheet">

<!-- IBM Plex Sans Arabic -->
<link href="https://fonts.googleapis.com/css2?family=IBM+Plex+Sans+Arabic:wght@300;400;500;600;700&display=swap" rel="stylesheet">
```

### في styles.css:
```css
body {
    font-family: 'Cairo', sans-serif;  /* غيّر اسم الخط هنا */
}
```

---

## 1️⃣1️⃣ إضافة قسم جديد

**الخطوة 1**: أضف HTML في `index.html`:
```html
<section class="my-section" id="my-section">
    <div class="container">
        <div class="section-header">
            <h2 class="section-title">عنوان القسم</h2>
            <div class="title-underline"></div>
        </div>
        <div class="section-content">
            <!-- محتوى القسم هنا -->
        </div>
    </div>
</section>
```

**الخطوة 2**: أضف CSS في `styles.css`:
```css
.my-section {
    background: white;  /* أو أي لون */
    padding: 80px 0;
}

.section-content {
    /* تنسيقات المحتوى */
}
```

**الخطوة 3**: أضف رابط في القائمة:
```html
<li><a href="#my-section" class="nav-link">اسم القسم</a></li>
```

---

## 1️⃣2️⃣ تغيير الموقع الجغرافي

### في index.html - ابحث عن "العراق - بغداد"

استبدل بمدينتك:
```html
<p>العراق - بغداد</p>  <!-- عدّل هنا -->
```

---

## 1️⃣3️⃣ تعديل حقول النموذج

### في index.html - ابحث عن `contact-form`

**إضافة حقل جديد**:
```html
<div class="form-group">
    <label for="new-field">
        <i class="fas fa-icon"></i>
        اسم الحقل
    </label>
    <input type="text" id="new-field" name="new-field" required placeholder="نص توضيحي">
</div>
```

**أنواع الحقول**:
- `type="text"` - نص عادي
- `type="email"` - بريد إلكتروني
- `type="tel"` - رقم هاتف
- `type="number"` - أرقام فقط
- `type="date"` - تاريخ

---

## 1️⃣4️⃣ تخصيص رسالة الواتساب

### في script.js - ابحث عن `whatsappMessage`

```javascript
const whatsappMessage = `
مرحباً، أنا ${name}

📚 المادة: ${subject}
🎓 المرحلة: ${grade}
📱 رقم الهاتف: ${phone}

${message ? '💬 الرسالة:\n' + message : ''}

أرغب في الاستفسار عن خدماتكم.
`.trim();

// عدّل النص والأيقونات حسب رغبتك
```

---

## 1️⃣5️⃣ تغيير سرعة الرسوم المتحركة

### في styles.css - ابحث عن `--transition`

```css
:root {
    --transition: all 0.3s ease;  /* غيّر 0.3s لتسريع أو تبطيء */
}

/* أو للرسوم المتحركة الخاصة */
.hero-image-wrapper {
    animation: float 6s ease-in-out infinite;  /* غيّر 6s */
}
```

---

## 🎨 نصائح التخصيص

### ✅ افعل:
- اختبر التغييرات على متصفحات مختلفة
- احتفظ بنسخة احتياطية قبل التعديل
- اختبر على الموبايل بعد كل تغيير
- استخدم ألوان متناسقة

### ❌ لا تفعل:
- لا تحذف ملفات CSS أو JS
- لا تغيّر البنية الأساسية للـ HTML إلا إذا كنت متأكداً
- لا تستخدم أكثر من 3 ألوان رئيسية
- لا تبالغ في الرسوم المتحركة

---

## 🆘 عند حدوث خطأ

### إذا توقف شيء عن العمل:

1. **تراجع عن آخر تغيير**
2. **امسح cache المتصفح**: `Ctrl + Shift + Delete`
3. **افتح Console**: `F12` → Console → ابحث عن أخطاء بالأحمر
4. **تحقق من الأقواس**: تأكد من أن كل `<div>` له `</div>`

---

## 📝 قالب للنسخ واللصق

### زر جديد:
```html
<a href="#" class="btn btn-primary">
    <i class="fas fa-icon"></i>
    نص الزر
</a>
```

### كارت جديد:
```html
<div class="card">
    <h3>العنوان</h3>
    <p>الوصف</p>
</div>
```

### قسم بخلفية ملونة:
```html
<section style="background: linear-gradient(135deg, #F4C430, #00A651); padding: 60px 0;">
    <div class="container">
        <h2 style="color: white; text-align: center;">العنوان</h2>
    </div>
</section>
```

---

## 🔍 البحث السريع

للعثور على أي عنصر في الكود:
- `Ctrl + F` في محرر النصوص
- ابحث عن الكلمة المفتاحية
- استبدل واحفظ

---

**نصيحة أخيرة**: عدّل بثقة! يمكنك دائماً التراجع عن أي تغيير. 💪

---

**تحتاج مساعدة؟** 📞 07718885300
