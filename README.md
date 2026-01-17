# Tax Wizz – Excel to JSON Converter 🚀

Tax Wizz is a **Flask-based web application** designed to convert tax-related **Excel trade reports** into **structured JSON outputs**. It supports secure user authentication, real-time frontend–backend synchronization, custom conversion templates, and detailed activity tracking, making it suitable for financial data processing and tax automation workflows.

---

## ✨ Key Features

* 🔐 **User Authentication & Role Management**
  Secure login system with session handling, role-based access (admin/user), and activity logging.

* 📊 **Excel to JSON Conversion**
  Converts Excel files (`.xlsx`, `.xls`, `.xlsm`, `.xlsb`) into structured JSON formats for:

  * Intraday trades
  * Long-term capital gains

* ⚙️ **Custom Conversion Templates**
  Supports default and compact templates with configurable row ranges and output formats.

* 🔄 **Real-Time Sync Features**

  * Live conversion status updates
  * User activity history
  * Recent file tracking
  * Notifications and analytics

* 🧠 **User Preferences Management**
  Persistent preferences such as theme, notifications, auto-save, and default templates.

* 📁 **File Management & Backups**

  * Secure file uploads and downloads
  * User-specific directories
  * One-click backup creation (ZIP)

* 🧾 **JSON Validation**
  Validates generated JSON against a predefined schema to ensure correctness.

* 🛡️ **Robust Error Handling & Logging**
  Centralized logging, validation checks, and custom error pages (404, 500, file size limits).

---

## 🏗️ Tech Stack

* **Backend:** Python, Flask
* **Data Processing:** OpenPyXL, JSON
* **Security:** Flask Sessions, Werkzeug
* **Frontend:** HTML, CSS, JavaScript (Jinja2 Templates)
* **Utilities:** Logging, Threading, Hashing

---

## 📂 Project Structure

```
Tax-Wizz/
│── app.py
│── templates/
│   ├── login.html
│   ├── index.html
│   ├── error.html
│── static/
│   ├── css/
│   ├── js/
│── uploads/
│── user_data/
│── converted_files/
│── logs/
│   └── app.log
│── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/tax-wizz.git
cd tax-wizz
```

### 2️⃣ Create Virtual Environment (Optional but Recommended)

```bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Run the Application

```bash
python app.py
```

Server will start at:

```
http://localhost:5000
```

---

## 🔑 Default Login Credentials (Demo)

| Role  | Username | Password |
| ----- | -------- | -------- |
| Admin | admin    | admin123 |
| User  | user     | user123  |

> ⚠️ **Note:** Change credentials before deploying to production.

---

## 🔌 API Endpoints (Highlights)

* `POST /convert` – Convert Excel to JSON
* `POST /api/convert/custom` – Convert using custom templates
* `GET /api/files/recent` – Fetch recent files
* `GET /api/sync/status` – Real-time sync status
* `POST /api/backup` – Create user data backup
* `POST /api/validate/json` – Validate JSON schema
* `GET /health` – Application health check

---

## 📈 Output Formats

### Standard Format

* Capital gains (long-term)
* Profit & loss (intraday)
* Metadata (timestamp, version)

### Compact Format

* Trade summaries
* Aggregated P&L
* Simplified structure

---

## 🛠️ Future Enhancements

* Database integration (PostgreSQL / MongoDB)
* OAuth-based authentication
* Cloud storage support (AWS S3)
* Multi-file batch processing
* Frontend dashboard with charts

---

## 👤 Author

**Kushagra Srivastava**
B.Tech (Computer Science & Business Systems) | Data Science & AI

---

## 📜 License

This project is licensed under the **MIT License**.

---

⭐ If you find this project useful, feel free to star the repository!
