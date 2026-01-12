---
layout: page
title: Synthron
description: AI-Powered Custom PC Recommendation Platform.
img:
importance: 1
category: Side Projects
giscus_comments: false
---

## 🛠️ Synthron — Custom PC Recommendation Platform

**Synthron** is a full-stack web application that intelligently recommends custom PC builds based on user requirements such as budget, use-case (gaming, editing, productivity), regional availability, and personal preferences.

The platform combines **AI-driven prompt understanding** with **real-time price scraping** to generate practical, up-to-date PC configurations. It focuses on solving a real-world problem: translating vague user intent into technically compatible and cost-effective hardware builds.

---

## 🧠 System Overview

[Image of a full-stack web architecture diagram featuring React frontend, Django backend, PostgreSQL, Redis, LLaMA 3.2, and Playwright scraper]

- **Frontend:** React with a modern, responsive UI
- **Backend:** Django + Django REST Framework
- **Database:** PostgreSQL
- **Caching:** Redis for temporary storage and faster responses
- **AI Layer:** Local **LLaMA 3.2** model for natural-language prompt parsing
- **Scraping Engine:** Playwright for dynamic content extraction

The backend exposes REST APIs consumed by the frontend, while multiple specialized agents collaborate to generate a final build recommendation.

> 🔍 Current scraping reliability averages **70–75%**, with ongoing improvements planned.

---

## ✨ Key Features

- 🧠 **AI-driven prompt interpretation** using LLaMA 3.2  
- 🔍 **Real-time price and availability scraping** from trusted vendors  
- ⚙️ **Component-specific agents** (CPU, GPU, RAM, Storage, Motherboard)  
- 🌍 **Region-aware pricing** and availability detection  
- 🔐 **JWT-based authentication** with HttpOnly cookies  
- 📦 **User build history** stored and retrievable  
- 🧪 **Compatibility checks** (e.g., socket, chipset validation)  
- ⚡ **Fast, modern UI** built with React and Tailwind CSS  

---

## 🔗 How It Works

1. **User Input**  
   Example:  
   > “I want a gaming PC under $1000 in the USA, preferably AMD-based.”

2. **AI Parsing**  
   The LLM extracts intent, budget, region, and preferences.

3. **Agent Activation**  
   Each component agent independently searches for compatible parts.

4. **Data Collection**  
   - URLs are gathered programmatically  
   - Playwright scrapes live pricing and stock data

5. **Ranking & Selection**  
   Components are ranked based on:
   - Price
   - Availability
   - Compatibility
   - User preferences

6. **Final Build Output**  
   The recommended configuration is rendered on the frontend with links and pricing.

---

## 🌐 Trusted Vendors

- Amazon  
- Newegg  
- Micro Center  
- Scan UK  
- Additional regional retailers  

---

## ⚠️ Current Limitations

- Dynamic anti-bot measures may reduce scraping accuracy  
- Not all queries yield valid results (fallback logic is used)  
- Currency and regional detection are still evolving  

---

## 🔮 Future Improvements

- Improved scraping reliability using AI-assisted heuristics  
- Addition of PSU and PC case recommendations  
- Affiliate tracking integration  
- Admin dashboard for scraping diagnostics  
- OAuth authentication (Google, GitHub)  
- Enhanced DevOps workflows and cloud deployment  

---

## 🧰 DevOps & Deployment Roadmap

- 🐳 Docker-based containerization  
- ⚙️ CI/CD pipelines  
- ☁️ Cloud deployment on AWS  
- 🔄 Infrastructure automation  

---

## 🔗 Link to the CodeBase:

You can explore the source code, view the project structure, or contribute to the development here:  
👉 **[GitHub: Synthron](https://github.com/HopzAlot/Synthron)**

---

## 🤝 Contribution & Contact

This project is actively evolving.  
If you’re interested in contributing or discussing the system design, feel free to reach out:

**Email:** rehasaqib2006@gmail.com