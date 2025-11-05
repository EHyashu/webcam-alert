🎥 Webcam Alert System

A real-time motion detection system built with OpenCV and Python that uses your computer’s webcam to monitor activity and send alerts when motion is detected.
Ideal for home surveillance, lab monitoring, or any simple security setup.

🚀 Features

🧠 Motion Detection: Detects movement in front of the webcam using frame differencing.

📸 Automatic Image Capture: Saves frames where motion is detected.

✉️ Email Notifications: Sends an alert email when motion is detected (configurable).

⚙️ Configurable Sensitivity: Adjust the Gaussian blur and threshold for more precise detection.

🧩 Lightweight & Fast: Built purely with Python and OpenCV — no heavy dependencies.

🛠️ Tech Stack

Language: Python 3.x

Libraries: OpenCV, smtplib, email.message, time, os

Tools: VS Code, Git, Virtual Environment

📂 Project Structure
webcam-alert/
│
├── main.py             # Main script that handles webcam feed and motion detection
├── emailing.py         # Handles email alerts
├── .gitignore          # Ignored files (venv, cache, etc.)
├── requirements.txt    # Dependencies list
└── README.md           # Project documentation

⚙️ Setup Instructions
1️⃣ Clone the Repository
git clone https://github.com/<YOUR_USERNAME>/webcam-alert.git
cd webcam-alert

2️⃣ Create and Activate a Virtual Environment
python -m venv venv
venv\Scripts\activate   # (Windows)
source venv/bin/activate # (Mac/Linux)

3️⃣ Install Dependencies
pip install -r requirements.txt


If you don’t have a requirements.txt, create one with:

pip freeze > requirements.txt

▶️ Run the Application
python main.py


Press ‘q’ to quit the webcam window.

The script captures frames where motion is detected and can optionally email you an alert.

📧 Email Alert Configuration

To enable email alerts:

Open emailing.py

Replace with your Gmail credentials (use an App Password, not your real password)

Example:

msg['From'] = "youremail@gmail.com"
msg['To'] = "receiveremail@gmail.com"
smtp.login("youremail@gmail.com", "your_app_password")

📸 Output

Saved images will appear in the /images or /captures folder (depending on your code).

Each file represents a detected motion event.

⚠️ Troubleshooting

Camera not opening: Make sure no other app (Zoom, Teams, etc.) is using the webcam.

Frame empty error: Try changing the index in cv2.VideoCapture(0) → cv2.VideoCapture(1)

Email not sending: Enable “Less secure apps” or use Gmail App Passwords.

💡 Future Improvements

Add real-time notifications (Telegram/WhatsApp bot)

Store motion events in a database

Add GUI interface for non-technical users

Deploy on Raspberry Pi for a mini home surveillance system

🤝 Contribution Guidelines

Contributions are always welcome!
If you'd like to contribute:

Fork the repository

Create a new branch (git checkout -b feature-name)

Commit your changes (git commit -m "Add new feature")

Push the branch (git push origin feature-name)

Open a Pull Request

Please make sure your code is clean, well-documented, and tested before submitting.

📜 License

This project is licensed under the MIT License — you’re free to use, modify, and distribute it with attribution.

MIT License

Copyright (c) 2025 Aryan

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

🧑‍💻 Author

Aryan
AI & Data Science Student | Python & ML Developer
📫 GitHub
 • 💼 LinkedIn
