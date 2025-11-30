# 🚀 Business Location Scouter
## ✨ Business Location Scouter is an MCP server that identifies and ranks the best locations to open a business.

## 🌍 Overview

This project identifies the best city for business by combining real-time search intelligence, macroeconomic indicators, cost metrics, talent availability, and qualitative signals.

The result:
* 👉 A ranked list of cities
* 👉 A short business recommendation summary

Perfect for: startups, franchises, investors, consultants, and anyone who needs clear, data-backed expansion decisions.

---

## ✨ Key Features

### 🔎 Real-Time Intelligence

* Integrates with Tavily Search API for immediate, context-rich insights
* Gathers tourism demand, economic vibrancy, and business activity signals

### 📊 Multi-Signal Scoring Engine

* Weighted scoring using:
* Business density & economic activity
* Tourism flow & food culture signals
* Cost of operations
* Competition trends
* Talent availability

### 🧠 AI-Powered Insights (Claude/OpenAI compatible)

* Summarizes findings for each country/city
* Produces a consolidated opportunity overview

### 🛠️ Extendable Architecture

* Drop in new cities or data sources
* Adjust weights per industry
* Plug in Claude, OpenAI, Groq, or local LLMs
* Export results to HTML, PDF (optional), or API

---

### 📺 Demo Video

🎥 [Watch the Demo on YouTube](https://youtu.be/QjWTyAEODGA?si=OoEcizdhF5mtzRnB)

---

## How to use it

* Edit the claude config file to add the below and save it.
```
{
  "mcpServers": {
    "gradio": {
      "command": "npx",
      "args": [
        "mcp-remote",
        "https://mcp-1st-birthday-business-location-scouter.hf.space/gradio_api/mcp/sse"
      ]
    }
  }
}


```

* Once the MCP server is integrated into the Claude, then in the Claude UI enable the tools.
* **Example prompt to use on MCP client claude**: Example prompt to use on claude: i want to open a bakery in sweden, can you first scout the places and then rank them and then based on that only give me top 3

---

