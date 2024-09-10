
# شرح أساسيات HTML و CSS

### 1. مقدمة سريعة عن HTML و CSS (10 دقائق)
- **HTML:** الهيكل الأساسي للصفحة، بناء العناصر (Elements) مثل العناوين (Headings)، الفقرات (Paragraphs)، الصور (Images)، والروابط (Links).
- **CSS:** كيفية إضافة التصميم والتنسيق، فصل المحتوى عن التصميم، التعرف على الفكرة وراء الأنماط (Stylesheets).

**مثال:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Basic HTML</title>
    <style>
        h1 {
            color: blue;
        }
    </style>
</head>
<body>
    <h1>Hello, World!</h1>
    <p>This is a basic HTML and CSS example.</p>
</body>
</html>
```
**مهمة بسيطة:** قم بتعديل النصوص والألوان.

---

### 2. Selectors & Specificity (20 دقيقة)
- شرح أهمية الـ **selectors** في CSS.
- شرح الأنواع الأساسية:
    - **Element selectors** (`p {}`)
    - **Class selectors** (`.class {}`)
    - **ID selectors** (`#id {}`)
    - **Attribute selectors** (`[type="text"] {}`)
- التدرجية (specificity) وكيفية تأثير ترتيب الأنماط على التصميم.

**مثال:**
```html
<style>
    p {
        color: red;
    }
    .highlight {
        color: green;
    }
    #special {
        color: blue;
    }
</style>
<p>This is a paragraph.</p>
<p class="highlight">This is a highlighted paragraph.</p>
<p id="special">This is a special paragraph.</p>
```

**مهمة بسيطة:** قم بتغير الألوان و أضف بعض الـ classes و الـ IDs لفهم الانتقائية والتدرجية.

---

### 3. Box Model: Padding, Margin, Border (30 دقيقة)
- شرح مفهوم الـ **box model** وكيف يتعامل CSS مع العناصر كصناديق.
- شرح الفروقات بين:
    - **Padding**: المسافة بين المحتوى وحدود العنصر.
    - **Margin**: المسافة بين العنصر والعناصر الأخرى.
    - **Border**: حدود العنصر.

**مثال:**
```html
<style>
    .box {
        width: 200px;
        height: 100px;
        background-color: lightgray;
        padding: 20px;
        margin: 10px;
        border: 5px solid black;
    }
</style>
<div class="box">This is a box with padding, margin, and border.</div>
```

**مهمة بسيطة:** قم بتجربة تغيير قيم الـ padding والـ margin والـ border.

---

### 4. Positioning: Static, Relative, Absolute, Fixed (30 دقيقة)
- شرح أهمية النظام الافتراضي للموقع (static) وكيف يمكن تغيير موضع العناصر باستخدام:
    - **Relative**: بالنسبة لموقعها الأصلي.
    - **Absolute**: بالنسبة لأقرب عنصر يحتوي على موقع محدد.
    - **Fixed**: يبقى ثابتًا حتى مع التمرير.
    - **Sticky**: يتحرك حتى يصل إلى نقطة معينة ثم يصبح ثابتًا.

**مثال:**
```html
<style>
    .relative {
        position: relative;
        top: 20px;
        left: 30px;
        background-color: lightblue;
    }
    .absolute {
        position: absolute;
        top: 50px;
        left: 100px;
        background-color: lightgreen;
    }
</style>
<div class="relative">I am relative.</div>
<div class="absolute">I am absolute.</div>
```

**مهمة بسيطة:** قم بتحريك العناصر وتغير موضعها باستخدام القيم المختلفة.

---

### 5. Flexbox (40 دقيقة)
- شرح أهمية **flexbox** في ترتيب العناصر بشكل أكثر سلاسة من الطرق التقليدية.
- شرح بعض الخصائص الأساسية:
    - **display: flex**
    - **justify-content** (محاذاة أفقية)
    - **align-items** (محاذاة عمودية)
    - **flex-direction** (تحديد اتجاه العناصر)

**مثال:**
```html
<style>
    .flex-container {
        display: flex;
        justify-content: space-around;
        align-items: center;
        height: 200px;
        background-color: lightcoral;
    }
    .flex-item {
        background-color: lightyellow;
        padding: 20px;
        border: 2px solid black;
    }
</style>
<div class="flex-container">
    <div class="flex-item">Item 1</div>
    <div class="flex-item">Item 2</div>
    <div class="flex-item">Item 3</div>
</div>
```

**مهمة بسيطة:** قم بتغيير الاتجاه والمحاذاة للعناصر، وتجربة القيم المختلفة.

---

### 6. Responsive Design and Media Queries (30 دقيقة)
- شرح أهمية التصميم المستجيب وكيفية استخدام **media queries** لتعديل التصميم بناءً على أحجام الشاشة المختلفة.

**مثال بسيط:**
```css
@media (max-width: 600px) {
    .flex-container {
        flex-direction: column;
    }
}
```

**مهمة بسيطة:** قم بتعديل الكود بحيث يصبح التصميم متجاوبًا مع شاشات أصغر.

---



