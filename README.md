📲 WhatsApp Class Reminder — Automated Messages with AI
💡 I kept forgetting to message my class on WhatsApp before sessions. So I built a small tool that does it for me. You tell it what to say, who to send it to, and when, and it handles the rest using AI.

🔎 Why I Made This
Before every class, I need to send a reminder to my WhatsApp group. Sometimes I forget. Sometimes I remember too late. This tool lets me set it up once and stop thinking about it. The AI writes the message so it doesn't sound copy-pasted every time.

💡 What It Does

🕐 Sends a WhatsApp message at a time and day I choose
✍️ Uses Claude AI to write the message so it sounds natural, not robotic
📲 Sends to a specific contact or group
🔁 Can repeat on a schedule (every Monday at 9am, for example)


🛠️ What It's Built With

Claude AI or any other AI fit for the job writes the message based on a description I give it, what the class is, any updates, and the tone I want
WhatsApp is where the message gets sent
A scheduler checks the time and triggers the message when it's supposed to go out


🔄 How It Works
1. ⚙️  I set a day, time, and what the message should be about
2. 🕐  The scheduler waits until that moment
3. 🤖  The AI writes the message
4. 📲  The message goes out on WhatsApp

🗂️ What's in the Project
whatsapp-reminder/
├── 📄 README.md              ← this file
├── ⚙️  config.json            ← my schedule, group name, tone preference
├── 💻 src/
│   ├── scheduler.js          ← watches the clock and triggers messages
│   ├── ai.js                 ← sends the prompt to the AI and gets the message back
│   └── whatsapp.js           ← handles sending through WhatsApp
└── 📋 logs/
    └── sent.json             ← record of every message that went out

🚀 Getting Started
Step 1: Fill in your settings
Open config.json and add the group or contact name, the day and time to send, and a short description of what the message should say.
Step 2: Connect WhatsApp
The app uses the WhatsApp API (or a WhatsApp-connected tool) to send messages from your account.
Step 3: Run it
Start the scheduler. It will sit quietly and send the message at the right time without you having to do anything.

✏️ Why AI Writes the Message
I could write the same message every week and paste it in. But it starts to look stale. The AI reads my short description and writes something fresh each time, same information, different words. It keeps the reminders from feeling like spam.
`
🛣️ What's Next

 📅 Support for multiple classes with different schedules
 🔁 Dynamic messages that mention the date, session number, or topic automatically
 ✅ Confirmation log so I know the message actually went out
 📊 Simple dashboard to manage everything in one place


Built because I kept forgetting to message my class at the right time.
