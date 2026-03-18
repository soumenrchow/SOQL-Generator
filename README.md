# ⚡ SOQL Studio — AI-Powered Salesforce Query Generator

A single-file web app that generates accurate **SOQL** and **SOSL** queries for any Salesforce application using AI (Claude by Anthropic).

![SOQL Studio](https://img.shields.io/badge/Salesforce-SOQL%20%2F%20SOSL-0176d3?style=for-the-badge&logo=salesforce&logoColor=white)
![HTML](https://img.shields.io/badge/Built%20With-HTML%20%2F%20CSS%20%2F%20JS-f0b429?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

---

## 🚀 Live Demo

> Hosted via GitHub Pages: `https://<your-username>.github.io/<repo-name>`

---

## ✨ Features

- **Multi-Cloud Support** — Sales Cloud, Service Cloud, Marketing Cloud, Experience Cloud, Health Cloud, Financial Services Cloud, and Custom Orgs
- **Query Types** — Standard SELECT, Aggregates, Subqueries / Semi-Joins, Parent-Child Relationships, SOSL FIND
- **Output Styles** — Plain SOQL, Apex inline String, `Database.query()`, LWC `@wire` adapter, Tooling API format
- **SOQL Syntax Highlighting** — Color-coded keywords, functions, date literals, strings
- **Smart Field Tags** — Shows every queried field at a glance
- **Dev Notes** — FLS considerations, governor limit advisories, and performance tips
- **Query History** — Last 8 queries saved and reloadable in one click
- **Copy & Download** — Copy to clipboard or download as `.soql` file
- **Keyboard Shortcut** — `⌘ Enter` / `Ctrl + Enter` to generate

---

## 🛠️ Tech Stack

| Layer      | Technology |
|------------|-----------|
| Frontend   | Vanilla HTML, CSS, JavaScript |
| Fonts      | IBM Plex Mono + Plus Jakarta Sans (Google Fonts) |
| AI Engine  | [Claude API](https://www.anthropic.com) (claude-sonnet-4) |
| Hosting    | GitHub Pages (single static file) |

---

## 📦 Setup

This is a **zero-dependency** single HTML file. No build step required.

### GitHub Pages (recommended)

1. Fork or clone this repo
2. Go to **Settings → Pages**
3. Set source to `main` branch, root `/`
4. Visit `https://<your-username>.github.io/<repo-name>`

### Local

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
open index.html   # or just double-click the file
```

---

## 💡 Example Prompts

```
Get all open Opportunities over $50,000 created this year, ordered by close date
```
```
Find all Cases assigned to queues that have been open for more than 7 days
```
```
Show monthly revenue grouped by product family for this fiscal year
```
```
List Contacts with no Activity in the last 90 days from active Accounts
```
```
Find duplicate Leads by email address
```

---

## 🔒 Notes

- The app calls the **Anthropic Claude API** directly from the browser. No data is stored server-side.
- For production use, consider proxying the API call through a backend to keep your API key secure.
- SOQL queries are generated based on standard Salesforce schema. Custom fields (`__c`) are represented as examples — verify against your actual org schema.

---

## 📄 License

MIT — free to use, modify, and distribute.

---

<p align="center">Built with ⚡ and the Anthropic Claude API</p>
