# 🔒 PhishAlert: AI-Enhanced URL Protection (Gmail Extension)

## 📝 Overview
**PhishAlert** is a browser extension designed to improve email security by helping users identify potential phishing links in Gmail. The system monitors user interactions with email links, and when a user hovers over a link, it prompts them to verify the URL's safety, providing warnings if the link is deemed suspicious or safe.

This project is part of our **thesis** on improving online security by integrating phishing detection into email services.


---

### 🚀 Features
- ✅ Permission-based URL safety checks.
- ✅ Responsive UI for security prompts.
- ✅ Hover and click detection for enhanced interaction control.
- ✅ Clean, user-friendly interface with modal-based user prompts.
- ✅ Color-coded alerts for better visibility:
  - 🟥 Suspicious Link
  - 🟩 Safe Link
- ✅ Secondary verification using OpenAI API for deep link analysis.
- ✅ Error handling with specific messages for different scenarios.
- ✅ Lightweight & efficient, ensuring minimal performance impact.
- ✅ Tailwind CSS for a sleek and modern design.

---


### 🎯 Usage
1. Open Gmail in your browser.
2. Hover over any email link to trigger the security check.
3. A security prompt will appear to confirm the link’s safety.
4. Color-coded modals indicate the URL status:
   - 🟥 Red → Suspicious Link
   - 🟩 Green → Safe Link


---

### 🔁 System Flow
1. **🖥️ Frontend**: The user submits a URL to the backend through a REST API call.
2. **🛠️ Backend**:
    - ✅ Validates the incoming URL.
    - 🔍 Sends the URL to Google Safe Browsing and OpenAI APIs for analysis.
    - 📊 Processes and combines the results into a final verdict.
3. **📡 Broadcast**:
    - 📩 Sends the safety verdict to the frontend for user notifications.
    - 📡 Uses WebClient to transmit the results to the Arduino device for hardware alerts.

---

### 🛠 Technologies Used

#### 💻 Frontend (JavaScript + Tailwind CSS)
  - Connects to the backend using Fetch API.
  - Uses Vanilla CSS for popups and Tailwind CSS for the browser extension UI.
  - JavaScript handles core functionalities and interactions.

#### 🔧 Backend (Spring Boot - Java)
  - Handles API requests and processes responses.
  - Communicates with external services and forwards data to the frontend and Arduino.

#### ⚡ Caching (Caffeine Cache)
  - Enhances performance by storing frequently accessed data in memory.
  - Reduces backend load and improves response times.

#### 🌐 APIs & Integrations
  - 🛡 Google Safe Browsing API – Detects unsafe links to protect users from phishing and malware threats.
  - 🤖 OpenAI API – Performs secondary verification by analyzing the URL when Google Safe Browsing does not flag it as unsafe. It evaluates various risk factors such as domain structure, URL patterns, content indicators, and potential phishing characteristics to enhance safety validation.
  - 🧩 Chrome Extensions API - Seamlessly integrates with the browser to handle user interactions and permissions.


---

### 📂 Repositories
- **Frontend Repository:** [GitHub - PhishAlert Frontend Repository](https://github.com/JonArbell/phish-alert-frontend)  
- **Backend Repository:** [GitHub - PhishAlert Backend Repository](https://github.com/JonArbell/phish-alert-backend)


---


### ⚠️ Additional Notes
- ⚡ **Compatibility**: The extension is optimized for **Google Chrome**, and other browsers may not fully support the functionality due to API differences.
- 🚀 **Performance Impact**: The extension is designed to be lightweight with minimal performance impact. However, excessive use of the security checks could slightly impact page load times.
- 🔐 **Security Considerations**: Always ensure your extension is running on the latest version to prevent security vulnerabilities, especially in handling user interactions and API calls.


---


## 👨‍💻 Team Members
- **Ballon, Parizsha Marye** - Logo Designer
- **Bautista, Sebastian Kent** - Support Funds
- **Cadao, Aaron Charles** - Support Frontend Developer
- **Cruz, Cristina Alexis** - Project Manager
- **De Ocampo, Jon Arbell** - Arduino Developer, Full Stack Developer
- **Enierga, Charls** - Hardware Specialist (Circuit Design)
- **Luyong, Marialyn** - Research Analyst
- **Pingol, Rose** - Research Analyst
- **Playda, Crislie Key** - Research Analyst
- **Rodriguez, Reymar** - Vice Project Manager, Support Frontend Developer, Hardware Specialist (Circuit Design)


---

### ✍️ Technical Writers: All team members contributed to documentation.

---

**🚀 Stay protected from phishing with PhishAlert! 🔐💡**
