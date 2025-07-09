# n8n Email Automation with Google Sheets 📧

This n8n workflow reads contact data from a Google Sheet and sends **personalized emails** to each person using dynamic variables like Name, Company, and a Custom Message.

## 🔄 How It Works

1. **Schedule Trigger** – Starts the workflow manually or on a schedule.
2. **Google Sheets Node** – Reads data from a sheet with columns: `Name`, `Email`, `Company`, `CustomMessage`.
3. **SplitInBatches Node** – Loops through each row (contact).
4. **Send Email Node** – Sends a customized email to each user using template variables.

## 📸 Screenshot

![Workflow Screenshot](Screenshot (2).png)


### ✉️ Email Example

**Subject:**  
`Welcome to {{ $json["Company"] }}, {{ $json["Name"] }}!`

**Body:**  

## 📄 Submission Items

- `workflow.json` – Exported n8n workflow
- `screenshot.png` – Canvas screenshot of workflow
- [Google Sheet Template (View only)](https://docs.google.com/spreadsheets/d/1uKPGf-dZyEA0kbkByrGG0Kl9BDJRvOhWi1W7yHgZr4Y/edit?usp=sharing)

---

✅ Built with 💙 by [Adish Pandya](https://github.com/Adish7Pandya)