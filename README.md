📧 Priority Email Sorting System

The Priority Email Sorting System is an automated tool that categorizes emails based on their urgency and importance. Using rule-based filtering (keywords + sender identification), it assigns each email a High, Medium, or Low priority.

This helps users automatically organize inboxes, reduce clutter, and ensure that critical messages are never missed.


---

⭐ Key Features

Automatic Prioritization
Uses subject line, keywords, and sender identity to classify emails.

Custom Rule Engine
Modify keywords or add new rules without changing the core logic.

Sender-Based Priority Boost
Important senders (boss, clients, bank, etc.) automatically get higher priority.

Simple CSV Integration
Accepts input emails via CSV and outputs sorted results.

Beginner-Friendly Code
Clean Python implementation suitable for students and developers.



---

🛠 Tech Stack

Python 3

CSV / File I/O

(Optional) IMAP or Gmail API for real inbox integration



---

📂 Project Structure

priority-email-sorter/
│── email_sorter.py        # Main logic for email classification
│── rules.py               # Keyword and sender rules
│── emails.csv             # Input dataset
│── sorted_emails.csv      # Output with assigned priorities
│── README.md              # Documentation


---

⚙️ How It Works

1. System reads each email’s sender and subject.


2. Checks for important keywords like:

“urgent”, “ASAP”, “payment”, “deadline”, “meeting”, etc.



3. Applies priority rules based on sender + keywords.


4. Assigns email to:

🟥 High Priority

🟧 Medium Priority

🟩 Low Priority



5. Saves sorted results in a new CSV file.




---

📊 Example Input (emails.csv)

Sender	Subject

ceo@company.com	Project deadline tomorrow
bank@alerts.com	Payment reminder
friend@gmail.com	Weekend plan



---

📊 Example Output (sorted_emails.csv)

Sender	Subject	Priority

ceo@company.com	Project deadline tomorrow	High
bank@alerts.com	Payment reminder	High
friend@gmail.com	Weekend plan	Low



---

▶️ Running the Program

1. Install Python dependencies

No external libraries required. Python's built-in CSV module is used.

2. Run the script

python email_sorter.py

3. View the results

A new file sorted_emails.csv will be created with priority labels.


---

✨ Customization

Modify Keywords

Edit rules.py to add or remove priority keywords:

HIGH_PRIORITY_KEYWORDS = ["urgent", "payment", "deadline", "important", "meeting"]

Add Important Senders

IMPORTANT_SENDERS = ["ceo@company.com", "bank@alerts.com"]


---

🧩 Future Enhancements

Gmail/Outlook API integration

Machine learning model for automated priority prediction

GUI dashboard for visual email overview

Spam detection module


