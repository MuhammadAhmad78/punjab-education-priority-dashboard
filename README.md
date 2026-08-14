# Punjab District Education Priority Dashboard (2019–20)

A Power BI project that ranks all 36 districts of Punjab, Pakistan by education need — combining literacy rates, gender literacy gaps, and out-of-school rates into a single **Primary Education Priority Score**, so that limited education resources can be directed to the districts that need them most.

![Priority Level](https://img.shields.io/badge/Priority%20Levels-4-blue)
![Districts](https://img.shields.io/badge/Districts-36-green)
![Data Year](https://img.shields.io/badge/Data-2019--20-orange)
![Made with Power BI](https://img.shields.io/badge/Made%20with-Power%20BI-yellow)

---

## 📌 Overview

Pakistan's Punjab province has stark disparities in education access between districts. This project turns raw district-level literacy statistics into a ranked, color-coded priority list that education planners, NGOs, and policymakers can use to identify where intervention is most urgently needed.

Each of the 36 districts is scored on a **Primary Education Score (0–100)**, derived from:
- Overall literacy rate
- Female literacy rate
- Gender literacy gap
- Out-of-school children rate

Districts are then bucketed into four **Priority Levels**: `Critical`, `High`, `Medium`, `Lower`.

## 🎯 Key Insights

- **Average literacy rate across Punjab districts: ~62%**, with a wide range between the lowest and highest performing districts.
- **Rajanpur** has the lowest literacy rate in the province, while **Rawalpindi** has the highest — a gap of 40 percentage points between them.
- **4 districts (Rajanpur, Muzaffargarh, D.G. Khan, Rahim Yar Khan)** fall into the `Critical` priority band — mostly in South Punjab.
- The **average gender literacy gap is ~8.6 percentage points**, but reaches as high as **16 points** in some districts (e.g. Mianwali), pointing to significant disparities in girls' education access.
- **11 districts** are classified `High` priority and **12** as `Medium`, showing that the majority of Punjab still needs meaningful investment in primary education infrastructure.

## 📁 Repository Structure

```
├── data/
│   └── pakistan_district_education_priority_punjab_2019_20.csv   # Source dataset
├── powerbi/
│   └── Punjab_District_Education_Priority_Index.pbix              # Power BI project file
├── screenshots/
│   └── dashboard_preview.png                                     # Dashboard screenshots (add yours here)
├── docs/
│   └── DATA_DICTIONARY.md                                        # Column-by-column data description
├── README.md
├── LICENSE
└── .gitignore
```

## 📊 Dataset

**File:** `data/pakistan_district_education_priority_punjab_2019_20.csv`
**Rows:** 36 districts | **Province:** Punjab, Pakistan | **Reference period:** 2019–20

See [`docs/DATA_DICTIONARY.md`](docs/DATA_DICTIONARY.md) for a full description of every column.

## 🖥️ Power BI Dashboard

The Power BI project file is included at [`powerbi/Punjab_District_Education_Priority_Index.pbix`](powerbi/Punjab_District_Education_Priority_Index.pbix).

> Add a screenshot of the dashboard to `screenshots/` before pushing, so visitors can preview it without opening Power BI — see the setup guide below.

The dashboard includes:
- A ranked table/matrix of all districts by Primary Education Score
- A map visual showing priority levels geographically across Punjab
- KPI cards for province-wide averages (literacy, female literacy, gender gap, out-of-school rate)
- Slicers to filter by Priority Level

## 🛠️ How to Use

1. Clone this repository.
2. Open `powerbi/Punjab_District_Education_Priority_Index.pbix` in [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free).
3. If prompted, point the data source to `data/pakistan_district_education_priority_punjab_2019_20.csv`.
4. Explore the report, or use `Publish` to push it to your own Power BI Service workspace.

## 🧮 Methodology

The **Primary Education Score** is a weighted composite index built from four indicators (literacy rate, female literacy rate, gender literacy gap, and out-of-school rate), normalized so that districts with the greatest educational need score highest. Districts are then grouped into four tiers:

| Score Range | Priority Level |
|---|---|
| 65 – 100 | Critical |
| 45 – 64.9 | High |
| 30 – 44.9 | Medium |
| 0 – 29.9 | Lower |

## 📄 License

This project is licensed under the [MIT License](LICENSE) — feel free to use, adapt, and build on it.

## 🙋 Author

Built as a data analysis / Power BI portfolio project. Contributions and suggestions are welcome — feel free to open an issue or pull request.
