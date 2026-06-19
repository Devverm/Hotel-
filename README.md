# 🏨 Hotel Reservation Analysis Dashboard — Platinum Oasis

A Power BI dashboard built to analyze reservation data for **Platinum Oasis**, a premium hotel chain catering to business travelers, vacationers, and corporate groups. The dashboard uncovers booking trends, cancellation drivers, operational preferences, and guest retention opportunities.

---

## 📋 Project Overview

Platinum Oasis faced four key business challenges: a high cancellation rate, unclear guest preferences, operational inefficiencies, and low repeat-guest retention. This project addresses all four by transforming raw reservation data into actionable intelligence through an interactive, three-page Power BI dashboard.

**Objectives:**
1. Identify booking trends and seasonal demand patterns
2. Analyze cancellation drivers and recommend mitigation strategies
3. Optimize operations around room types, meal plans, and parking
4. Enhance guest retention by understanding new vs. returning guest behavior

---

## 📁 Project Structure

```
hotel-reservation-analysis-dashboard/
├── Hotel.csv                         # Source dataset (36,275 reservation records)
├── Hotel_Reservation_Analysis.pdf    # Presentation walkthrough of insights
├── dashboard/
│   ├── 01_overview_page.jpg          # Dashboard screenshot — Overview
│   ├── 02_cancellations_page.jpg     # Dashboard screenshot — Cancellations
│   └── 03_operations_page.jpg        # Dashboard screenshot — Operational Insights
└── README.md
```

---

## 📊 Dataset Details

**Source:** [Kaggle — Hotel Booking Dataset](https://www.kaggle.com/datasets/ahmedwaelnasef/hotel-booking/data)

The dataset contains **36,275 reservations** across **19 columns** covering the period 2017–2018.

| Column | Description |
|---|---|
| `ID` | Unique reservation identifier |
| `n_adults` | Number of adults in the booking |
| `n_children` | Number of children in the booking |
| `weekend_nights` | Number of weekend nights booked |
| `week_nights` | Number of weekday nights booked |
| `meal_plan` | Meal plan selected (Meal Plan 1/2/3 or Not Selected) |
| `car_parking_space` | Whether parking was requested (1 = Yes, 0 = No) |
| `room_type` | Type of room reserved (Room_Type 1–7) |
| `lead_time` | Days between booking date and arrival date |
| `year` | Year of arrival |
| `month` | Month of arrival |
| `date` | Day of arrival |
| `market_segment` | Booking channel: Online, Offline, Corporate, etc. |
| `repeated_guest` | Whether guest is returning (1) or new (0) |
| `previous_cancellations` | Number of prior cancellations by the guest |
| `previous_bookings_not_canceled` | Number of prior completed stays |
| `avg_room_price` | Average nightly room rate |
| `special_requests` | Number of special requests made |
| `status` | Booking outcome: `Canceled` or `Not_Canceled` |

---

## 📈 Dashboard Pages

### Page 1 — Overview
Key metrics, monthly booking trends, market segment breakdown, lead time distribution, and customer demographics (adults vs. children).

### Page 2 — Cancellations
Cancellation rate, monthly cancellation trends, distribution of cancellation status, impact of special requests on cancellations, and lead time vs. cancellation rate scatter analysis.

### Page 3 — Operational Insights
Guest preferences for room types, meal plan adoption rates, parking space utilization, and booking channel performance.

---

## 🔑 Key Metrics

| Metric | Value |
|---|---|
| Total Bookings | 36,275 |
| Cancellation Rate | 33% (11,885 bookings) |
| Average Lead Time | 85 days |
| Repeat Guest Rate | 2.56% (930 guests) |
| Parking Utilization | 3.1% of bookings |
| Online Bookings Share | 64% (23,214 bookings) |

---

## 💡 Key Insights

**Booking Trends**
- Peak booking period runs from **July to October**, with rising volumes and higher average room prices during this window.
- The majority of guests (94.6%) are adults, with children making up only 5.4% of travelers.

**Cancellations**
- Cancellation rate stands at **33%**, concentrated among bookings with **lead times exceeding 30 days**.
- Guests who make **zero special requests** cancel more frequently than those who make one or more.
- Seasonality plays a role — certain months see noticeably elevated cancellation activity.

**Guest Preferences**
- **Room Type 1** is the most popular choice for both new and returning guests (28,130 out of 36,275 bookings).
- **Meal Plan 1** dominates at 76% of all bookings (27,835 reservations).
- Only **3.1%** of guests request parking, signaling underutilization of parking facilities.

**Retention**
- Only **2.56%** of guests are repeat visitors, representing a significant opportunity for loyalty program investment.

---

## ✅ Recommendations

| Area | Actions |
|---|---|
| **Reduce Cancellations** | Introduce flexible cancellation policies; proactively engage long-lead-time bookers; encourage special requests at booking |
| **Optimize Operations** | Prioritize Room Type 1 inventory; streamline Meal Plan 1 supply chain; repurpose underused parking space |
| **Enhance Retention** | Launch a loyalty rewards program; offer personalized promotions to returning guests |
| **Leverage Seasonality** | Apply dynamic pricing during July–October peak; run off-season promotions to smooth demand |

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Power BI Desktop** | Dashboard creation, data modelling, and interactivity |
| **DAX** | Custom KPI measures and calculated columns |
| **Power Query** | Data cleaning and transformation |
| **CSV (Kaggle)** | Source data format |

---

## 🚀 Getting Started

1. Clone or download this repository.
2. Open **Power BI Desktop**.
3. Load `Hotel.csv` as the data source via **Get Data → Text/CSV**.
4. Apply the following data type assignments in Power Query:
   - `lead_time`, `n_adults`, `n_children` → Whole Number
   - `avg_room_price` → Decimal Number
   - `year`, `month`, `date` → Whole Number (or combine into a Date column)
   - `repeated_guest`, `car_parking_space` → Whole Number (binary flags)
5. Open the `.pbix` report file and refresh the data source path if needed.
6. Use the slicers (Year/Month, Market Segment, Lead Time) to explore the data interactively.

---

## 🔗 Project Resources

- **Presentation (PDF):** [Hotel Reservation Analysis.pdf](./Hotel_Reservation_Analysis.pdf) — Full slide walkthrough of the analysis and insights
- **Kaggle Notebook:** [View on Kaggle](https://www.kaggle.com/code/xiaotingb/hotel-reservation-analysis-power-bi)
- **GitHub Repository:** [View on GitHub](https://github.com/angelaboo/hotel-reservation-analysis-dashboard)

---

## 👤 Author

**Angela Boo**
- **GitHub:** [github.com/angelaboo](https://github.com/angelaboo)
- **Kaggle:** [kaggle.com/xiaotingb](https://www.kaggle.com/xiaotingb)
- **LinkedIn:** [Connect with Me](https://www.linkedin.com/in/xxtt)

---

*#PowerBI #DataAnalytics #HospitalityAnalytics #BusinessIntelligence #DataVisualization*
