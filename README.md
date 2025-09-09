# Refining Product Data and Pricing for an Enhanced Customer Experience in Online Fashion Retail
# Purpose

The objective of this project is to help AJIO, one of India’s largest online fashion retailers (part of Reliance Retail), address critical challenges in product data quality, pricing transparency, and catalog balance. Clean, structured, and actionable data supports better business decisions, targeted growth, and a smoother customer experience.
# What This Project Covers

  - ### Business Problem:
    AJIO’s catalog suffers from messy product data (inconsistent brand and color names), unpredictable discounts, and a skewed product mix between men’s and women’s sections. These pain points can lead to poor search quality, erode customer trust, and block sales growth.

  - ### Project Goal:
    To clean and analyze a real-world AJIO product dataset (~367,000 listings from Kaggle), identify meaningful pricing and assortment patterns, and deliver recommendations that can drive more reliable search, fairer pricing, and stronger growth.

# Data & Methods

## Dataset:

  - Publicly available from Kaggle (“Ajio Fashion Clothing”), comprising 367,172 products after cleaning.

  - Key columns: Brand, Product Description, Gender Category, Discount Price, Original Price, Color.

## Tools and Techniques:

  - Python (Pandas, FuzzyWuzzy) for data wrangling and cleaning.

  - ANOVA, t-tests, and correlation analysis for identifying pricing and discount trends.

  - Visualizations with Matplotlib and Seaborn to surface business critical patterns.

# Data Cleaning & Transformation

  - **Brands:**
    Cleaned and standardized to 1,972 unique entries (e.g., “allensolly” corrected to “allen-solly”).

  - **Colors:**
    Reduced >4,000 messy names and typos to just 33 standard colors.

  - **Discounts:**
    Removed negative or implausible discounts.

  - **Outliers:**
    Managed using the IQR method; this keeps the core analysis focused and trustworthy.

# Final Clean Dataset Summary:

text
Total Products: 367,172
Brand Names: 1,972 (post-cleaning)
Color Categories: 33 (down from 4,296)
Discount Price Range: ₹81 to ₹230,800
Discount Percent Range: 0.0% to 93.99%
Gender Distribution: 211,534 Women’s (57.6%), 155,638 Men’s (42.4%)

# Analysis & Key Insights
  - ### Pricing & Discounts

  - Average Discount Percent: 41.2%, Median Discount: 49.96%.

  - Budget to mid-range dominates: Most products fall under ₹5,000, and discounts are heaviest in these bands.

  - ### Luxury Segment:
    Accounts for 6.4% of the catalog. These products show high variance in discounts, some deeply discounted, some hardly at all, which can erode luxury brand value.

  - ### Strong Correlation:
    Original price and discount price are closely linked (Pearson r = 0.81).

## Gender & Assortment

  - ### Women’s products:
    57.6% of the catalog, 56% of the total estimated revenue.

  - ### Men’s products:
    Fewer offerings, especially in premium and luxury, though there are proportionally more high-ticket outliers.

  - ### Clear opportunity:
    Expanding men’s premium and luxury choices can drive new growth.

## Brands & Revenue

  - Top 15 brands (Jolie-Robe, Max, Puma, etc.) capture a disproportionately high share of listings and revenue.

  - Predominant colors (blue, black, white, gray, green) make up nearly half of all products, indicating reliable shopper preferences.

# Visual Highlights

(Add visuals here, such as bar charts of top colors, boxplots for discount distribution, heatmaps for gender price bands, and treemaps of brand share. Placeholders are provided for your visuals.)
1. **Top 15 Colors (Bar Chart):** 

   - Visualizes the 15 most common, cleaned color categories (after wrangling thousands of typos).
   - Clearly shows customer color preferences and catalog concentration.

<img width="639" height="515" alt="image" src="https://github.com/user-attachments/assets/e2dd84ba-c557-4336-9531-188902321276" />

2. **Discount Percentage by Price Band (Boxplot):**
   
    - Displays the distribution of discount percentages across different price segments (Budget, Mid-range, Premium, High-End, Luxury).
    - Clearly illustrates how discount strategies vary with product pricing and highlights where the most substantial discounts or inconsistencies occur.

<img width="825" height="435" alt="image" src="https://github.com/user-attachments/assets/a7896f94-d671-46fa-b9fd-dddc6c9a629e" />

   

# What This Means & Recommendations

  - ### Continuous Data Hygiene:
    Regular cleaning and validation are essential for scalable search, recommendations, and analytics.

  - ### Strategic Discounting:
    Institute standard rules for luxury discounts to avoid erratic deep cuts that degrade brand value.

  - ### Balanced Expansion:
    Prioritize men’s assortment growth in premium and luxury, while maintaining strong offerings for women.

  - ### Inventory and Marketing:
    Focus on best-selling colors and top brands for stocking and promotion.

  - ### Data-Driven Decision-Making:
    Monitor patterns and realign discounting by price band to optimize profits and customer satisfaction.

# Impact

## By addressing data quality and using analysis-driven recommendations, AJIO can:

  - Boost customer trust and shopping efficiency.

  - Improve conversion and sales with smarter discount and assortment strategies.

  - Strengthen its competitive position as India’s digital fashion leader.

# About

This project was completed as part of the BS Data Science & Applications Capstone at IIT Madras.
