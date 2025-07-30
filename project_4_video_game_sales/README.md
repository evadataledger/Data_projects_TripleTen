# Project 4: Video Game Sales Forecasting (Integrated Anaysis) 

## Objective

To identify patterns that contribute to the commerical success of video games across regions, platforms, and genres using 2016 data - to forecast trends and guide a 2017 marketing strategy. 

## Dataset
`games.csv` contains gam names, platforms, release year, sales by region, critic/user scores, genres, and ESRB ratings. 

## Tools Used
- Python (`pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`)
- Jupyter Notebook

## Key Stages 

1. **Data Overview & Cleaning**
   - Standardized column names
   - Converted dtypes
   - Handled missing values (`TBD` & `NaN`)
   - Calculated `total_sales`

2. **Sales Trend Analysis**
   - Platforms ranked by total sales over time
   - Determined lifecycle trends for platforms
   - Explored genre popularity & profitability

3. **Regional Profiles**
   - Top platforms & genres in NA, EU, JP
   - Examined ESRB influence by region

4. **Hypothesis Testing**
   - Are average user ratings equal on Xbox One and PC?
   - Are ratings for Action vs Sports genres different?


---

## Key Insights

- Platforms like PS4 and XOne dominated in global sales
- Strong correlation between critic score and sales on top platforms
- Regional preferences (e.g., Japan prefers handheld consoles like 3DS)
- Action and Shooter genres remain top-selling worldwide

---

## Folder Structure

```bash
project_4_video_game_sales/
├── notebooks/
│   └── project_4_integrated_clean.ipynb
├── data/
│   └── games.csv
├── README.md
├── requirements.txt
