# 🗂️ **BLO Search & Verification Dashboard — Power BI Project**

<!-- ### 📘 *Created for Real-World Government Workflow Optimization* -->

![BLO DB Finder PowerBI](res/video.gif)

<!-- --- -->

## 📄 **Special Intensive Revision (SIR) — Core Context of This Project**

The **Special Intensive Revision (SIR) Form** is the central reason this project exists.  
It is an official enumeration document used by the **Election Commission of India (ECI)** during its **house-to-house verification drive** to update and clean the electoral rolls.

## 🔹 **What the SIR Form Is**

A verification form distributed by **Booth Level Officers (BLOs)** during home visits (and also online), enabling citizens to:

- Verify their voter information  
- Update incorrect details  
- Enroll if they are not yet registered  

## 🔹 **Purpose of the SIR Drive**

The SIR process aims to:

- Cleanse electoral databases  
- Remove *duplicate*, *deceased*, or *shifted* voters  
- Ensure every eligible citizen is properly included  

## 🔹 **Why It Is Important**

Accurate electoral rolls are the backbone of **free and fair elections**.  
The SIR exercise ensures correctness, completeness, and inclusivity.

## 🔹 **Where Citizens Access It**

Eligible citizens can typically complete verification through the **ECI Voters’ Service Portal**.

---

## 🔍 **Project Overview**

This project was developed to solve a **real and challenging problem faced by BLOs (Booth Level Officers)** in India.

A BLO is responsible for:

- Verifying citizen details
- Cross-checking electoral records
- Managing corrections and updates
- Handling lakhs of entries in massive CSV sheets

Traditionally, BLOs used tools like **Excel + Ctrl+F**, which becomes extremely slow and inefficient with **8–10 lakh+ records**.

To support my mother (a BLO) and officers like her, I built a **Power BI Dashboard** that:

- Loads large datasets instantly
- Allows **fast keyword-based search** across multiple fields
- Filters by *Name, Relative Name, Age, Gender, AC Number, Booth Number, EPIC No*, etc.
- Works offline for security (Govt data)

This dramatically improves speed, accuracy, and convenience.

---

## 🌱 **Problem Statement**

### ❌ *Old Method: Manual Search in Excel (Ctrl + F)*

- Slow and freezes with large files
- Hard to apply multiple filters
- Requires full dataset on each device
- Not mobile-friendly

### ⚠️ *Temporary Fix: Regex-Based Google Sheet*

My father created a solution using Google Sheets + Regex.

But:

- Google Sheets becomes slow beyond ~50k rows
- Users must upload the full dataset → ❌ security issue
- Slow on mobile networks
- Not scalable for other BLOs

### ✅ *Final Solution: Power BI Dashboard*

- Handles **8,27,963+ rows** smoothly (based on screenshot)
- Fast filtering with multiple fields
- Clean interface for BLO workflow
- Runs offline on personal laptop (no internet needed)

However, Power BI dashboards are **not accessible on mobile without a Premium license**.

So I built an additional **Python-based Dashboard** that works on any mobile or device.

👉 *GitHub Repo:* **[https://github.com/shloktilokani/BLO-Database-Finder](https://github.com/shloktilokani/BLO-DB-Finder.git)**

---

## ⚙️ **Project Workflow**

### **1️⃣ Data Source**

Data is loaded from a CSV file containing government electoral details.

Fields include:

- `serial_no`
- `name`
- `relation`
- `relative_name`
- `gender`
- `age`
- `epic_no`
- `ac_no`
- `booth_no`

Dataset Size: **8+ lakh rows**

---

### **2️⃣ Dashboard Design in Power BI**

The dashboard consists of:

#### 🔹 **Search Bars**

- Search by *Name*
- Search by *Relative Name*
- Search by *Surname/Second Name*

#### 🔹 **Main Table View**

Shows all voter details with features:

- Gujarati text support
- Scrollable large table
- Lightweight rendering

#### 🔹 **Count KPI**

Displays number of matched records
(e.g., **827,963** rows total, **118** rows filtered in screenshot)

#### 🔹 **Filters**

- Age filter
- Gender filter
- AC No
- Booth No
- Any keyword match

The design is minimal, clean, and optimized for BLO field needs.

---

## 🧪 **Example Use Case**

Searching for the name **"અમીત શાહ"** returns **118 matching records** instantly.

The results include:

- Surname variations
- Relative names
- Booth and AC details
- EPIC numbers

This helps BLOs complete verification **rapidly**.

---

## 💡 **Insights & Impact**

### ✔️ **Massively faster data search** compared to Excel

### ✔️ **Accurate filtering** even with Gujarati names

### ✔️ **Offline and secure** — ideal for government work

### ✔️ **Designed for non-technical users**

### ✔️ **Reusable tool for any BLO office**

Even officers without technical experience can filter lakhs of records easily.

---

## 🏁 **Conclusion**

This project demonstrates the power of **Power BI as a real-world operational tool**.

It transforms:

- Manual, slow verification → Automated, fast filtering
- Complex datasets → Simple and intuitive interface

To solve mobile accessibility issues, I created a complementary **Python dashboard**.

👉 **Python Version (Mobile Friendly):**  
[https://github.com/shloktilokani/BLO-Database-Finder](https://github.com/shloktilokani/BLO-DB-Finder.git)

---

## 🚀 **Future Enhancements**

- Convert dashboard into a Web App (Flask/React)
- Add voice-based search for BLOs in the field
- Integrate multilingual support (Gujarati, Hindi, English)
- Auto-detection of spelling mistakes using NLP

---

## 📦 **Project Files**

- `data.csv` — Source dataset
- `.pbix` file — Power BI dashboard
- Link to mobile-friendly Python version

---

## ⭐ **Thank You!**

If this dashboard was helpful, please ⭐ star the repo or share feedback!
