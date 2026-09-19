🔳 QR Code Generator & Decoder

A simple and interactive Python + Streamlit application to generate and decode QR Codes.

The application allows users to enter a URL or any text/information, generate a QR Code, display it, download it, and decode the generated QR Code.

It also supports uploading an existing QR Code image and decoding it.

Note: This project does not use OpenCV. Image handling is done using Pillow (PIL) and QR decoding is performed using ZXing-C++.

🚀 Live Demo

Deploy this application on Streamlit Community Cloud and access it directly from your browser.

Suggested application name:

PragyanAI QR Code Generator & Decoder

Suggested URL:

https://pragyanai-qr-code-generator-decoder.streamlit.app
✨ Features
1. Generate QR Code

Enter:

Website URL
Text
Contact information
Email
Any other information

Click:

🔳 Generate QR Code

The application generates and displays the QR Code.

2. Download QR Code

After generating the QR Code, users can download it as:

generated_qr_code.png
3. Decode Generated QR Code

Click:

🔍 Decode QR Code

The application reads the generated QR Code and displays the decoded information.

Example:

https://www.pragyanai.com
4. Upload Existing QR Code

Users can also upload an existing:

PNG
JPG
JPEG

QR Code image.

The application detects and decodes the information contained in the QR Code.

5. Clickable URL

If the decoded information is a web URL, the application displays it as a clickable link.

Example:

Decoded Information:

https://www.pragyanai.com

Open Link: https://www.pragyanai.com
🏗️ Application Architecture
                    USER
                      │
                      ▼
              Streamlit UI
                      │
          ┌───────────┴───────────┐
          │                       │
          ▼                       ▼
    Generate QR              Upload QR
          │                       │
          ▼                       ▼
       qrcode                 Pillow
          │                       │
          ▼                       ▼
       Pillow                 ZXing-C++
          │                       │
          ▼                       ▼
     QR Image                 Decode QR
          │                       │
          └───────────┬───────────┘
                      │
                      ▼
              Decoded Information
                      │
                      ▼
                Display Result
🛠️ Technologies Used
Technology	Purpose
Python	Application programming
Streamlit	Web UI
qrcode	QR Code generation
Pillow	Image processing
ZXing-C++	QR Code decoding
📁 Project Structure
pragyanai-qr-code-generator-decoder/
│
├── app.py
│
├── requirements.txt
│
├── README.md
│
└── .gitignore
⚙️ Installation
Step 1 — Clone Repository
git clone https://github.com/YOUR_USERNAME/pragyanai-qr-code-generator-decoder.git

Go to the project directory:

cd pragyanai-qr-code-generator-decoder
Step 2 — Create Virtual Environment
Windows
python -m venv venv
venv\Scripts\activate
macOS / Linux
python3 -m venv venv
source venv/bin/activate
📦 Install Dependencies

Run:

pip install -r requirements.txt

Or install directly:

pip install streamlit qrcode[pil] Pillow zxing-cpp
▶️ Run the Application

Run:

streamlit run app.py

Streamlit will provide a local URL similar to:

http://localhost:8501

Open the URL in your browser.

🧪 How to Use
Step 1 — Enter Information

For example:

https://www.pragyanai.com
Step 2 — Generate QR Code

Click:

🔳 Generate QR Code

The QR Code will appear on the screen.

Step 3 — Download QR Code

Click:

⬇️ Download QR Code

to save the QR Code.

Step 4 — Decode QR Code

Click:

🔍 Decode QR Code

The application will decode the QR Code.

Output:

https://www.pragyanai.com
📤 Decode an Existing QR Code

The application also supports decoding QR Codes created outside the application.

Upload an image:

my_qr_code.png

Then click:

🔍 Decode Uploaded QR Code

The decoded information will be displayed.

🧠 Python Concepts Demonstrated

This project is useful as a practical Python learning project because it combines several concepts.

Python
Variables
Functions
Conditional Statements
Exception Handling
String Processing
File Handling
Libraries
QR Code
QR Code Generation
QR Code Detection
QR Code Decoding
Image Processing
Streamlit
Text Input
Buttons
Columns
Images
File Upload
Download Button
Session State
Status Messages
🔄 Complete Processing Flow
Enter URL / Information
          │
          ▼
     Generate QR
          │
          ▼
      QR Image
          │
          ├──────────────► Download
          │
          ▼
      Decode QR
          │
          ▼
   Decoded Information
          │
          ▼
     Display Result
🔐 Privacy

The application processes QR images within the running application.

No API key is required.

No OpenAI API is required.

No external database is required.

🚀 Deploy on Streamlit Community Cloud
1. Create GitHub Repository

Create a repository named:

pragyanai-qr-code-generator-decoder
2. Upload Files

Upload:

app.py
requirements.txt
README.md
.gitignore

Your GitHub repository should look like:

📁 pragyanai-qr-code-generator-decoder

📄 app.py
📄 requirements.txt
📄 README.md
📄 .gitignore
3. Open Streamlit Community Cloud

Go to:

https://share.streamlit.io/

Sign in using your GitHub account.

4. Create Application

Select:

Create app

Then select:

Repository:
YOUR_USERNAME/pragyanai-qr-code-generator-decoder

Branch:
main

Main file:
app.py

Click:

Deploy
🌐 Deployment

After deployment, Streamlit will provide a URL similar to:

https://pragyanai-qr-code-generator-decoder.streamlit.app

You can share this URL with students, developers, or users.

📚 Learning Extensions

This project can be extended into a larger Computer Vision + AI application.

Level 1
Generate QR Code
Decode QR Code
Download QR Code
Level 2
Upload QR Code
Batch QR Code Decoding
Multiple QR Codes
QR Code History
Level 3
URL Validation
Email QR
Wi-Fi QR
Contact/VCard QR
Location QR
Level 4 — Advanced
QR Code Analytics
Scan Tracking
Database Integration
User Authentication
Dashboard
QR Code Expiry
Dynamic QR Codes
🎓 Student Mini Project

This application can be used as a practical project to teach:

Python
        ↓
Libraries
        ↓
Image Processing
        ↓
QR Code Technology
        ↓
Streamlit
        ↓
Web Application
        ↓
GitHub
        ↓
Cloud Deployment

It demonstrates how a Python program can be converted into a real web application and deployed to the cloud.

👨‍💻 Author

PragyanAI

AI Engineering | Generative AI | Agentic AI | Data Science | Industry Skills

Website:

https://www.pragyanai.com
⭐ Support

If you find this project useful, consider giving the GitHub repository a ⭐.

📄 License

This project is intended for educational and demonstration purposes.
