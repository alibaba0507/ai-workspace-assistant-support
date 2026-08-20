# Chrome Web Store Metadata & Presentation Package

## 1. Chrome Web Store Full Description Copy

### AI Workspace Agent: Your Autonomous Multi-Modal Web Companion

Transform how you read, research, extract, and automate data across the web. **AI Workspace Agent** embeds state-of-the-art AI models—including Google Gemini and OpenRouter models—directly into your browser to turn passive web browsing into an interactive, automated workspace.

---

### 🧠 Autonomous Agentic Mode (ReAct Framework)
Unlike basic summarizers that only read raw text on your screen, our **ReAct Agentic Loop** allows the AI to think, plan, and execute multi-step workflows autonomously:
* **Deep Page Context Analysis:** Scrapes visible text, active selections, or full DOM structures.
* **External Page Extraction:** Instruct the agent to follow relevant links, open background tabs, and aggregate detailed information across multiple sources automatically.
* **Screenshot & Visual Analysis:** Capture visual tab canvases for multimodal inspection.

---

### ⚡ Custom Agent Tools (JavaScript Automation)
Empower your AI agent with custom browser tools. Write lightweight, secure JavaScript snippets in your settings panel to give the agent direct programmatic control over page DOM elements:
* Extract structured data tables into JSON.
* Click specific page elements or filter dense datasets on command.
* Import/Export tool configurations seamlessly using standalone JSON files.

---

### 📰 Smart RSS & Content Intelligence
* Automatically detect XML/RSS feed formats on active tabs.
* Execute two-step relevance analysis: the AI filters feed items matching your intent and fetches full-text articles for synthesized summaries.

---

### ⏰ Scheduled Background Automations
* Set prompts to execute automatically every hour, daily, or weekly.
* Receive native desktop notifications upon task completion.
* Inspect cumulative activity in your built-in **Diagnostic Activity Console** and export logs anytime.

---

### 🔐 Bring Your Own Key (BYOK) & Privacy-First Architecture
* **Direct Provider Connections:** Use your own OpenRouter or Google Gemini API keys.
* **Zero Middleman Data Retention:** Your keys and data reside exclusively in your local browser storage (`chrome.storage.local`).
* **Dark & Light Mode Support:** Built-in theme toggling designed to blend with your native browser workflow.

---

### 🚀 How to Get Started
1. Click **Add to Chrome** and pin the extension icon to your toolbar.
2. Open **Settings (⚙️)** and input your Gemini or OpenRouter API Key.
3. Import ready-to-use custom tools in the **Custom Agent Tools Matrix** (`options.html`).
4. Paste template prompts into the **Prompt Panel** or run them directly in the extension popup!

---

## 2. Starter Kits & Prompt Library

### 💡 Example Prompts

#### Executive Web Summarizer
```text
You are an executive research assistant. Analyze the active tab and respond with:
1. A 2-sentence executive summary.
2. Bullet points highlighting 3 key takeaways or metrics.
3. A "Critical Takeaway" section pointing out any missing context or assumptions.
```

#### Financial Statement & Earnings Extractor
```text
You are a senior financial analyst. Analyze the provided page text or document and extract financial metrics into a clean JSON structure.
Include:
1. Company Name & Ticker Symbol
2. Reporting Period (e.g., Q3 2025, FY 2025)
3. Revenue, Net Income, Gross Margin, and EPS (Actual vs. Estimated)
4. Management Guidance & Key Growth Drivers
5. Notable Risks or Headwinds mentioned
Return ONLY valid JSON.
```
#### Stock Valuation & Fundamental Matrix
```text
Extract key fundamental ratios and valuation metrics from the page context.
Organize output into the following categories:
- Valuation: P/E Ratio, Forward P/E, P/S Ratio, P/B Ratio, EV/EBITDA
- Profitability: Return on Equity (ROE), Return on Assets (ROA), Operating Margin
- Balance Sheet: Total Debt, Cash & Short-Term Investments, Debt-to-Equity Ratio
- Dividend: Dividend Yield, Payout Ratio, Ex-Dividend Date
Format the result as a markdown table followed by a 2-sentence summary of overall financial health.
```
