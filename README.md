# 🤖 Smart E-Commerce Negotiation Chatbot

This project is a **Flask-based AI-powered chatbot** designed for a smart e-commerce platform. It enables users to:

- 🛍️ Browse products  
- 💬 Negotiate prices using **text or voice**  
- 🧾 Place orders  
- 🗣️ Post and view reviews with **sentiment analysis**  
- 🗄️ Leverage a **modern PostgreSQL backend**

---

## 🚀 Live Demo

🔗 [Click here to view the live app](#)  
⚠️ **Please remember to logout after use.**  
Data for reviews and orders is automatically deleted upon logout to optimize storage.

---

## 📂 Features

### 🔍 Browse Products
- Displays products from `ecommerce.csv`
- Includes name, description, and price

### 🤖 Smart Negotiation
- Negotiate prices via **text or voice**
- Uses basic discount logic with predefined limits
- Responds with synthesized audio using **Google Text-to-Speech (gTTS)**

### 🛒 Place Orders
- Final price is stored post negotiation
- Orders are **timestamped** and **user-specific**

### 📝 Post Review
- Submit review text
- Sentiment analyzed using **VADER** (Positive, Negative, Neutral)
- Stored in **PostgreSQL**

### 👁️ View Reviews & Orders
- View your own reviews and orders
- Displayed in admin-style table format using **Tailwind CSS**

### 🔐 Authentication
- Signup/Login system
- Secure storage of user data in PostgreSQL

### 🧼 Automatic Cleanup
- Voice recordings are **not saved permanently**
- Temp audio files are deleted immediately after processing
- Reviews and orders are deleted **after logout**

---

## 🛠️ Tech Stack

| Layer       | Technology                     |
|-------------|--------------------------------|
| Backend     | Python, Flask                  |
| Frontend    | HTML, Tailwind CSS             |
| AI Features | VADER (NLP), gTTS, SpeechRecognition |
| Database    | PostgreSQL (hosted on Render)  |
| Deployment  | Render                         |

---

## 🗃️ Dataset

- Product data: `Dataset/ecommerce.csv`
- Negotiation price data: `model_cleaned.csv`

---

## 🔒 Security & Constraints

- Hosted on **Render PostgreSQL Free Plan** (1 GB storage limit)
- **Data cleanup** after logout to manage storage efficiently
- **ffmpeg** used for voice conversion
- Compatible with browsers that support **WebM audio recording**

---

## ⚙️ Setup Instructions

### 📁 Clone the Repository

```bash
git clone https://github.com/viveknunavath/Chatbot_AI.git
cd Chatbot_AI
📦 Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
🗄️ Set up PostgreSQL
Get credentials from your Render PostgreSQL dashboard

Update the get_db_connection() function in Main.py with your credentials

▶️ Run the Flask App
bash
Copy
Edit
python Main.py
Open http://localhost:10000 in your browser

👤 Author
Poralla Nagaraju
For questions or collaboration, connect via GitHub or email.

📝 License
This project is licensed under the MIT License.

✨ Thank you for using this smart e-commerce negotiation assistant! ✨

vbnet
Copy
Edit

Let me know if you’d like this README to include images, badges (like build or license), or usage GIFs.







