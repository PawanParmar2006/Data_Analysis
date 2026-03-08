# 📊 App Store Data Visualization Dashboard

This repository contains a collection of **advanced interactive data visualizations** built using **Python, Pandas, and Plotly**.
The project analyzes **mobile app store datasets** and generates multiple graphs with **strict filtering rules, multilingual category transformations, and time-restricted dashboard visibility**.

Each visualization simulates **real-world business dashboards** where charts appear only during specific time windows.

---

# 🚀 Project Overview

This project performs:

* 📈 Advanced **data visualization**
* 🧹 Complex **data filtering**
* 🌍 **Multilingual category translations**
* ⏱ **time-based dashboard rendering**
* 📊 Interactive **Plotly charts**
* 📁 Exporting graphs as **HTML dashboards**

---

# 🛠 Technologies Used

| Tool                | Purpose                        |
| ------------------- | ------------------------------ |
| **Python**          | Core programming               |
| **Pandas**          | Data cleaning & transformation |
| **Plotly**          | Interactive charts             |
| **Datetime & pytz** | Time-based graph visibility    |
| **HTML Export**     | Dashboard visualization        |

---

# 📊 Visualizations Included

## 1️⃣ Grouped Bar Chart – Ratings vs Reviews

Compares **Average Rating and Total Reviews** for the **Top 10 app categories by installs**.

### Filters Applied

* Rating ≥ **4.0**
* App size ≥ **10 MB**
* Last Updated month = **January**

### Time Visibility

🕒 **3 PM – 5 PM IST**

---

## 2️⃣ Choropleth Map – Global Installs by Category

Visualizes the **Top 5 categories by installs** while excluding specific categories.

### Filters Applied

* Categories starting with **A, C, G, S are excluded**
* Top 5 categories by installs
* Highlight categories with installs **> 1 million**

### Time Visibility

🕒 **6 PM – 8 PM IST**

---

## 3️⃣ Dual Axis Chart – Installs vs Revenue

Compares **Average Installs and Average Revenue** for **Free vs Paid apps**.

### Filters Applied

* Installs ≥ **10,000**
* Revenue ≥ **10,000**
* Android Version > **4.0**
* Size > **15 MB**
* Content Rating = **Everyone**
* App name length ≤ **30 characters**

### Time Visibility

🕒 **1 PM – 2 PM IST**

---

## 4️⃣ Time Series Chart – Install Growth Trend

Tracks **total installs over time by app category**.

### Special Features

* Highlights **>20% month-over-month install growth**
* Category translations:

  * **Beauty → सौंदर्य (Hindi)**
  * **Business → வணிகம் (Tamil)**
  * **Dating → Partnersuche (German)**

### Filters Applied

* Reviews > **500**
* App name **cannot start with X, Y, Z**
* App name **cannot contain letter S**

### Time Visibility

🕒 **6 PM – 9 PM IST**

---

## 5️⃣ Bubble Chart – App Size vs Rating

Analyzes the relationship between **App Size, Rating, and Installs**.

### Chart Logic

* **Bubble Size → Installs**
* **Game category highlighted in pink**

### Filters Applied

* Rating > **3.5**
* Reviews > **500**
* Sentiment Subjectivity > **0.5**
* Installs > **50,000**
* App name **cannot contain letter S**

### Translations

* Beauty → **सौंदर्य**
* Business → **வணிகம்**
* Dating → **Partnersuche**

### Time Visibility

🕒 **5 PM – 7 PM IST**

---

## 6️⃣ Stacked Area Chart – Cumulative Installs

Displays **cumulative installs over time by category**.

### Filters Applied

* Rating ≥ **4.2**
* Reviews > **1000**
* App size between **20 MB – 80 MB**
* App name **cannot contain numbers**
* Category must start with **T or P**

### Translations

* Travel & Local → **Voyage et Local (French)**
* Productivity → **Productividad (Spanish)**
* Photography → **写真 (Japanese)**

### Special Feature

Highlights months with **>25% install growth**.

### Time Visibility

🕒 **4 PM – 6 PM IST**

---

# ⏰ Dashboard Time Logic

Each graph appears only during its **assigned time window**.

| Graph              | Time        |
| ------------------ | ----------- |
| Dual Axis Chart    | 1 PM – 2 PM |
| Grouped Bar Chart  | 3 PM – 5 PM |
| Stacked Area Chart | 4 PM – 6 PM |
| Bubble Chart       | 5 PM – 7 PM |
| Choropleth Map     | 6 PM – 8 PM |
| Time Series Chart  | 6 PM – 9 PM |

Outside these windows, the graphs **will not render in the dashboard**.

---

# 📁 Project Structure

```
app-analytics-visualizations
│
├── data
│   └── apps_dataset.csv
│
├── graphs
│   ├── grouped_bar_chart.py
│   ├── choropleth_map.py
│   ├── dual_axis_chart.py
│   ├── time_series_chart.py
│   ├── bubble_chart.py
│   └── stacked_area_chart.py
│
├── outputs
│   └── *.html
│
└── README.md
```

---

# ⚙️ Installation

Clone the repository

```
git clone https://github.com/yourusername/app-analytics-visualizations.git
```

Install required libraries

```
pip install pandas plotly pytz
```

Run the scripts

```
python graph_script.py
```

Each graph will generate an **interactive HTML file**.

---

# 📁 Output

The generated files will look like:

```
Dual_Axis_Top3_Category_Comparison.html
Bubble_App_Size_vs_Rating.html
Stacked_Area_App_Installs.html
Global Installs Choropleth.html
TimeSeries_App_Installs_Growth.html
GroupedBar_Top10_Category_Rating_Reviews.html
```

Open them in any browser to view the interactive dashboards.

---

# 🎯 Learning Outcomes

This project demonstrates:

* Advanced **data preprocessing**
* Complex **filtering logic**
* Plotly **interactive dashboards**
* **Time-based visualization control**
* **Multilingual data transformation**
* Real-world **data analytics workflow**

---

# 👨‍💻 Author

**Pawan Rajput**

Aspiring **AI / ML Engineer & Data Analyst**

Passionate about **Machine Learning, Data Visualization, and Analytics**.

---

# ⭐ Support

If you find this project helpful, consider giving the repository a **⭐ Star on GitHub**.


