# AI Lead Qualification Agent

Built by **Sunny Abichandani** | DGM, Senior PM @ Bharti Airtel

## 🚀 Live Demo

**[Open the AI Lead Qualification Form](https://sunnyabichandani1-tech.github.io/lead-qualification-agent/)**

---

## Overview

A fully functional AI Lead Qualification Agent that integrates **directly with VAPI** for instant outbound calls. No webhooks, no Make.com, pure API integration.

### How It Works

1. **📝 User fills form** — Name, Phone, Plan selection
2. **🤖 Form triggers VAPI API** — Direct call to VAPI endpoint
3. **📞 Monika agent calls** — Within 60 seconds
4. **🎯 Real-time qualification** — AI converses and qualifies lead

---

## Tech Stack

| Component | Technology |
|-----------|-----------|
| **Voice AI** | VAPI (Outbound Calling) |
| **LLM** | OpenAI GPT-4o Mini |
| **Transcriber** | Deepgram Nova 3 (Multilingual) |
| **Voice Synthesis** | 11labs Multilingual V2 |
| **Frontend** | Vanilla HTML/CSS/JavaScript |
| **Hosting** | GitHub Pages |
| **API** | Direct VAPI REST API (no webhooks) |

---

## VAPI Configuration

**Agent: Monika** (Lead Qualification Specialist)

- **Agent ID**: `ddd7c231-e11a-4199-b5c4-9aab68a4717d`
- **API Key**: `38329966-e64b-4d89-b38c-a4100967a3dd` (Public)
- **API Endpoint**: `https://api.vapi.ai/call`
- **Call Type**: Outbound
- **Language**: English (Multilingual capable)

---

## Features

✅ **No scroll required** — Fits one viewport perfectly  
✅ **Clean modal design** — Inspired by Jio.com  
✅ **Direct VAPI integration** — No intermediaries  
✅ **Plan selection** — With OTT icons (Netflix, Hotstar, Prime)  
✅ **Real-time calls** — Initiated immediately after form submission  
✅ **Mobile responsive** — Works on all devices  
✅ **Builder credentials** — Shows who built this  
✅ **Production-ready** — Deployed on GitHub Pages  

---

## Form Structure

### Step 1: Lead Capture
- Full name
- Mobile number (+91 prefix)
- Plan selection (₹199/month or ₹299/month)

### Step 2: Call Initiation
- Form submits to VAPI API
- Monika agent assigned
- Outbound call initiated to customer's phone

### Step 3: Confirmation
- Success modal shows
- Call details confirmed
- Customer receives call within 60 seconds

---

## API Integration

### Direct VAPI Call

```javascript
POST https://api.vapi.ai/call
Headers: {
  'Authorization': 'Bearer 38329966-e64b-4d89-b38c-a4100967a3dd',
  'Content-Type': 'application/json'
}
Body: {
  'assistantId': 'ddd7c231-e11a-4199-b5c4-9aab68a4717d',
  'phoneNumber': '+91XXXXXXXXXX',
  'customData': {
    'customerName': 'Name',
    'selectedPlan': '299',
    'timestamp': '2026-07-15T...'
  }
}
```

---

## Architecture

```
┌─────────────────────┐
│  Landing Page       │
│  (How it works)     │
└──────────┬──────────┘
           │
      [Get Started]
           │
┌──────────▼──────────┐
│  Form Modal         │
│  (Name, Phone, Plan)│
└──────────┬──────────┘
           │
      [Submit Form]
           │
┌──────────▼────────────────────┐
│  VAPI API Call                │
│  POST /call                    │
│  + Customer Data              │
└──────────┬────────────────────┘
           │
┌──────────▼──────────────────────┐
│  Monika Agent Assigned          │
│  Outbound Call Initiated        │
└──────────┬──────────────────────┘
           │
┌──────────▼──────────────────────┐
│  Customer Phone Rings           │
│  AI Conversation Begins         │
│  Lead Qualified                 │
└──────────────────────────────────┘
```

---

## Deployment

### GitHub Pages

- **Status**: ✅ Live and Active
- **URL**: https://sunnyabichandani1-tech.github.io/lead-qualification-agent/
- **Branch**: `main`
- **Source**: `/` (root)

### How to Deploy

1. Upload `index.html` to repository
2. Go to **Settings** → **Pages**
3. Select **Branch**: `main`, **Folder**: `/`
4. Save and wait 1-2 minutes

---

## Testing the Form

1. **Open**: https://sunnyabichandani1-tech.github.io/lead-qualification-agent/
2. **Click**: "Get Started →"
3. **Fill Form**:
   - Name: Any name
   - Phone: Your actual phone number
   - Plan: Select ₹199 or ₹299
4. **Submit**: "Get AI Call Now"
5. **Wait**: Monika will call within 60 seconds

---

## Performance Metrics

| Metric | Value |
|--------|-------|
| **Agent Cost** | ~$0.11/min |
| **Transcriber Latency** | 280ms |
| **Model Latency** | 540ms |
| **Voice Latency** | 840ms |
| **Total Latency** | ~1,660ms |
| **Page Load Time** | <1s |

---

## Use Cases

✅ **Lead Qualification** — Auto-qualify inbound leads  
✅ **Customer Engagement** — Instant callback for interested customers  
✅ **Sales Acceleration** — Reduce queue time, increase conversion  
✅ **Support Triage** — Route service requests to right team  
✅ **Product Demos** — Schedule demos automatically  
✅ **Event Registration** — Confirm attendance via call  

---

## Author

**Sunny Abichandani**

- **Title**: Deputy General Manager (DGM), Senior Product Manager
- **Company**: Bharti Airtel (10+ years)
- **PM Experience**: 5+ years
- **Specialization**: Fleet Productivity, AI Agents, B2B/D2C Products
- **Career Metrics**: ₹800Cr+ revenue impact, 70% productivity uplift, 80K+ incremental sales

### Connect

- **LinkedIn**: [Profile](https://linkedin.com/in/your-profile)
- **GitHub**: [@sunnyabichandani1-tech](https://github.com/sunnyabichandani1-tech)
- **Email**: [your-email]

---

## License

This project is **open for demonstration and educational purposes**.

Free to fork, use, and modify for your own projects.

---

## Contributing

Found a bug? Have an improvement? Feel free to:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

---

## Roadmap

- [ ] Multi-language support
- [ ] Analytics dashboard
- [ ] Webhook integration for custom handling
- [ ] CRM integration (Salesforce, HubSpot)
- [ ] SMS/WhatsApp as alternate channels
- [ ] Advanced lead scoring
- [ ] Custom agent system prompts

---

**Last Updated**: July 15, 2026

**Status**: ✅ Production Ready
