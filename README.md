# TinyURL Project

ברוכים הבאים לפרויקט TinyURL! הפרויקט הזה הוא שרת לקיצור כתובות URL. בעזרתו תוכלו להמיר כתובות URL ארוכות לקצרות ופשוטות לשימוש.

## תכונות עיקריות
- קיצור כתובות URL ארוכות לכתובות קצרות
- ניהול ובקרה על כתובות URL מקוצרות
- מעקב אחרי מספר הגישות לכתובות המקוצרות

## דרישות מערכת
- Python 3.8 ומעלה
- ספריות Python המפורטות בקובץ `requirements.txt`

## התקנה
1. שיבו את הפרויקט ממאגר GitHub:
    ```bash
    git clone https://github.com/SaraToprowitch/TinyURLProject.git
    cd TinyURLProject
    ```

2. צרו והפעילו סביבה וירטואלית (אופציונלי אך מומלץ):
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # ב-Windows השתמשו ב: venv\Scripts\activate
    ```

3. התקינו את התלויות:
    ```bash
    pip install -r requirements.txt
    ```

## הפעלה
1. הריצו את השרת:
    ```bash
    python app.py
    ```

2. השרת ירוץ על ברירת המחדל בכתובת http://127.0.0.1:5000

## שימוש
### יצירת URL מקוצר
שלחו בקשה מסוג POST לכתובת `/shorten` עם כתובת ה-URL הארוכה שברצונכם לקצר:
```json
{
    "long_url": "https://example.com/some/very/long/url"
}
