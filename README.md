# Ajio-fashion-customer-experience

# Project Overview

This project aims to enhance AJIO’s online fashion retail platform by refining product data and optimizing pricing strategies to deliver a smoother, fairer, and more enjoyable shopping experience. AJIO, a leading Indian online fashion retailer under Reliance Retail, houses an extensive product catalogue with over 367,000 items. Despite its success, challenges such as inconsistent product metadata, unpredictable pricing and discounts, and gender-based catalogue imbalances have impacted customer experience and sales growth.

Through comprehensive data cleaning, pricing analysis, and gender segmentation, this work seeks to improve search accuracy, optimize discount allocation, and address underdeveloped product segments—especially in men’s premium and luxury fashion.
Dataset & Scope

  Source: Kaggle’s “Ajio Fashion Clothing” dataset, scraped directly from AJIO’s official website.

  Size: 367,172 product listings with nine key attributes: product brand, color, description, gender category, original price, discount price, discount percentage,   among others.

  Data Quality Issues: Initially included thousands of inconsistent color labels and nearly 2,000 brand name variations, along with negative or impossible discount values.

# Key Challenges Addressed

  Data Quality: Inconsistent naming of colors and brands hindered accurate product discovery and customer trust.

  Pricing & Discounts: Unsystematic discounting patterns, particularly within the luxury segment, risk confusing customers and undermining brand equity.

  Gender Imbalance: A disproportionate focus on women’s products, coupled with fewer premium and luxury men’s offerings, limits growth potential.

# Methodology

  Employed Python tools (Pandas, FuzzyWuzzy) to clean and standardize text fields, compressing color categories from over 4,000 to 33 standard groups, and correcting thousands of brand name typos (e.g., “allensolly” to “allen-solly”).

  Grouped products by price bands (Budget, Mid-range, Premium, High-End, Luxury) and gender, removing outliers using the Interquartile Range (IQR) method to focus on typical trends.

  Utilized statistical analyses including ANOVA and t-tests to assess significant differences in discount strategies across price and gender segments.

  Visualized insights using bar charts, boxplots, heatmaps, treemaps, and scatterplots to clearly communicate patterns.

# Insights & Findings

  Clean Data Transforms Usability: Reliable and standardized product attribute data improved search results and recommendation quality.

  Discounting Patterns: Mid-range and premium items typically receive deeper and more consistent discounts; however, luxury discounting is erratic, sometimes exceeding mass-market levels, which is unusual and potentially detrimental to brand perception.

  Gender Disparity in Catalogue: Women’s products comprise 57.6% of the catalog and drive majority sales volume, while men’s premium and luxury segments show significant underrepresentation.

  Pricing Correlation: A strong positive correlation (Pearson r = 0.81) exists between original and discounted prices, indicating rational discounting practices with opportunities for refinement in luxury tiers.

# Recommendations

  Implement Regular Automated Data Cleaning: Establish ongoing processes to maintain accurate, consistent product information, fostering customer trust and enhancing discovery.

  Expand Men’s Premium and Luxury Offerings: Target underserved segments to seize growth opportunities and balance the catalog.

  Develop Consistent Luxury Discounting Policies: Protect brand prestige by applying clear, data-driven discount strategies in the luxury category.

  Invest in Bestselling Brands and Popular Colors: Prioritize inventory and marketing around dominant brands (Jolie-Robe, Max, Puma) and favored colors (blue, black) to maximize sales.

  Adopt Discounting Strategies by Price Bands: Tailor discounts thoughtfully across price tiers to optimize profit margins and customer satisfaction.

# Project Structure

text
ajio-fashion-customer-experience/
├── data/                 # Raw and cleaned datasets  
├── notebooks/            # Jupyter notebooks for exploratory analysis and visualization  
├── src/                  # Scripts for data processing and modeling  
├── reports/              # Proposal and final project reports  
├── slides/               # Viva presentation slides  
├── README.md             # Project documentation  
├── requirements.txt      # Python package dependencies  
└── LICENSE               # Licensing information  
