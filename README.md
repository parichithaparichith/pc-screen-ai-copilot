# **AI-Powered Exam and Interview Copilot**

Welcome to the **AI-Powered Exam and Interview Copilot**, a cutting-edge application designed to assist you during exams, interviews, or any scenario where quick, accurate answers are needed. This tool leverages OpenAI's API to provide instant insights and solutions to questions captured via screenshots. Whether you're preparing for an interview or tackling a challenging exam, this application is your ultimate copilot.

---

## **Key Features**
- **Instant AI Assistance**: Get real-time answers to questions by submitting screenshots.
- **Mobile-Friendly**: Seamlessly connect your mobile device to your PC for easy screenshot capture.
- **Custom Prompts**: Tailor the AI's response by providing specific instructions or prompts.
- **Free to Use**: No hidden costs—just set it up and start using it for free!
- **Privacy-First**: Your data and API key are securely managed locally.
- **History Tracking**: View all your screenshots and AI-generated answers in one place.

---

## **How It Works**

1. **Run the Application in the Background**:
   - Start the application on your PC, and it will run in the background, ready to assist you whenever needed.

2. **Anonymously Take Screenshots Using Your Mobile**:
   - Connect your mobile device to the application via the same Wi-Fi network.
   - Use your mobile to take screenshots of your PC screen without anyone knowing, even if you're sharing your screen.

3. **Generate Answers for Questions in Screenshots**:
   - The application uses OpenAI's GPT model to analyze the screenshot and generate accurate answers to the questions present.

4. **Handle Multi-Page Questions**:
   - If a question spans multiple pages, take multiple screenshots and submit them together. The AI will process all screenshots to provide a comprehensive answer.

5. **Submit Screenshots with Custom Prompts**:
   - Add a custom prompt (e.g., "Explain this question" or "Provide the answer") to guide the AI's response.

6. **View Screenshot History**:
   - All screenshots and their corresponding AI-generated answers are stored locally.
   - Open the history page to review all your previous screenshots and answers at any time.

---

## **Use Cases**

### **1. Anonymously Capture PC Screenshots**
- **Use Case**: If you need to take screenshots of your PC screen without anyone knowing (e.g., during a shared screen session), this application allows you to do so discreetly using your mobile device.

### **2. Monitor Screen Content with AI**
- **Use Case**: Use your mobile to monitor and analyze your PC screen content in real-time. The AI can help you understand complex information or generate answers on the fly.

### **3. Generate Answers for Online Exams**
- **Use Case**: During online exams, quickly capture questions using your mobile, submit them to the AI, and receive accurate answers instantly.

### **4. Interview Preparation**
- **Use Case**: Practice answering interview questions by submitting them to the AI. Use the generated responses to refine your answers and improve your confidence.

### **5. Local Data Storage**
- **Use Case**: All screenshots and AI-generated answers are stored locally on your device, ensuring your data remains private and secure.

---

## **How to Set Up and Run the Application**

### **Prerequisites**
Before you begin, ensure you have the following:

1. **Python 3.11+**:
   - Make sure Python 3.11 or higher is installed on your system.
   - Check your Python version:
     ```bash
     python --version
     ```
   - If Python is not installed, download it from [python.org](https://www.python.org/downloads/).

2. **Install Dependencies**:
   - Install all required dependencies using the `requirements.txt` file:
     ```bash
     pip install -r requirements.txt
     ```

3. **Set Up OpenAI API Key**:
   - Sign up for an OpenAI API key at [OpenAI](https://platform.openai.com/signup/).
   - Add your API key to the application:
     - Open the `settings.ini` file in the project directory.
     - Add your OpenAI API key:
       ```
       OPENAI_API_KEY=your_api_key_here
       ```

4. **Run the Application**:
   - Start the application:
     ```bash
     python main.py
     ```
   - The application will run on `http://localhost:8888`.

### **Run application in the Background**

#### **Linux/Mac**:
- Use `nohup` to run the Flask application in the background and keep it running even after closing the terminal:
  ```bash
  nohup python3 main.py &
  ```
  - The `&` symbol runs the process in the background.
  - Output logs will be saved in the `nohup.out` file by default.

- Alternatively, use a terminal multiplexer like `tmux` or `screen` to manage the process:
  ```bash
  tmux new -s flask_session
  python3 main.py
  ```
  - Detach from the session using `Ctrl+B D` (for `tmux`) or `Ctrl+A D` (for `screen`).
  - Reattach later with `tmux attach -t flask_session`.

- To stop the background process:
  - Find the process ID (PID) using:
    ```bash
    ps aux | grep python
    ```
  - Kill the process using:
    ```bash
    kill <PID>
    ```

---

#### **Windows**:
- Use `pythonw.exe` to run the Flask application in the background without a terminal window:
  ```cmd
  pythonw.exe main.py
  ```
  - This will run the script in the background, and no terminal window will appear.

- To stop the background process:
  - Open **Task Manager**.
  - Locate the `pythonw.exe` process under the **Background Processes** section.
  - Right-click and select **End Task**.

---

## **How to Use the Application**

### **1. Scan QR Code to Open on Mobile**
- Ensure your mobile device is connected to the **same Wi-Fi network** as your computer.
- Open the camera or a QR code scanner app on your mobile device.
- Scan the QR code displayed on the webpage: `http://localhost:8888/connect-mobile`.
- The webpage will open automatically on your mobile browser.

### **2. Open Home Page to Take Screenshot and Submit to AI**
- During an exam or interview, if you encounter a question on the screen:
  1. **Open the Home Page**:
     - Navigate to the home page of the application: `http://<your-local-ip>:8888`.
  2. **Take a Screenshot**:
     - On your mobile device, click the "Take Screenshot" button to capture the question displayed on your PC screen.
  3. **Enter a Custom Prompt**:
     - Enter a custom prompt (e.g., "Explain this question" or "Provide the answer").
  4. **Submit to GPT**:
     - Click the "Submit to GPT" button to send the screenshot and prompt to the AI.
  5. **View the Answer**:
     - The application will generate an answer and display it on the webpage.

---

## **Why Use This Application?**
- **Boost Productivity**: Save time by getting instant answers to complex questions.
- **Interview Prep**: Use it as a free interview copilot to practice and refine your responses.
- **Exam Assistance**: Tackle tough exam questions with confidence and accuracy.
- **User-Friendly**: Simple setup and intuitive interface make it accessible to everyone.
- **Privacy-Focused**: All data is stored locally, ensuring your information remains secure.

---

## **SEO Keywords**
- Free interview copilot
- AI-powered exam assistant
- Instant question solver
- Screenshot to AI answer
- Mobile-PC collaboration tool
- Real-time exam help
- Interview preparation tool
- Anonymous screenshot tool
- Local data storage
---

## **FAQs**

### **Q1: Is this application free to use?**
Yes, the application is completely free to use. You only need an OpenAI API key, which may incur costs based on usage.

### **Q2: Can I use this for interviews?**
Absolutely! This tool is perfect for interview preparation. Use it to practice answering questions or to get real-time assistance during mock interviews.

### **Q3: Is my data secure?**
Yes, your data is processed locally, and your API key is stored securely in the `settings.ini` file. No data is shared with third parties.


## **License**
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## **Support**
If you encounter any issues or have questions, please open an issue on GitHub or reach out to us at [parichithaparichith@gmail.com].

---

**Get started today and transform the way you tackle exams and interviews with the AI-Powered Exam and Interview Copilot!**