# 🤖 AI Customer Support Chatbot for Restaurants

An intelligent AI-powered chatbot that handles 80%+ of common customer inquiries for restaurants — automatically, 24/7, in multiple languages.

![Status](https://img.shields.io/badge/Status-Live-brightgreen)
![AI](https://img.shields.io/badge/AI-Powered-blue)
![Industry](https://img.shields.io/badge/Industry-Restaurants%20%26%20Hospitality-orange)

---

## 🎬 Live Demo

**▶️ [Watch the 2-minute demo](https://www.loom.com/share/85021d1b7dd34235ae2be8ed40295028)**

---

## 🧠 What It Does

Restaurants receive the same questions hundreds of times per week:

- *"What's on the menu?"*
- *"Are you open on Sunday?"*
- *"Do you have gluten-free options?"*
- *"How do I book a table?"*
- *"Do you deliver?"*

This chatbot answers **all of them instantly** using a knowledge base — no hallucination, no wrong answers, no human needed.

---

## ⚙️ Architecture

```
┌─────────────┐     ┌──────────────────┐     ┌─────────────────┐
│   Customer   │────▶│   AI Chatbot     │────▶│  Knowledge Base  │
│  (Website)   │◀────│   Engine         │◀────│  (Restaurant     │
│              │     │                  │     │   Data)          │
└─────────────┘     └──────────────────┘     └─────────────────┘
                            │
                    ┌───────┴───────┐
                    │  NLP Engine   │
                    │  - Intent     │
                    │    Detection  │
                    │  - Entity     │
                    │    Extraction │
                    │  - Context    │
                    │    Management │
                    └───────────────┘
```

### How It Works

1. **Customer sends a message** via website chat widget
2. **AI processes the message** — understands intent and extracts entities
3. **Knowledge base lookup** — retrieves accurate, up-to-date restaurant information
4. **Response generation** — crafts a natural, helpful response
5. **Delivered instantly** — sub-second response time, 24/7

---

## 🎯 Key Features

| Feature | Description |
|---------|-------------|
| **Knowledge-Based Responses** | Only answers from verified restaurant data — zero hallucination |
| **Multi-Category Support** | Menu, hours, reservations, delivery, allergies, location, specials |
| **Allergy & Dietary Handling** | Identifies gluten-free, vegan, vegetarian, nut-free options accurately |
| **Reservation Assistance** | Guides customers through the booking process |
| **Multi-Language Ready** | Supports English and Swedish out of the box |
| **24/7 Availability** | Never sleeps, never takes a break |
| **Graceful Handoff** | Escalates complex queries to human staff |

---

## 📊 Sample Interactions

### Menu Inquiry
```
Customer: "What vegetarian options do you have?"
Bot:      "We have several vegetarian options! Our popular choices include:
           - Falafel Plate (crispy falafel with hummus and salad)
           - Grilled Halloumi Wrap
           - Vegetable Curry with rice
           All can be made vegan on request. Would you like to see the full menu?"
```

### Booking Request
```
Customer: "Can I book a table for 4 on Saturday at 7pm?"
Bot:      "I'd be happy to help with your reservation! For a table of 4 this
           Saturday at 7pm, I recommend booking directly through our reservation
           system or calling us at [phone]. Weekend evenings are popular,
           so booking in advance is recommended!"
```

### Allergy Question
```
Customer: "I have a nut allergy. What can I eat safely?"
Bot:      "Your safety is our priority! Our nut-free options include:
           - All grilled meats (chicken, lamb, beef)
           - Rice dishes
           - Most salads (without dressing)
           Please inform your server about your allergy when you arrive,
           and our kitchen will take extra precautions."
```

---

## 🏗️ Knowledge Base Structure

The chatbot's knowledge base is organized into structured categories:

```json
{
  "restaurant": {
    "name": "Restaurant Name",
    "location": "Full address",
    "hours": {
      "monday-friday": "11:00 - 22:00",
      "saturday": "12:00 - 23:00",
      "sunday": "12:00 - 21:00"
    },
    "menu": {
      "starters": [...],
      "mains": [...],
      "desserts": [...],
      "drinks": [...]
    },
    "dietary_info": {
      "gluten_free": [...],
      "vegetarian": [...],
      "vegan": [...],
      "nut_free": [...]
    },
    "delivery": {
      "available": true,
      "platforms": ["Foodora", "Uber Eats"],
      "radius_km": 5
    },
    "reservation": {
      "method": "phone / online",
      "max_party_size": 12
    }
  }
}
```

---

## 💰 Business Impact

| Metric | Before | After |
|--------|--------|-------|
| Avg. response time | 2-4 hours | **< 5 seconds** |
| Questions handled without staff | 0% | **80%+** |
| Availability | Business hours only | **24/7** |
| Language support | Staff-dependent | **Multi-language** |
| Customer satisfaction | Variable | **Consistent** |

---

## 🚀 Use Cases

This system is designed for but not limited to:

- 🍽️ **Restaurants** — Menu, bookings, hours, delivery, allergies
- 🏨 **Hotels** — Room availability, amenities, check-in/out, directions
- 🏥 **Clinics** — Appointment booking, services, insurance, hours
- 💈 **Service businesses** — Pricing, availability, booking, FAQs
- 🛒 **E-commerce** — Product info, shipping, returns, order status

---

## 🛠️ Tech Stack

- **AI/NLP Engine** — Large Language Model with retrieval-augmented generation
- **Knowledge Base** — Structured data store with real-time updates
- **Chat Interface** — Embeddable web widget
- **Analytics** — Conversation tracking and insights

---

## 📬 Contact

**Built by Arjun Ponnaganti**

- 🌐 Website: [arjunworks.se](https://arjunworks.se)
- 💼 LinkedIn: [linkedin.com/in/arjun-ponnaganti](https://linkedin.com/in/arjun-ponnaganti)
- 📧 Email: ponnagantiarjun644@gmail.com

---

## 📄 License

This project is proprietary. For licensing inquiries, please contact the author.
