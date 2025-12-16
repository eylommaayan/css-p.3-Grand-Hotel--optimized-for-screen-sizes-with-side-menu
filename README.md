
<img width="1906" height="926" alt="image" src="https://github.com/user-attachments/assets/3247c94b-6ddc-4d0c-97c4-9d359f9f77f9" />
<img width="1900" height="902" alt="image" src="https://github.com/user-attachments/assets/16843831-17d2-4d65-ae6d-89b02f51cd6e" />
<img width="1692" height="957" alt="image" src="https://github.com/user-attachments/assets/e58763be-3f0a-4aad-9a66-6f52ce2e76de" />
<img width="1796" height="907" alt="image" src="https://github.com/user-attachments/assets/694441a7-ba3b-4fe4-b154-f854f4e636cc" />
<img width="1806" height="923" alt="image" src="https://github.com/user-attachments/assets/e028bc0c-a9f7-4972-b90e-9ad6bc5db2e3" />.

---

# 🏨 אתר תרגול CSS – “מלון כיף בטבריה”

פרויקט תרגול לבניית אתר תדמית בסגנון **Landing Page** עם:

* ✅ **תפריט צד קבוע (Sidebar)**
* ✅ **תפריט נפתח (Navigation Drawer) בעזרת Checkbox**
* ✅ **Hero Header עם תמונת רקע + טקסט וכפתור**
* ✅ **Sections: About / Rooms / Customers / Footer**
* ✅ **Responsive (Media Queries)**

---

## 🎯 מטרת הפרויקט

להדגים שליטה ב־CSS אמיתי דרך פרויקט מלא:

* להבין Layout נכון עם `flex` ו־`position: fixed/absolute`
* לבנות תפריט נפתח *בלי JavaScript*
* לעבוד עם שכבות (`z-index`) ורקעים (`background + gradient`)
* לבנות אתר שנראה “כמו מוצר אמיתי” ולא רק תרגילים קטנים

---

## ✅ מה נלמד בקורס / בפרויקט

### 1) יסודות CSS ועבודה נכונה

* `box-sizing: border-box`
* עבודה עם `rem` ו־`html { font-size: 62.5% }`
* היררכיית סלקטורים + class names

### 2) Layout מקצועי

* Flexbox:

  * `display: flex`
  * `flex-direction`
  * `justify-content`
  * `align-items`
* חלוקת עמוד ל־Sections בצורה מסודרת

### 3) Sidebar קבוע + תפריט נפתח

* Sidebar קבוע עם:

  * `position: fixed`
  * `height: 100%`
* פתיחה/סגירה של תפריט באמצעות checkbox:

  * `.checkbox:checked ~ .navigation { left: 8rem; }`
* אנימציית “המבורגר” → X בעזרת:

  * `transform: rotate(...) translate(...)`
  * `opacity: 0`

### 4) רקעים ותמונות

* `background: linear-gradient(...), url(...) center no-repeat`
* `background-size: cover`
* שימוש ב־overlay כדי לשפר קריאות טקסט

### 5) טיפוגרפיה ואייקונים

* Google Fonts
* Font Awesome Icons
* Hover effects

### 6) כרטיסים (Cards)

* Rooms cards עם:

  * `box-shadow`
  * כפתורים עם Hover
* Customers cards עם תמונה + טקסט

### 7) תמונות בשכבות (About Us Images)

* `position: absolute` + `transform: translate(...)`
* `overflow: hidden` כדי למנוע “בריחה” של תמונות מחוץ לאזור

### 8) Responsive Design

* Media Queries לדוגמה:

  * `@media(max-width: 1400px)`
  * `@media(max-width: 1200px)`
  * `@media(max-width: 900px)`
  * `@media(max-width: 750px)`

---

## 🧩 מבנה הפרויקט

```bash
project/
├─ index.html
├─ css/
│  └─ style.css
└─ img/
   ├─ header-1.jpg
   ├─ nav-bg.jpeg
   ├─ crown.png
   ├─ about-us-img-1.jpeg ...
   ├─ single-room.jpeg ...
   └─ gallery-img-1.jpeg ...
```

---

## ▶️ איך מריצים מקומית

1. מורידים/משכפלים את הפרויקט:

```bash
git clone <repo-url>
```

2. פותחים את `index.html` בדפדפן
   (או עם Live Server ב-VSCode)

---

## 🖼️ איך האתר נראה עם CSS

האתר כולל:

* תפריט צד קבוע עם אייקונים
* תפריט נפתח עם חיפוש וקישורים
* Header עם תמונת רקע + כפתור
* About עם תמונות בשכבות
* Rooms עם Cards
* Customers עם כרטיסי ביקורת
* Footer עם מידע, טופס וגלריה

📌 מומלץ להוסיף צילומי מסך:

* `screenshots/home.png`
* `screenshots/menu-open.png`
* `screenshots/rooms.png`

---

## ⬇️ למטה: דוגמה של HTML רגיל (בלי CSS)

הדוגמה הבאה מראה איך האתר נראה “נטו” HTML — בלי עיצוב, בלי layout, רק מבנה:

```html
<!DOCTYPE html>
<html lang="he">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>מלון כיף בטבריה - HTML בלבד</title>
</head>
<body>

  <header>
    <h1>מלון כיף בטבריה</h1>
    <p>ברוכים הבאים למלון כיף</p>
    <button>תרשמו</button>
  </header>

  <nav>
    <ul>
      <li><a href="#">בית</a></li>
      <li><a href="#">פרטים עלינו</a></li>
      <li><a href="#">חדרים</a></li>
      <li><a href="#">אירועים</a></li>
      <li><a href="#">שירות לקוחות</a></li>
      <li><a href="#">צור קשר</a></li>
    </ul>
  </nav>

  <main>
    <section>
      <h2>עלינו</h2>
      <p>
        מלון כיף בטבריה מציע חוויית אירוח רגועה מול הנוף, חדרים נעימים, שירות חם
        ומיקום מושלם לטיולים, כנרת ואטרקציות לכל המשפחה.
      </p>
      <button>קרא עוד</button>
    </section>

    <section>
      <h2>חדרים</h2>

      <article>
        <h3>חדר יחיד</h3>
        <p>תיאור קצר...</p>
        <p>מחיר: $99</p>
        <button>Book Now</button>
      </article>

      <article>
        <h3>חדר זוגי</h3>
        <p>תיאור קצר...</p>
        <p>מחיר: $199</p>
        <button>Book Now</button>
      </article>

      <article>
        <h3>Lux</h3>
        <p>תיאור קצר...</p>
        <p>מחיר: $299</p>
        <button>Book Now</button>
      </article>

      <article>
        <h3>VIP</h3>
        <p>תיאור קצר...</p>
        <p>מחיר: $399</p>
        <button>Book Now</button>
      </article>
    </section>

    <section>
      <h2>הלקוחות שלנו</h2>

      <article>
        <h3>מור</h3>
        <p>לקוחה מרוצה</p>
        <p>"החדר היה נקי ומסודר, הצוות היה מדהים והנוף בבוקר פשוט וואו. נחזור שוב!"</p>
      </article>

      <article>
        <h3>מישל</h3>
        <p>לקוחה מרוצה</p>
        <p>"מיקום מצוין, שירות מהיר, ואווירה נעימה מאוד. מומלץ למשפחות."</p>
      </article>
    </section>
  </main>

  <footer>
    <h3>צור קשר</h3>
    <p>eylon@more-ways.co.il</p>
    <p>Tel: 0586659111</p>

    <form>
      <label>הרשם לעדכונים:</label>
      <input type="text" placeholder="האימייל שלך..." />
      <button>הרשם</button>
    </form>
  </footer>

</body>
</html>
```

---
