# Flask Personal Blog Website

A responsive, multi-page blog website built with **Flask** and **Bootstrap**.  
It features an About page, Contact form with email sending capability, and dynamic blog posts fetched from an external API.

---

## 📌 Features
- **Home Page** – Displays all blog posts dynamically from a JSON API.
- **Single Post View** – Click on a post to read its full content.
- **About Page** – Simple introduction page.
- **Contact Page** – Form that sends messages directly to your email using SMTP.
- **Responsive Design** – Built with Bootstrap for a clean and mobile-friendly UI.

---

## 🚀 Technologies Used
- **Backend**: [Flask](https://flask.palletsprojects.com/)
- **Frontend**: HTML5, CSS3, Bootstrap 5
- **Email Sending**: Python `smtplib` with Gmail SMTP
- **Data Source**: JSON API (via `requests` library)
- **Environment Variables**: `.env` file for sensitive data

---

## 📂 Project Structure

├── main.py # Flask application entry point

├── templates/ # HTML templates

│ ├── index.html # Home page

│ ├── about.html # About page

│ ├── contact.html # Contact form page

│ ├── post.html # Single blog post page

│ ├── header.html # Reusable header

│ └── footer.html # Reusable footer

├── static/ # CSS, JS, and images

├── .env # Environment variables (not included in repo)

└── requirements.txt # Python dependencies

---

## ⚙️ Setup & Installation

1. **Clone the repository**
   bash
   git clone https://github.com/bunyaminenis/flask-blog.git
   cd flask-blog
   
2. **Create and activate a virtual environment**
   python -m venv venv
   source venv/bin/activate      # Mac/Linux
   venv\Scripts\activate         # Windows

3. **Create .env file in the project root:**

   MY_EMAIL=your_email@example.com
   PASSWORD=your_email_password
   TO_EMAIL=destination_email@example.com

4. **Run the app**
   
   python main.py

5. **Open in browser**
   
   http://127.0.0.1:5000
   
---

📧 Email Configuration

This project uses Gmail SMTP for sending emails.

You may need to enable App Passwords or Allow less secure apps in your Google account settings.

---

📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

---


💡 Future Improvements

Add user authentication for posting blogs.

Integrate a database for storing posts instead of an external API.

Add pagination and search functionality.
