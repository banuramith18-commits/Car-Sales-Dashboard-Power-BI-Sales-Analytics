# 🚗 Car Sales Dashboard — Power BI Sales Analytics

> An interactive two-page **Power BI Dashboard** analyzing car sales performance across dealers, regions, body styles, colors, and companies in the US market. Features **YTD vs MTD KPIs**, weekly trend lines, geographic sales maps, and a drillable transaction-level detail view.

---

## 🖼️ Dashboard Preview

### 📊 Overview Page
![Car Sales Overview](DashBoard.pdf)

### 📋 Details Page
> Transaction-level drill-down with per-car sales records across all dealers and models.

> 💡 *Replace PDF references above with `.png` screenshots for inline GitHub rendering.*

---

## 📌 Overview

This dashboard provides a comprehensive view of car sales performance across the United States, enabling sales managers and analysts to:

- 📈 Track **Year-to-Date (YTD)** and **Month-to-Date (MTD)** performance vs. prior year
- 🗺️ Visualize **geographic sales distribution** by dealer region
- 🏷️ Analyze sales by **body style**, **color**, and **company**
- 🔍 Drill down into **individual transaction records** on the Details page

---

## 🎯 Key KPIs (Overview Page)

| KPI | YTD Value | MTD Value | YoY Change |
|-----|-----------|-----------|------------|
| 💰 Total Sales | **$33.6M** | $28.52M | 🟢 +20.9% |
| 💵 Avg Price per Car | **$28.1K** | $28.38K | 🔴 -1.2% ($0.4K) |
| 🚘 Cars Sold | **6,918** | $1.01K | 🟢 +18.29% (1.27K) |

---

## 🎯 Key KPIs (Details Page)

| KPI | YTD Value | MTD Value | YoY Change |
|-----|-----------|-----------|------------|
| 💰 Total Sales | **$37.3M** | $25.76M | 🟢 +26.7% |
| 💵 Avg Price per Car | **$27.9K** | $28.12K | 🔴 -0.3% ($0.1K) |
| 🚘 Cars Sold | **6,343** | $0.92K | 🟢 +21.30% (1.35K) |

---

## 📈 Visualizations

### Overview Page

| Visual | Description |
|--------|-------------|
| 📉 Area Chart | YTD Sales Weekly Trend — peaks & troughs across 50 weeks |
| 🍩 Donut Chart | YTD Total Sales by Body Style — SUV, Hatchback, Sedan, Passenger, Hardtop |
| 🍩 Donut Chart | YTD Total Sales by Color — Pale White, Black, Red |
| 🗺️ Bubble Map | YTD Cars Sold by Dealer Region — US cities (Austin, Scottsdale, Greenville, etc.) |
| 📊 Table | Company Wise Sales — YTD Avg Price, Cars Sold, Total Sales, % GT YTD Sales |

### Details Page

| Visual | Description |
|--------|-------------|
| 📋 Data Table | Full transaction log — Car ID, Date, Customer, Dealer, Company, Color, Model, Total Sales |

---

## 🗂️ Repository Structure

```
Car-Sales-Dashboard/
│
├── Car Sales.xlsx         # Raw sales dataset
├── DashBoard.pbix         # Power BI workbook (interactive)
├── DashBoard.pdf          # Exported static dashboard
└── README.md              # Project documentation
```

---

## 🧰 Tools & Technologies

| Tool | Purpose |
|------|---------|
| [Microsoft Power BI](https://powerbi.microsoft.com/) | Dashboard design & visualization |
| Microsoft Excel (`.xlsx`) | Raw data source |
| DAX | YTD/MTD calculations, YoY variance measures |
| Power Query | Data transformation & modeling |
| Bing Maps | Geographic dealer region visualization |

---

## 📦 Dataset

The dataset (`Car Sales.xlsx`) contains individual car sales transaction records with the following key fields:

| Column | Description |
|--------|-------------|
| `Car_id` | Unique car sale ID (e.g. `C_CND_010646`) |
| `Date` | Transaction date (e.g. 02 January 2023) |
| `Customer Name` | Buyer's name |
| `Dealer_Name` | Dealership name (e.g. Diehl Motor CO Inc) |
| `Company` | Car manufacturer — Ford, Audi, BMW, Chevrolet, Dodge, etc. |
| `Color` | Car color — Black, Red, Pale White |
| `Model` | Car model — Focus, 3000GT, Lumina, Boxter, Corvette, etc. |
| `Body Style` | SUV, Hatchback, Sedan, Passenger, Hardtop |
| `Transmission` | Transmission type (filterable) |
| `Engine` | Engine type (filterable) |
| `Total Sales` | Revenue from individual sale (in $K) |

### 🔢 Sample Transaction Records

| Car ID | Date | Customer | Dealer | Company | Color | Model | Sales |
|--------|------|----------|--------|---------|-------|-------|-------|
| C_CND_010646 | 02 Jan 2023 | Owen | Diehl Motor CO Inc | Ford | Black | Focus | $49K |
| C_CND_010647 | 02 Jan 2023 | Patrick | Enterprise Rent A Car | Mitsubishi | Red | 3000GT | $20K |
| C_CND_010649 | 02 Jan 2023 | Wyatt | Star Enterprises Inc | Chevrolet | Red | Lumina | $12K |
| C_CND_010654 | 02 Jan 2023 | George | Iceberg Rentals | Porsche | Red | Boxter | $24K |
| C_CND_010661 | 03 Jan 2023 | Rohan | Nebo Chevrolet | Cadillac | Black | Eldorado | $37K |

---

## 🏢 Company-wise Performance Snapshot

| Company | YTD Avg Price | Cars Sold | YTD Total Sales | % of Total |
|---------|--------------|-----------|----------------|------------|
| Acura | $28.5K | 163 | $4.6M | 2.39% |
| Audi | $26.2K | 86 | $2.3M | 1.16% |
| BMW | $25.5K | 248 | $6.3M | 3.25% |
| Buick | $32.9K | 152 | $5.0M | 2.58% |
| Cadillac | $44.8K | 206 | $9.2M | 4.75% |
| Chevrolet | $25.4K | 449 | $11.4M | 5.87% |
| Chrysler | $25.0K | 474 | $11.9M | 6.11% |
| **Dodge** | $29.1K | **603** | **$17.6M** | **9.03%** |
| Ford | $31.6K | 415 | $13.1M | 6.75% |
| Honda | $22.0K | 192 | $4.2M | 2.18% |

> 🏆 **Dodge leads in both cars sold (603) and total sales share (9.03%)**

---

## 🔽 Interactive Filters (Both Pages)

| Filter | Options |
|--------|---------|
| Body Style | All, SUV, Hatchback, Sedan, Passenger, Hardtop |
| Dealer_Name | All / specific dealer |
| Transmission | Multiple select |
| Engine | All / specific engine type |

---

## 💡 Key Insights

- 🏆 **Dodge dominates** with 603 cars sold and 9.03% of total YTD sales
- 📈 **Total sales grew 20.9% YoY** — strong market recovery signal
- 💵 **Average price dipped 1.2%** — competitive pricing pressure across brands
- 🚘 **Cars sold up 18.29% YoY** — volume growth outpacing price growth
- 🗺️ **Scottsdale, Austin, and Greenville** are the strongest dealer regions on the map
- 🎨 **Pale White is the most popular color**, followed by Black and Red
- 🚙 **SUVs lead in body style sales**, consistent with US market preferences

---

## 🔧 Future Improvements

- [ ] Add a **Year / Month slicer** for time-based filtering
- [ ] Build a **Profit Margin** page (if cost data is available)
- [ ] Add **forecasting** using Power BI's built-in analytics
- [ ] Publish to **Power BI Service** for live sharing and scheduled refresh
- [ ] Add **model-level drill-through** from the company table to individual models

---

## 🚀 How to Use

1. **View Static Export** — Open `DashBoard.pdf` in your browser or PDF viewer
2. **Explore Interactively** — Open `DashBoard.pbix` in [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
3. **Access Raw Data** — Open `Car Sales.xlsx` in Excel or load into Power BI / Python for further analysis

---

## 🙋 Author

**Mindbender66**
- 🐙 GitHub: [@Mindbender66](https://github.com/Mindbender66)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
