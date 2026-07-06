📊 Soft Skills Questionnaire
A dynamic and responsive questionnaire application built to collect user feedback and automatically synchronize data with external cloud tools.

🚀 Features
Data Collection: Gathers user responses efficiently through a clean, modern interface.
Google Sheets/Excel Integration: Sends all submitted form data directly to a spreadsheet in real-time via the SheetMonkey API.
Instant Notifications: Automatically triggers an email notification to the administrator as soon as a new response is submitted.

🛠️ Technologies Used
Frontend: HTML5, CSS3, JavaScript (ES6+)
Integration & Automation: SheetMonkey API / Webhooks (for Excel spreadsheet and email automation)

🧠 JavaScript Architecture & Logic
The core logic of this application focuses on performance and scalability. Instead of hardcoding every single question into the HTML, the interface is generated dynamically using JavaScript:

Dynamic DOM Manipulation: The script reads a data structure (such as an array of objects containing the questions) and handles DOM injection into the quiz container.

HTML Template Utilization: Leverages the modern template HTML tag. The JavaScript clones the template structure, fills it with the specific question data, and appends it to the DOM. This keeps the code clean, dry (DRY principle), and highly maintainable.

State Management: Tracks user progress and score variations dynamically as they interact with the form inputs before submission.

📄 How it Works
The JavaScript renders the questions dynamically using the HTML template structure.

The user answers the questions in the dynamic interface.

Clicking the Enviar (Submit) button triggers a native POST request to the SheetMonkey API endpoint.

The data is instantly recorded in the connected spreadsheet, and an email notification is generated.
