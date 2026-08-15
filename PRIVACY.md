# Privacy Policy for Custom Multimodal AI Assistant

**Effective Date:** August 15, 2026  
**Last Updated:** August 15, 2026  

Custom Multimodal AI Assistant ("AI Workspace Context Capture") is committed to protecting your privacy. This Privacy Policy explains what data this browser extension processes, how that data is stored, and the third-party services involved in providing its functionality.

---

## 1. Data Collection and Usage

This extension is built on a local-first architecture. We do not own, operate, or maintain central servers, tracking databases, or analytics services. All processing and configuration storage occur directly within your local browser environment.

### A. Information Provided by You
* **Provider API Keys:** When you configure your OpenRouter API Key (`orKey`) or Google Gemini API Key (`geminiKey`), these keys are saved strictly in your browser's encrypted local storage (`chrome.storage.local`). They are transmitted only to the respective model provider API endpoints when you execute an AI task.
* **License Keys:** If you activate a paid plan pass, your Payhip license key is stored locally and transmitted to Payhip's verification endpoint (`payhip.com/api/v2/license/verify`) to validate license status.
* **Custom Prompts & JavaScript Tools:** Prompt templates and custom JavaScript tool snippets created in the Settings matrix are stored locally in `chrome.storage.local`.

### B. Context & Web Content Data
* **Page Text & Screenshots:** Depending on your trigger actions, the extension extracts page text content, selected text, RSS feed data, or captures window screenshots (`activeTab`, `scripting`). This extracted context is compiled locally and sent to your chosen AI model provider (Google Gemini or OpenRouter) to fulfill your request.
* **Execution Logs:** Diagnostic logs, task histories (`taskLogs`), and site output histories (`siteLogs`) are stored exclusively on your device in local storage.

---

## 2. Third-Party Data Transmission

This extension connects exclusively to third-party endpoints specified by your configuration or required for basic service operations:

1. **Google Gemini API (`generativelanguage.googleapis.com`):** Page context, prompt instructions, and base64 screenshots are sent to Google Gemini only when you select a Gemini model. Data processing is governed by Google's Privacy Policy and API Service Terms.
2. **OpenRouter API (`openrouter.ai`):** Page context and prompt instructions are sent to OpenRouter only when you select an OpenRouter model. Data processing is governed by OpenRouter's Privacy Policy.
3. **Payhip API (`payhip.com`):** Your license key is transmitted over HTTPS to Payhip solely for validating subscription tiers. No browsing context, page content, or API keys are ever sent to Payhip.

*We do not share, sell, rent, or trade your data, webpage content, API keys, or personal information with any fourth parties, data brokers, or advertising networks.*

---

## 3. Data Retention and Storage

* **Local Retention:** All settings, API keys, custom prompts, custom JS snippets, and execution history remain in your browser's local storage until manually cleared or until the extension is uninstalled.
* **Automated Log Cleanup:** Execution logs are retained locally and automatically garbage-collected based on your retention settings (default 5 days).
* **No Remote Server Storage:** We maintain zero external server infrastructure; thus, none of your page context data or stored settings are accessible to the developer.

---

## 4. Compliance with Google Chrome Web Store User Data Policy

Custom Multimodal AI Assistant strictly complies with the Chrome Web Store Developer Program Policies:
* **Single Purpose:** The extension requests permissions (`activeTab`, `storage`, `scripting`, `alarms`, `notifications`, `tabs`, `<all_urls>`) solely to extract web context and execute user-driven AI workflows.
* **No Selling of User Data:** We do not sell user data to third parties under any circumstances.
* **No Remote Code Execution:** All extension logic is packaged natively in accordance with Manifest V3 standards. User-defined custom JS tools run inside the sandboxed active tab context.
* **No Data Usage for Credit/Lending:** We do not process user data for determining creditworthiness, lending, or financial scoring.

---

## 5. User Control and Data Erasure

You maintain complete control over your data:
* **Clear Logs:** You can clear execution logs anytime via the Diagnostic Logger or Settings tab.
* **Remove Credentials:** Deactivating your license or clearing input fields removes stored keys from `chrome.storage.local`.
* **Complete Erasure:** Uninstalling the extension completely purges all associated local data and settings from your browser storage.

---

## 6. Contact Information

If you have any privacy questions or feedback regarding this policy, please submit an issue via our official Support Form:  
[Official Support & Feedback Form](https://docs.google.com/forms/d/e/1FAIpQLSc0RwJQC_aHFH8mdKqMqe0kazHJgXTwyBCSRBzTeJ6E-KXMrw/viewform?usp=dialog)
