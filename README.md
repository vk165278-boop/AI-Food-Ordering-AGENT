

##  Brief One Line Summary

An AI chatbot built using n8n and Google Gemini that helps users place orders, get restaurant information, and check order status.

---

#  Overview

This project is a simple AI-powered restaurant chatbot created using **n8n automation** and **Google Gemini AI**.

The chatbot interacts with customers and provides quick responses for common restaurant queries. It can guide users to place an order, answer FAQs, and check order or stock information.

---

#  Problem Statement

Restaurants receive many repeated questions from customers like:

- What is on the menu?
- How can I place an order?
- Is my order ready?
- What are your opening hours?

Answering these questions manually takes time.

This chatbot automates these tasks and provides instant responses, improving customer experience.

---

#  Dataset

This project does not use a traditional dataset.

Instead, it uses:

- User chat messages
- Restaurant menu information
- FAQ details
- Order and stock information stored in Google Sheets (optional)

---

# Tools and Technologies

- **n8n** – Workflow Automation
- **Google Gemini** – AI Model
- **Simple Memory** – Stores previous conversation
- **Google Sheets** – Stores restaurant data
- **AI Agent Node** – Processes user queries
- **Chat Trigger** – Starts the chatbot conversation

---

#  Methods

### Step 1: User sends a message

The chatbot starts when a user types a message.

### Step 2: Chat Trigger

The Chat Trigger node receives the user's message.

### Step 3: AI Agent

The AI Agent understands what the user wants.

### Step 4: Memory

Simple Memory keeps track of previous messages so the chatbot can have a natural conversation.

### Step 5: Google Gemini

Google Gemini generates an intelligent response based on the user's request.

### Step 6: Response

The chatbot replies with options like:

-  Place an Order
-  FAQ / Information
-  Check Order / Stock

---

#  Key Insights

- Automates restaurant customer support
- Provides instant AI-generated responses
- Maintains conversation history
- Can be connected with Google Sheets
- Built using a low-code platform (n8n)
- Easy to customize and expand

---

#  Dashboard / Model / Output

### Workflow

```
User Message
      │
      ▼
Chat Trigger
      │
      ▼
AI Agent
      │
 ┌────┴────┐
 │         │
 ▼         ▼
Memory   Google Gemini
      │
      ▼
Response to User
```


```

---

#  How to Run this Project?

### 1. Install n8n

```
npm install -g n8n
```

### 2. Start n8n

Windows PowerShell:

```
& "$env:APPDATA\npm\n8n.cmd"
```

### 3. Import the Workflow

- Open n8n
- Click **Import Workflow**
- Select the workflow JSON file

### 4. Add Credentials

Configure:

- Google Gemini API Key
- Google Sheets Credentials (if used)

### 5. Execute the Workflow

Click **Execute Workflow** and start chatting with the restaurant bot.

---

#  Results & Conclusion

The chatbot successfully handles basic restaurant queries without human intervention.

It provides quick responses, improves customer support, and demonstrates how AI can be combined with automation tools like n8n.

This project is a great beginner-friendly example of AI automation.

---

#  Future Work

- WhatsApp Integration
- Telegram Bot
- Online Payment Support
- Real-time Order Tracking
- Database Integration
- Voice Assistant
- Admin Dashboard

---

#  Author & Contact

**Author:** Vansh Kumar

**Skills Used:** n8n, Google Gemini, Google Sheets, AI Automation

**Email:** vk165278@gmail.com
