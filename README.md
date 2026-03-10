# Sample Streamlit Dashboard

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue)](#)
[![Streamlit](https://img.shields.io/badge/Streamlit-App-FF4B4B)](#)

דוגמה קצרה לדשבורד אינטראקטיבי ב‑**Streamlit** עם גרפים באמצעות **Plotly** וטבלת נתונים עם **pandas**.

---

## תצוגה מקדימה

- כרטיסי KPI (Sales / Revenue / Users / Engagement)
- פילטר בסרגל צד לבחירת מדד
- גרף קו לאורך חודשים
- טבלת נתונים

> טיפ: אפשר להוסיף צילום מסך כאן (למשל `assets/screenshot.png`) ואז להציג אותו כך:  
> `![Dashboard Screenshot](assets/screenshot.png)`

---

## דרישות מקדימות

- **Python 3.10+** (מומלץ)
- Windows / macOS / Linux

---

## התקנה

מומלץ לעבוד עם סביבת עבודה וירטואלית:

```bash
python -m venv .venv
```

הפעלה:

```bash
# Windows (PowerShell)
.venv\Scripts\Activate.ps1
```

```bash
# macOS / Linux
source .venv/bin/activate
```

התקנת תלויות:

```bash
pip install streamlit pandas plotly
```

---

## הרצה

```bash
streamlit run dashboard.py
```

לאחר ההרצה, Streamlit ידפיס כתובת מקומית (לרוב `http://localhost:8501`) לפתיחה בדפדפן.

---

## מבנה הפרויקט

```text
Gitdemo/
├─ dashboard.py   # אפליקציית Streamlit (דשבורד)
└─ test.py        # דוגמת "Hello, World!"
```

---

## התאמה אישית מהירה

- **הוספת/שינוי מדדים**: ערוך את הרשימה ב‑`selected_metric` ואת הנתונים ב‑`data` בתוך `dashboard.py`.
- **שינוי ויזואליזציה**: החלף את `px.line(...)` ל‑`px.bar(...)`, `px.area(...)` וכו'.
- **נתונים אמיתיים**: החלף את יצירת הנתונים המקומית בקריאה ל‑CSV/DB/API והמשך לעבוד עם `df`.

---

## בעיות נפוצות

- **`streamlit` לא מזוהה**: ודא שהפעלת את ה‑venv ושביצעת `pip install ...`.
- **Policy של PowerShell**: אם הפעלת venv נחסמת, אפשר להריץ PowerShell כמנהל ולהריץ:
  - `Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser`

---

## תרומה

תרומות מתקבלות בשמחה:

- Fork
- יצירת Branch
- Pull Request עם תיאור קצר + צילום מסך אם יש שינוי UI

---

## רישיון

אם לא הוגדר רישיון עדיין, אפשר להוסיף `LICENSE` (למשל MIT) לפי הצורך.

