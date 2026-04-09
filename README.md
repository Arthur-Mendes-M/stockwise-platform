# StockWise Platform

Full-stack inventory and stock management platform built for small businesses.
I developed both the frontend (this repository) and the backend API, as a
university project. The system covers the complete commercial cycle — products,
sales, purchases, clients, virtual stock, and automated PDF reports.

**Live:** [stockwise-self.vercel.app](https://stockwise-self.vercel.app)

---

## Tech stack

![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![shadcn/ui](https://img.shields.io/badge/shadcn--ui-000000?style=flat-square)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Recharts](https://img.shields.io/badge/Recharts-22C55E?style=flat-square)
![jsPDF](https://img.shields.io/badge/jsPDF-FF0000?style=flat-square)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)

---

## Features

**Dashboard**
- Summary cards: total sales by day, month, year, and total products
- Out-of-stock and low-stock alerts
- 4 chart types: bar, pie, radar, and line — all from real transaction data

**Products**
- Full product catalog with CRUD
- Barcode scanner integration for quick lookup

**Sales & Purchases**
- Register and manage sales and purchase orders
- PDF generation per transaction (via pdfMake)
- Update and delete operations

**Clients**
- Client registration and management
- Linked to sales history

**Virtual Stock**
- Container-based stock organization (think shelves or storage boxes)
- QR code scanner for quick container lookup
- Products assigned to containers for physical location tracking

**Reports**
- Custom PDF reports with date range filter
- Pulls data from products, sales, purchases, clients, and containers
- Download directly from the interface

**StockWizard**
- AI-powered chat assistant embedded in the dashboard
- Answers questions about the company's stock and transactions
- Supports web search queries with `pesquise...` prefix
- Accessible via floating button or `Alt+W` keyboard shortcut

**Auth**
- Company-level login with JWT token
- Protected routes throughout the app

---

## Running locally

```bash
git clone https://github.com/Arthur-Mendes-M/stockwise-platform
cd stockwise-platform
npm install
cp .env.example .env
# set VITE_API_BASE_URL to your backend URL
npm run dev
```

---

*Built by [Arthur Martins](https://github.com/Arthur-Mendes-M)*
