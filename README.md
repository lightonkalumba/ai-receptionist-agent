# 🤖 AI Receptionist Agent

An AI-powered virtual receptionist that handles appointment scheduling using a smart agent, natural language input, and Google Calendar integration.

---

## 🧠 What It Does

This agent automates the appointment booking process by:
- Receiving appointment requests via webhook
- Parsing user inputs (Name, Phone, Email, Date & Time)
- Checking availability in Google Calendar
- Booking the appointment if available
- Suggesting 3 alternatives if the time slot is taken
- Responding with a confirmation or alternative suggestions

---

## ⚙️ Features

- Uses OpenAI (GPT-4o) for natural language processing
- Integrates with Google Calendar for real-time scheduling
- Responds with dynamic messages based on availability
- Designed for 30-minute appointment slots
- Built entirely in n8n using modular nodes

---

## 📂 Project Files

- `AI_Receptionist_Agent.json` — Full n8n workflow
- `README.md` — This file

---

## 🔄 How to Use

1. Import the `.json` workflow into your n8n instance
2. Set up credentials for:
   - **OpenAI** (for AI reasoning)
   - **Google Calendar** (for availability & booking)
3. Configure your webhook to receive appointment requests
4. Deploy and test via a POST request or UI form

---

## 🛡 Rules Embedded in the Agent

- Always check availability before booking
- If unavailable, provide 3 closest alternatives
- If available, confirm booking
- All appointments default to 30 minutes

---

## 📄 License

MIT — Free to use and modify.

---

## 💬 Example Use Case

> “Hi, I’d like to book an appointment with John Doe on June 5th at 3 PM.”

➡️ Response:  
> “The appointment has been booked.”  
> or  
> “The requested time is unavailable, these times are: 3:30 PM, 4:00 PM, 4:30 PM.”

---

Let me know if you want a cool project thumbnail or want to bundle a demo GIF for the GitHub repo.
