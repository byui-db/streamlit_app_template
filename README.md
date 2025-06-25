# Streamlit CRUD App (SQLite Version)

This is a simple template Streamlit app for performing **CRUD operations** (Create, Read, Update, Delete) on a SQLite database. Designed for educational use — ideal for deploying on **Streamlit Community Cloud**.

---

## 📦 Project Structure

```
.
├── app.py               # Main Streamlit app
├── config.py            # Database/table/column settings
├── requirements.txt     # For deployment
├── database.sqlite      # Your SQLite database (add this)
```

---

## 🚀 How to Use (For Students)

### Step 1: Export Your MySQL DB to SQLite

Use a tool like DB Browser for SQLite **or**:

```bash
# Export MySQL to SQL
mysqldump -u your_user -p your_db > dump.sql

# Convert SQL to SQLite (optional method)
pip install sqlite-utils
sqlite-utils convert dump.sql database.sqlite
```

Place the resulting `database.sqlite` file in this folder.

---

### Step 2: Update Config

Open `config.py` and set:
- `TABLE_NAME` to the name of your table
- `COLUMNS` to the fields you want to show/edit (excluding the `id` column)

---

### Step 3: Run Locally

```bash
pip install -r requirements.txt
streamlit run app.py
```

---

### Step 4: Deploy to Streamlit Cloud

1. Push this repo to GitHub
2. Visit: [https://streamlit.io/cloud](https://streamlit.io/cloud)
3. Log in and click **"New app"**
4. Connect your GitHub repo
5. Click **Deploy**

✅ Done! Your SQLite DB will be bundled with your code and run in the cloud.

---

## 📬 For Educators

This template is meant for:
- Class projects
- Assignments with database components
- Lightweight app demos with local DBs

Want more private app slots or memory? Contact: `support@streamlit.io`

---
