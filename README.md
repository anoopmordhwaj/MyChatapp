ChatApp - Real-time Web Chat using Django & WebSockets

🚀 A real-time chat application built with Django, WebSockets, Daphne, and SQLite3. The frontend uses HTML, CSS, and JavaScript.

🛠 Features

✅ Real-time messaging using WebSockets

✅ Django Channels for handling WebSocket connections

✅ User authentication and chat rooms

✅ SQLite3 as the database

✅ Join Chatgroups using room ID.




📌 Installation & Setup


1️⃣ Clone the Repository


Copy code ->


git clone https://github.com/anoopmordhwaj/MyChatapp.git

cd chatapp


2️⃣ Create a Virtual Environment (Recommended)


Copy code ->

python -m venv env
source env/bin/activate  # macOS/Linux
env\Scripts\activate  # Windows

3️⃣ Install Dependencies

Copy code ->

pip install -r requirements.txt

4️⃣ Apply Migrations

Copy code ->

python manage.py migrate

5️⃣ Create a Superuser (Optional for Admin Panel)

Copy code ->

python manage.py createsuperuser


6️⃣ Run the Development Server


Copy code ->

python manage.py runserver

Visit http://127.0.0.1:8000/ in your browser.


🚀 Running with Daphne for WebSockets




Make sure Django Channels, Daphne and restframework are installed and configured in settings.py:


python code


INSTALLED_APPS = [

    "daphne",
    
    'django.contrib.admin',
    
    'django.contrib.auth',
    
    'django.contrib.contenttypes',
    
    'django.contrib.sessions',
    
    'django.contrib.messages',
    
    'django.contrib.staticfiles',
    
    "channels",
    
    "chat",
    
    'rest_framework',
    
]



ASGI_APPLICATION = "chatapp.asgi.application"

📂 Project Structure



chatapp/

│── chat/                  # Chat app

│── chatapp/               # Static files (CSS, JS)

│── media/                 # Media files (Images)

│── templates/             # HTML templates

│── db.sqlite3             # SQLite database

│── manage.py              # Django management script

env                        # Virtual environment

requirements.txt           # Dependencies



💡 Contributing


Feel free to contribute by forking the repo, making improvements, and submitting a pull request! 🚀


![image](https://github.com/user-attachments/assets/b285387d-aa68-4a29-b0ef-c36baba3fcee)
![image](https://github.com/user-attachments/assets/e34ca369-2de3-4777-9391-3cc5eb90bd40)
![image](https://github.com/user-attachments/assets/25ad828e-ebc5-49a0-a0af-65f7e18db1c2)
![image](https://github.com/user-attachments/assets/c22017ad-3766-4e23-96d5-b905b1a90647)

