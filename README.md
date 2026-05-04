# 🤖 AI Lead Scoring Engine

Automated sales lead scoring system that evaluates and prioritizes leads using GPT-4o before they reach the sales team.

## 🎯 What it does

Instead of a sales rep manually reviewing 100 leads per day, this system automatically scores each new lead and assigns a priority: **HOT / WARM / COLD** — in real-time.

## 🔄 How it works

1. Lead fills out a **Typeform** form (company, budget, urgency, business need)
2. **n8n** webhook triggers the workflow instantly
3. **GPT-4o** analyzes the responses and assigns a score 0-100 with reasoning
4. Lead is saved to **Airtable** with full AI analysis
5. Card is created in **Monday.com** with priority status
6. If score > 75 → instant **Slack** alert to #hot-leads channel

## 🧩 Tech Stack

| Tool | Role |
|------|------|
| Typeform | Lead capture form |
| n8n | Workflow orchestration |
| GPT-4o | AI lead scoring |
| Airtable | Lead database |
| Monday.com | Sales board |
| Slack | Real-time HOT lead alerts |


## 🛠️ Setup

1. Import `workflow.json` into n8n
2. Configure credentials: OpenAI, Airtable, Monday.com, Slack
3. Set up Typeform webhook pointing to n8n webhook URL
4. Activate workflow

## 📸 Workflow Preview

![n8n Workflow]<img width="1877" height="969" alt="image" src="https://github.com/user-attachments/assets/c7cc12cc-d5e3-404e-afb2-f50387a9389e" />
airtable-screenshot.png<img width="1854" height="340" alt="image" src="https://github.com/user-attachments/assets/d61fd19b-6967-4845-8507-930902c21ead" />
monday-screenshot.png<img width="1889" height="562" alt="image" src="https://github.com/user-attachments/assets/a9771ad6-eea1-45ee-8bbc-2281a2b81301" />
slack-screenshot.png<img width="1808" height="667" alt="image" src="https://github.com/user-attachments/assets/be5dcc87-6765-43dc-a71c-bcf76f01d884" />





