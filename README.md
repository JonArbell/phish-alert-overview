# PhishAlert: AI-Enhanced URL Protection (Gmail Extension)

## Overview
**PhishAlert** is a browser extension designed to improve email security by helping users identify potential phishing links in Gmail. The system monitors user interactions with email links, and when a user hovers over a link, it prompts them to verify the URL's safety, providing warnings if the link is deemed suspicious or safe.

This project is part of our **thesis** on improving online security by integrating phishing detection into email services.


### Features
- Permission-based URL safety checks.
- Responsive UI for security prompts.
- Hover and click detection for enhanced interaction control.
- Clean, user-friendly interface with modal-based user prompts.
- Dynamic feedback system with color-coded modal alerts (Red for Suspicious, Yellow for Error, Green for Safe).
- Secondary verification using OpenAI API for additional link safety analysis.
- Error handling with specific messages for different scenarios.
- Lightweight and efficient, ensuring minimal performance impact while checking URLs.
- Used **Tailwind CSS** for responsive, customizable, and visually appealing design of the extension’s user interface.


### Prerequisites
Before using the **PhishAlert** extension, make sure you have the following installed:

- **Google Chrome** (latest version recommended)
- **Git** for cloning the repository
- A **Gmail account** to test the extension functionality
- **Tailwind CSS CLI** (for styling the extension's UI)


### Installation
**Clone the Repository**
1. ``` git clone https://github.com/JonArbell/phish-alert.git ```
2. ``` cd phishing-detector ```

**Install the Extension**
1. Load the Extension in Chrome
2. Open Chrome and navigate to chrome://extensions/.
3. Enable Developer Mode (toggle in the top right corner).
4. Click Load Unpacked and select the project directory.
5. The extension will be loaded and ready for use in Gmail.

### Usage
1. Open Gmail in your browser.
2. Hover over any email link to trigger the security check prompt.
3. Confirm if you want to check the link for safety.
4. If the link is suspicious, a red modal with the label "Suspicious" will appear. If the link is safe, a green modal with the label "Safe" will appear. If there is an error, a yellow modal with a specific error message will appear.

### Technologies Used
- **JavaScript**: Core functionality for user interactions and dynamic content handling.
- **Tailwind CSS**: Ensures responsive and visually appealing design for the extension's UI.
- **Chrome Extensions API**: Integrates seamlessly with the browser to manage user interactions and permissions.
- **Backend (Java Spring Boot)**: Manages communication between the extension and external APIs securely and efficiently.
  
### APIs
- **Google Safe Browsing API**: Detects unsafe links to protect users from phishing and malware threats.
- **OpenAI API**: Performs secondary verification by analyzing the URL when Google Safe Browsing does not flag it as unsafe. It evaluates various risk factors such as domain structure, URL patterns, content indicators, and potential phishing characteristics to enhance safety validation.


### Additional Notes
- **Compatibility**: The extension is optimized for **Google Chrome**, and other browsers may not fully support the functionality due to API differences.
- **Performance Impact**: The extension is designed to be lightweight with minimal performance impact. However, excessive use of the security checks could slightly impact page load times.
- **Security Considerations**: Always ensure your extension is running on the latest version to prevent security vulnerabilities, especially in handling user interactions and API calls.

  


## Team Members
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

## Technical Writers
- **Ballon, Parizsha Marye** 
- **Bautista, Sebastian Kent** 
- **Cadao, Aaron Charles** 
- **Cruz, Cristina Alexis** 
- **De Ocampo, Jon Arbell**
- **Enierga, Charls** 
- **Luyong, Marialyn** 
- **Pingol, Rose**
- **Playda, Crislie Key**
- **Rodriguez, Reymar**
