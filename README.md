# Scientific-Calculator-Project


🧮 Enterprise Scientific Calculator using Python

The Enterprise Scientific Calculator is a powerful and professional-grade calculator application built using Python and Tkinter.
It supports basic arithmetic, scientific and engineering functions, trigonometry, logarithmic operations, memory functions, expression history, and keyboard input handling — all within a clean GUI interface.

🚀 Key Features
Category	Functions
Basic Maths	+ , − , × , ÷ , %, √, x², 1/x
Scientific	sin, cos, tan, cot, sec, log, ln, eˣ, π, factorial
Engineering	radian/degree conversion, power functions, modulus
Memory Functions	M+, M-, MR, MC
History Panel	Stores and displays previous calculations
GUI Features	Clear (C), Clear Entry (CE), Keyboard Support
Error Handling	Handles invalid inputs and exceptions
🛠️ Technologies Used
Technology	Purpose
Python	Core programming
Tkinter	GUI development
Math Library	Scientific functions and calculations
PIL / Pillow (optional)	UI icons and button visualization
📂 Project Structure
EnterpriseScientificCalculator/
│
├── scientific_calculator.py     # Main Python application
├── README.md                    # Project documentation
├── requirements.txt             # Dependencies (optional)
├── screenshots/                 # UI screenshots (if added)
└── assets/ (optional)           # Icons/images for GUI

📥 Installation Guide
1️⃣ Clone the Repository
git clone https://github.com/your-username/EnterpriseScientificCalculator.git
cd EnterpriseScientificCalculator

2️⃣ Install Required Modules
pip install pillow


(Optional — only used if icon images are included)

▶️ Run the Calculator
python scientific_calculator.py

📸 User Interface Preview

(Insert a screenshot)
/screenshots/main_ui.png

💻 Sample Code Snippet
import math
from tkinter import *

expression = ""

def press(num):
    global expression
    expression += str(num)
    equation.set(expression)

def equalpress():
    try:
        global expression
        total = str(eval(expression))
        equation.set(total)
        expression = total
    except:
        equation.set("Error")
        expression = ""

def clear():
    global expression
    expression = ""
    equation.set("")

🧠 Concepts Applied
Concept	Usage
OOP (Classes)	Modular GUI and calculation structure
Event Handling	Button clicks and key press integration
Exception Handling	Prevents crashes during invalid inputs
GUI Design	Tkinter Frames, Buttons, Entry, Grid
Math Module	Trigonometric & logarithmic functions
State Management	Expression tracking and history
🌟 Future Enhancements

🔹 Dark / Light Theme toggle
🔹 Graph plotting (using Matplotlib)
🔹 Voice input using SpeechRecognition API
🔹 Convert to Android/Windows EXE using Kivy or PyInstaller
🔹 Enhance UI with CustomTkinter or PyQt

📜 License

This project is licensed under the MIT License.
Feel free to fork, modify, and improve!

🙌 Acknowledgements

💻 Python Official Documentation
📘 Tkinter GUI Guide
🧮 Math Module Resources
