# Refining Product Data and Pricing for an Enhanced Customer Experience in Online Fashion Retail
# Project Background

AJIO, part of Reliance Retail, is one of India’s largest online fashion retailers, offering a massive range of products for men, women, and kids. Despite its popularity, the platform has faced challenges such as inconsistent product data (e.g., brand and color), unpredictable pricing and discounting, and an imbalance in product offerings between genders.
This project, conducted as part of the IITM BS program capstone, leverages a Kaggle dataset with over 367,000 AJIO product listings to identify business-impacting patterns and provide actionable recommendations to enhance customer experience and drive growth.

# Key Insights and Recommendations are provided on four focus areas:

  Data Quality

  Pricing and Discounts

  Gender Balance in Catalog

  Revenue and Brand Performance

# Supporting Resources:

  SQL scripts for data cleaning

  SQL queries on business questions

  Interactive Tableau dashboard

# Data Structure & Initial Checks

# The primary dataset consists of 367,172 products and includes the following attributes:

  Brand: Standardized to 1,972 unique entries post-cleaning

  Color: Reduced from over 4,000 inconsistent variations to 33 standard color names

  Description: Short product summaries

  Gender Category: Mostly 'Men' or 'Women'

  Original_Price / Discount_Price: Numerical, ranging from ₹99–₹230,800

  Discount_Percent: 0%–93.99% after cleaning

Entity-Relationship Diagram:
(Insert ERD illustration here if available)
Executive Summary

# Overview of Findings
AJIO’s vast catalog is primarily budget and mid-range fashion, with women’s products comprising 58% of offerings and driving the majority of revenue. While discounting is common (average ~41%, median nearly 50%), luxury items (6% of catalog) receive unusually large and variable discounts, clouding brand value. Standardizing product data and addressing gender assortment imbalances present clear opportunities for customer experience and sales growth.

(Insert a dashboard snapshot or high-level visualization here)
Insights Deep Dive
# 1. Data Quality

  Main Insight 1: Cleaning reduced color categories from 4,000+ to 33 and fixed thousands of brand typos (e.g., “allensolly” → “allen-solly”), improving catalog trust and search relevance.

  Main Insight 2: Standardized attributes drastically improved analytics reliability and user experience.

  Main Insight 3: The top five colors—blue, black, white, gray, and green—make up almost half the entire product base, indicating strong and clear customer preferences.

(Visualization: Bar chart of top colors and brands after cleaning)
# 2. Pricing and Discounts

  Main Insight 1: Budget and mid-range items (~94% of the catalog) are heavily discounted; median discount is 50%.

  Main Insight 2: Luxury goods (above ₹10,000) receive inconsistent and sometimes excessive discounts, risking brand dilution.

  Main Insight 3: Strong price/discount correlation found (Pearson r = 0.81), indicating rational markdowns for most segments but outlier handling issues in luxury.

(Visualization: Boxplots of discount % by price band; scatterplot original vs. discount price)
# 3. Gender Balance in Catalog

  Main Insight 1: Women’s options represent 57.6% of catalog listings and 56% of sales; men’s premium/luxury is significantly underrepresented.

  Main Insight 2: Women have more choices across all price bands, especially in mid and premium.

  Main Insight 3: Men’s catalog features higher outliers in price, but fewer items overall, highlighting a gap for targeted expansion.

(Visualization: Heatmap of gender vs price band; boxplot of discounted price by gender)
# 4. Revenue and Brand Performance

  Main Insight 1: Women’s fashion not only leads in volume but in revenue contribution (₹1.32M vs. ₹0.96M for men).

  Main Insight 2: A handful of brands—Jolie-Robe, Max, Puma—dominate sales, suggesting strategic focus areas for partnerships and stocking.

  Main Insight 3: Consistently performing colors and brands are key levers for inventory and marketing optimizations.

(Visualization: Treemap of top brands, revenue by segment)
Recommendations

# Based on the findings, the following actionable recommendations are made for stakeholders:

  Automate Data Standardization: Regular audits and cleaning of product data to maintain accuracy and improve search/discoverability.

  Rebalance Product Assortment: Expand men’s premium/luxury offering to tap into underserved segments and boost sales.

  Refine Discount Strategy for Luxury: Institute clear guidelines to balance inventory movement with luxury branding and minimize deep, random discounts in high-value ranges.

  Prioritize Top Colors/Brands: Ensure top performing brands and colors remain well-stocked and central in campaigns.

  Dynamic, Data-Driven Discounting: Use analysis to calibrate discounts across price bands for optimal profitability and satisfaction.


# Assumptions and Caveats

  All data is sourced from a public Kaggle dataset, representing the state of the AJIO catalog at the time of scraping.

  Product URLs and images were excluded for this analysis; only core attributes were used.

  Outliers were identified and managed using IQR for both price features; this may exclude some genuine luxury/unusual items from the majority analysis.

  Certain business insights rely on segmentation thresholds (e.g., luxury defined as above ₹10,000) that are agreed with business norms, but these can be tuned as needed.

  Gender categories are based on available product tags and may not fully reflect inclusive segmentations.
