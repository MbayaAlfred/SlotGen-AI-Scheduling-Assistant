# 🕐 SlotGen

### Turn daily availability into client-ready booking options in seconds.

**SlotGen** is a client scheduling and communication application built with **Google AI Studio** during my Google AI Professional Certificate journey.

It transforms working-hour availability into structured appointment slots, allows users to select the times they want to offer, and generates client-ready messages for **SMS, WhatsApp/DM, and email**.

> **AI-Assisted Development • Workflow Automation • Scheduling Logic • UX Design**

---

## 📑 Table of Contents

* [Overview](#overview)
* [The Problem](#problem)
* [Solution](#solution)
* [Screenshots](#screenshots)
* [Key Features](#features)
* [How SlotGen Works](#how-it-works)
* [Application Walkthrough](#walkthrough)
* [Technology Stack](#technology)
* [Project Structure](#project-structure)
* [AI-Assisted Development](#ai-development)
* [What I Learned](#lessons)
* [Future Enhancements](#future)

---

<a id="overview"></a>

## 🔎 Overview

Scheduling a client often involves more manual work than expected.

A service provider may know they are available from **9:00 AM to 5:00 PM**, but still needs to calculate appointment intervals, account for breaks and buffers, decide which times to offer, and manually format those options into a client message.

**SlotGen simplifies that workflow.**

The user defines their availability and scheduling preferences. SlotGen generates valid booking options, allows the user to select which appointments to offer, and converts those selections into client-ready communication.

### From availability to communication

```text
Availability
     ↓
Configure Duration & Buffer
     ↓
Generate Booking Slots
     ↓
Select Client Options
     ↓
Generate Message
     ↓
Copy / Share
```

**The goal is simple: spend less time calculating availability and more time serving clients.**

---

<a id="problem"></a>

## 🎯 The Problem

Consider a professional who is available from:

**9:00 AM – 5:00 PM**

and schedules:

**45-minute appointments with a 5-minute buffer.**

Without automation, they need to manually determine:

```text
9:00 AM  – 9:45 AM
9:50 AM  – 10:35 AM
10:40 AM – 11:25 AM
11:30 AM – 12:15 PM
...
```

Then they still need to:

* Decide which appointments to offer
* Type the available times into a message
* Personalize the message
* Format it appropriately
* Send it through the client's preferred communication channel

Doing this once is simple.

Doing it repeatedly for multiple clients becomes an unnecessary administrative task.

---

<a id="solution"></a>

## 💡 Solution

SlotGen turns:

### **Working Hours → Booking Options → Client-Ready Message**

The application provides a guided workflow where users can:

* 📅 Select a booking date
* 🕐 Define available working hours
* ✂️ Configure split shifts
* ⏱️ Select an appointment duration
* ⏳ Add buffer time between appointments
* ⚡ Generate valid booking slots automatically
* ☀️ Quickly select Morning or Afternoon availability
* ✅ Select individual booking options
* 👤 Personalize the message with a client name
* 🌎 Include timezone information
* 💬 Choose a communication format
* 📋 Copy the generated message
* 📱 Continue into the WhatsApp sharing workflow

---

<a id="screenshots"></a>

## 📸 Screenshots

### Welcome to SlotGen

The onboarding experience introduces the application's four-step workflow:

**Availability Window → Appointment Calculation → Quick Picks → Client-Ready Text**

![SlotGen Overview](assets/01-slotgen-overview.png)

---

### Availability & Generated Booking Slots

Users configure their availability, appointment duration, buffer settings, and other scheduling preferences.

SlotGen then calculates the available booking windows.

![SlotGen Availability](assets/02-availability-and-generated-slots.png)

---

### Client-Ready Message

Selected booking slots are transformed into formatted client communication.

Users can personalize the output with information such as the client's name and timezone.

![SlotGen Message](assets/03-client-message-generation.png)

---

### WhatsApp Sharing

The prepared booking message can continue into the WhatsApp sharing workflow for review and sending.

![SlotGen WhatsApp](assets/04-whatsapp-booking-share.png)

---

<a id="features"></a>

## ✨ Key Features

| Feature                         | Description                                                |
| ------------------------------- | ---------------------------------------------------------- |
| 📅 **Date Selection**           | Generate availability for a selected day or multiple dates |
| 🕐 **Availability Windows**     | Define custom start and end times                          |
| ✂️ **Split Shifts**             | Support availability containing breaks                     |
| ⏱️ **Duration Presets**         | 15, 30, 45, 60, and 90-minute appointments                 |
| ⏳ **Buffer Time**               | Add transition time between appointments                   |
| ⚡ **Automatic Slot Generation** | Convert working hours into valid booking intervals         |
| ☀️ **Quick Picks**              | Quickly select Morning or Afternoon slots                  |
| ✅ **Individual Selection**      | Choose exactly which appointments to offer                 |
| 👤 **Client Personalization**   | Include client information in generated messages           |
| 🌎 **Timezone Support**         | Add timezone context when communicating availability       |
| 🕐 **Time Formatting**          | Support user-friendly time display options                 |
| 💬 **Multiple Message Styles**  | Format availability for SMS, WhatsApp/DM, or email         |
| 📋 **Copy to Clipboard**        | Copy generated availability for use elsewhere              |
| 📱 **WhatsApp Sharing**         | Continue the generated message into WhatsApp               |
| 💾 **Saved Defaults**           | Reuse commonly used scheduling settings                    |

---

<a id="how-it-works"></a>

## ⚙️ How SlotGen Works

A typical SlotGen workflow begins with a user's availability.

### Example

```text
Date:                 Tuesday, August 25
Availability:         9:00 AM – 5:00 PM
Appointment Duration: 45 minutes
Buffer:               5 minutes
```

SlotGen applies the scheduling configuration and generates available booking windows.

```text
9:00 AM  – 9:45 AM
9:50 AM  – 10:35 AM
10:40 AM – 11:25 AM
11:30 AM – 12:15 PM

2:00 PM  – 2:45 PM
2:50 PM  – 3:35 PM
3:40 PM  – 4:25 PM
```

The user then decides which of those slots should actually be offered to the client.

```text
Working Hours
      │
      ▼
Scheduling Configuration
      │
      ▼
Slot Calculation
      │
      ▼
Available Booking Slots
      │
      ▼
User Selection
      │
      ▼
Message Formatting
      │
      ▼
Client Communication
```

This separates two important concepts:

**When am I available?**

from:

**Which of those times do I want to offer this client?**

---

<a id="walkthrough"></a>

## 🖥️ Application Walkthrough

### Step 1 — Select a Date

Choose:

* Today
* Tomorrow
* A specific date
* Multi-day availability

---

### Step 2 — Define Availability

Set the start and end of the working window.

Common availability presets make configuration faster, while **Split Shift** supports schedules containing breaks.

---

### Step 3 — Configure Appointment Duration

Choose from common appointment lengths:

```text
15 min | 30 min | 45 min | 60 min | 90 min
```

Optional buffer time can be added between appointments.

---

### Step 4 — Generate Booking Slots

SlotGen calculates the valid appointment windows from the scheduling configuration.

The result is displayed as selectable booking cards.

---

### Step 5 — Select Client Options

Users can select:

* Individual slots
* Morning availability
* Afternoon availability
* Multiple booking options

This gives the user final control over what is actually offered to the client.

---

### Step 6 — Choose the Message Style

The selected appointments can be formatted for different communication scenarios, including:

**Quick Text / SMS**

**Clean Bulleted**

**WhatsApp / DM**

**Professional / Email**

---

### Step 7 — Personalize the Message

Add client-specific information such as:

```text
Client Name
Timezone
Time Format
```

SlotGen generates a ready-to-review client message containing the selected booking options.

---

### Step 8 — Copy or Share

The final message can be copied for use elsewhere or continued into the WhatsApp sharing workflow.

The user remains in control and reviews the message before sending.

---

<a id="technology"></a>

## 🛠️ Technology Stack

SlotGen was developed using an **AI-assisted application development workflow with Google AI Studio and Gemini**.

| Area                    | Technology                              |
| ----------------------- | --------------------------------------- |
| AI-Assisted Development | Google AI Studio                        |
| Generative AI           | Google Gemini                           |
| Frontend                | *To be verified from repository source* |
| Application Logic       | *To be verified from repository source* |
| UI / Styling            | *To be verified from repository source* |
| Source Control          | Git / GitHub                            |
| Deployment              | *To be documented*                      |

> **Note:** The final technology stack will reflect technologies verified directly from the repository source rather than assumptions about AI-generated code.

---

<a id="project-structure"></a>

## 📂 Project Structure

The repository is organized around the SlotGen application and supporting documentation.

```text
SlotGen/
│
├── README.md
│
├── src/
│   └── application source
│
├── assets/
│   ├── 01-slotgen-overview.png
│   ├── 02-availability-and-generated-slots.png
│   ├── 03-client-message-generation.png
│   └── 04-whatsapp-booking-share.png
│
├── docs/
│   └── project documentation
│
├── .gitignore
└── application configuration
```

> This section will be updated to match the final repository structure.

---

<a id="ai-development"></a>

## 🧠 AI-Assisted Development

SlotGen was built while completing the **Google AI Professional Certificate** as a practical exploration of AI-assisted application development.

Rather than limiting AI to question-and-answer interactions, I wanted to explore how AI could help transform an everyday workflow problem into a functional application.

### Development Journey

```text
Real-World Problem
        ↓
Requirements Definition
        ↓
AI-Assisted Prototyping
        ↓
Application Development
        ↓
UI/UX Iteration
        ↓
Testing & Validation
        ↓
Workflow Refinement
        ↓
Functional Application
```

AI-assisted development supported areas such as:

* Requirements refinement
* Rapid prototyping
* Code generation
* UI development
* Feature iteration
* Debugging assistance
* Workflow refinement

However, AI-generated code is not the final engineering decision.

Human judgment remains necessary for:

* Requirements
* Application behavior
* Business rules
* Testing
* Validation
* User experience
* Security
* Responsible deployment

---

<a id="lessons"></a>

## 🎓 What I Learned

One of the most important lessons from building SlotGen was understanding the difference between:

> **Building an application that works for the developer and building an application that another person can confidently use.**

A prototype can rely on assumptions understood by its creator.

A user-facing application cannot.

That realization influenced features such as:

* Guided onboarding
* Clear scheduling controls
* Sensible defaults
* Saved preferences
* Quick-selection options
* Predictable output
* Reset functionality
* Client-ready formatting
* Human review before communication

The project reinforced an important principle of AI-assisted development:

### **AI can accelerate development, but the developer remains responsible for the product.**

The value is not simply that AI generated code.

The value is using AI effectively while continuing to make deliberate decisions about the **problem, workflow, logic, user experience, validation, and final solution**.

---

<a id="future"></a>

## 🚀 Future Enhancements

SlotGen currently focuses on quickly transforming availability into client-ready booking options.

Potential future enhancements include:

* [ ] Google Calendar integration
* [ ] Microsoft Outlook integration
* [ ] Calendar conflict detection
* [ ] Saved user profiles
* [ ] Client preference management
* [ ] Booking confirmation workflow
* [ ] Automated appointment reminders
* [ ] Enhanced timezone handling
* [ ] Multi-user scheduling
* [ ] Mobile optimization
* [ ] Cloud deployment
* [ ] AI-assisted scheduling recommendations

---

## 👨‍💻 About the Developer

**Alfred Charles Mbaya**

**Business Intelligence • Data Engineering • AI**

My professional background centers on designing and delivering enterprise data and analytics solutions using technologies including **Power BI, Microsoft Fabric, SQL, Snowflake, Azure, and modern data platforms**.

SlotGen represents an expansion of that experience into **Generative AI and AI-assisted application development**—applying the same problem-solving approach used in business intelligence and data engineering to building practical AI-enabled applications.

---

## ⭐ Project Purpose

SlotGen is more than a certificate exercise.

It represents my experience taking:

### **A Real Problem → An Idea → AI-Assisted Development → Iterative Engineering → A Usable Application**

This project is part of my continued development at the intersection of **Data, Analytics, and Artificial Intelligence**.
