# HazardEye
AI-based hazard detection app
HazardEye 🛠️
Tagline: Autonomous Industrial Safety Monitoring
Project Goal:
HazardEye is a fully agentic and autonomous AI system designed to detect hazards in industrial environments, assess risks, generate step-by-step action plans, and provide professional safety reports—all in real-time. It helps prevent accidents, improve compliance, and protect workers before incidents occur.

________________________________________
Features ✨
•	Real-Time Hazard Detection:
Detects fire, gas leaks, electrical faults, missing PPE, and other safety violations from images or live camera feeds.
•	Agentic Risk Analysis:
Calculates risk scores and severity levels for detected hazards.
•	Action Plan Generation:
Uses OpenAI GPT API to generate practical, step-by-step mitigation actions for hazards.
•	Report Generator:
Creates PDF reports summarizing detected hazards, risk levels, and suggested actions.
•	Alerts & Notifications:
Sends instant alerts via WhatsApp and voice notifications for high-risk hazards.
•	Support Agent:
Integrated GPT-powered assistant for guidance and answers about industrial safety.
•	Interactive UI/UX:
Modern, colorful, and responsive interface with multiple pages: Home, Hazard Detection, Action Plans, Reports, About & Contact.
•	Autonomous & Agentic:
Fully autonomous workflow—no manual intervention needed for hazard detection and reporting.
________________________________________




Screenshots 📸
 


 


 


 

 


 


 


 


________________________________________
Installation & Setup 🖥️
1.	Clone the repository:
git clone https://github.com/naveedmazhar4/HazardEye.git
cd HazardEye
2.	Create and activate a virtual environment:
python -m venv venv
venv\Scripts\activate   # Windows
source venv/bin/activate # macOS/Linux
3.	Install dependencies:
pip install -r requirements.txt
4.	Add your OpenAI API Key:
•	Create utils/config.py
OPENAI_API_KEY = "your_openai_api_key_here"
5.	Run the app:
streamlit run app.py
________________________________________
Project Structure 📂
hazardeye/
│
├── app.py                         # Main Streamlit app (UI routing)
├── config.py                      # App settings, constants
├── requirements.txt               # All free Python dependencies
│
├── pages/                         # Multi-page navigation
│   ├── Home.py
│   ├── Detector.py              # Image/video hazard detector
│   ├── Action_Plans.py
│   ├── Reports.py
│   ├── About.py
│   └── Contact.py
│
├── agents/
│   ├── hazard_detector.py         # CNN/YOLO / free ML model
│   ├── action_plan_generator.py   # Agentic AI for action steps
│   ├── report_generator.py        # PDF/HTML report generator
│   ├── agent_orchestrator.py      # Multi-agent workflows
│   └── utils.py                   
│
├── assets/
│   ├── logo.png
│   ├── bg_welcome.jpg                 
│   ├── bg_live.png              
│   └── bg_action.jpg                
├── models/
│   ├── yolov8n.pt         
│   └── labels.txt
│
└── output/
    ├── generated_reports/         # PDF/HTML safety reports
    └── uploads/                   # User-uploaded files________________________________________
Tech Stack 🛠️
•	Python
•	Streamlit (UI/UX)
•	OpenAI GPT-3.5 / Mini 5 (Action Plan & Assistant Agent)
•	YOLOv8 (Hazard Detection)
•	PIL / OpenCV (Image Processing)
•	FPDF (PDF Report Generation)
________________________________________
Future Enhancements 🚀
•	Fully offline hazard detection with edge AI models.
•	Integration with wearable IoT devices for real-time safety monitoring.
•	Multi-language support for global deployment.
•	Advanced analytics dashboard with charts and trends.
________________________________________
Hackathon Use 🏆
HazardEye is perfect for hackathons because it:
•	Is fully autonomous and agentic.
•	Provides a wow-factor UI/UX.
•	Solves a real-world problem: industrial safety and hazard prevention.
•	Demonstrates GPT integration with live AI-generated action plans.
________________________________________
Contact ✉️
Developer: Naveed Ahmed
Email: naveedmazhar04@gmail.com
________________________________________
