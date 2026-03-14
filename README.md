I'll gather comprehensive information about your repository to provide a detailed project review and EDA analysis.Now let me get the notebook to see the detailed analysis:Now I have comprehensive information about the repository. Let me compile a detailed project review and EDA analysis:

---

# **Restaurant Cuisine Analysis - Project Review & EDA**

## 📋 **PROJECT OVERVIEW**

**Repository:** `Bharanidharan0077/Restaurant-Cuisine-Analysis-`  
**Language:** Jupyter Notebook  
**Status:** Active (Last updated: March 14, 2026)  
**Repository Size:** ~6.07 MB  
**Dataset Size:** 9,551 restaurant records across 141 cities

---

## 📊 **DATASET SUMMARY**

### **Data Dimensions:**
- **Rows:** 9,551 restaurants
- **Columns:** 21 features
- **Missing Values:** 9 missing values in the "Cuisines" column (9,542 non-null)
- **Duplicates:** 0 duplicate records

### **Feature Breakdown:**

| Category | Features |
|----------|----------|
| **Identifiers** | Restaurant ID, Restaurant Name |
| **Location** | Country Code, City, Address, Locality, Locality Verbose, Longitude, Latitude |
| **Cuisine Info** | Cuisines (1,825 unique combinations) |
| **Pricing** | Average Cost for two, Currency (12 unique currencies), Price range (1-4) |
| **Services** | Has Table booking, Has Online delivery, Is delivering now, Switch to order menu |
| **Ratings** | Aggregate rating (0-4.9), Rating color, Rating text, Votes (0-10,934) |

---

## 🔍 **KEY EXPLORATORY DATA ANALYSIS (EDA) FINDINGS**

### **1. TOP CUISINES ANALYSIS** 

#### Most Popular Cuisines:
```
North Indian:    3,960 restaurants (41.46%)
Chinese:         2,735 restaurants (28.64%)
Fast Food:       1,986 restaurants (20.79%)
```

**Insight:** North Indian cuisine dominates the dataset, accounting for over 2/5 of all restaurants. These three cuisines represent **90.89%** of all restaurant cuisines in the dataset.

---

### **2. GEOGRAPHIC DISTRIBUTION**

#### Top Cities:
- **New Delhi** leads with **5,473 restaurants** (57.3% of total dataset)
- This is a massive concentration in a single city
- 140 other cities represent remaining restaurants
- Geographic spread: 141 unique cities across multiple country codes

**Geographic Concentration:** The dataset is heavily skewed towards New Delhi, which may limit the generalizability of insights to other regions.

---

### **3. PRICING INSIGHTS**

#### Price Range Distribution:
- **Mean Price Range:** 1.80 (on scale of 1-4)
- **Median Price Range:** 2.0
- **Most Common:** Mid-range restaurants (Price range 2)
- **Range:** From budget (1) to premium (4)

**Insight:** The majority of restaurants fall into mid-range pricing categories, suggesting a strong market for moderately-priced establishments.

---

### **4. RATINGS & CUSTOMER ENGAGEMENT**

#### Aggregate Rating Statistics:
- **Mean Rating:** 2.67/5.0
- **Median Rating:** 3.2/5.0
- **Range:** 0 to 4.9
- **Votes Mean:** 156.91 votes per restaurant
- **Votes Median:** 31 votes (showing right-skewed distribution)

#### Rating Distribution:
- **Dark Green (Excellent):** 3,737 restaurants
- **Orange (Average):** 3,737 restaurants (matching excellent count interestingly)
- **Green (Very Good):** Significant portion
- **6 Rating Categories:** Distributed across color codes

---

### **5. SERVICE OFFERINGS ANALYSIS**

#### Table Booking:
- **No table booking:** 8,393 restaurants (87.9%)
- **With table booking:** Only 12% offer this service

#### Online Delivery:
- **No online delivery:** 7,100 restaurants (74.3%)
- **With online delivery:** 25.7% (Growing service)

#### Current Delivery Status:
- **Not delivering now:** 9,517 restaurants (99.6%)
- **Actively delivering:** < 1% (Minimal active operations)

#### Order Menu Switch:
- **Uniform:** All 9,551 restaurants show "No" (100%) - Feature appears non-informative

**Insight:** Online delivery is an emerging service with 1 in 4 restaurants offering it. Most restaurants don't have table booking systems.

---

### **6. RESTAURANT DISTRIBUTION**

#### Key Metrics:
- **Unique Restaurants:** 7,446 unique names
- **Repeated Names:** Some chains like "Cafe Coffee Day" appear 83 times
- **Most Common Location:** Connaught Place, New Delhi (122 occurrences)

---

## 🛠️ **TECHNICAL IMPLEMENTATION**

### **Tools & Libraries Used:**
- ✅ **Python** - Core programming language
- ✅ **Pandas** - Data manipulation and analysis
- ✅ **NumPy** - Numerical computations
- ✅ **Matplotlib** - Static visualizations
- ✅ **Seaborn** - Statistical data visualization
- ✅ **Jupyter Notebook** - Interactive analysis environment

### **Data Processing Steps:**
1. ✅ Data Loading & Inspection
2. ✅ Missing Value Detection (9 missing in Cuisines)
3. ✅ Duplicate Detection (0 duplicates found)
4. ✅ Data Type Validation
5. ✅ Column Name Standardization (lowercase, underscore formatting)
6. ✅ EDA with visualizations

---

## 📈 **KEY INSIGHTS & RECOMMENDATIONS**

### **1. Cuisine Strategy:**
- **Recommendation:** Focus on North Indian and Chinese cuisines for high demand
- **Opportunity:** Underrepresented cuisines could differentiate new restaurants
- **Finding:** Top 3 cuisines cover 90%+ of market

### **2. Location Strategy:**
- **Finding:** Extreme concentration in Delhi (57%)
- **Caution:** Limited geographic diversity; results may not generalize
- **Opportunity:** Analyze performance in non-Delhi cities

### **3. Pricing & Rating Correlation:**
- **Finding:** Mid-range restaurants (price=2) appear most common
- **Observation:** Average rating of 2.67 suggests competitive market
- **Trend:** Higher ratings concentrated in "Dark Green" category

### **4. Service Adoption:**
- **Online Delivery Opportunity:** 75% of restaurants don't offer online delivery - growing market
- **Table Booking Gap:** 88% lack table booking - modernization potential
- **Growth Area:** Digital services integration critical for competitiveness

### **5. Customer Engagement:**
- **High Variance:** Votes range 0-10,934 (significant disparity in visibility)
- **Median-Mean Gap:** Median 31 vs Mean 156.91 suggests outlier popular restaurants
- **Implication:** Marketing and reputation management critical for discoverability

---

## 📂 **REPOSITORY STRUCTURE**

```
Restaurant-Cuisine-Analysis/
├── Dataset .xls                          (Raw data - 2.24 MB)
├── Restaurant Cuisines analysis Level 1.ipynb  (Analysis notebook - 235 KB)
├── Task List.pdf                         (Project tasks)
└── README.md                             (Documentation)
```

## 📝 **CONCLUSION**

This is a **solid foundational data analysis project** with clean data and meaningful insights about restaurant preferences. The analysis correctly identifies North Indian cuisine dominance and mid-range pricing trends. However, the extreme concentration in Delhi (57%) limits geographic generalizability. The project would benefit from deeper statistical analysis, predictive modeling, and expanded visualizations to provide more actionable business intelligence.

**Overall Rating: 7/10** - Good start, requires deeper analysis for advanced insights.
