# TrendWear Fashion Retail Analytics (Codegnan Hackathon)

Data cleaning and exploratory data analysis (EDA) for the TrendWear retail case: sales, discounts, customers, promotions and stock.

## Project structure
```
TrendWear_Project/
├── data/
│   ├── raw/        sales.csv, Stores_csv.csv, stock.csv, promotion.csv, _Products.csv
│   └── cleaned/    created automatically by the notebook
├── notebooks/
│   └── TrendWear_EDA.ipynb
└── README.md
```

## Requirements
- Python 3.9 or higher
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `jupyter`

```
pip install pandas numpy matplotlib seaborn jupyter
```

## How to run
1. Put the 5 CSV files in `data/raw/`.
2. Open a terminal in the `notebooks/` folder and run `jupyter notebook`.
3. Open `TrendWear_EDA.ipynb` and choose **Kernel > Restart & Run All**.
4. Cleaned files are saved to `data/cleaned/`.

## Data files
| File | Contents |
|---|---|
| `sales.csv` | 500 bill line items (qty, MRP, selling price, discount per unit) |
| `Stores_csv.csv` | Transaction details (date, category, customer, payment, footfall, stock remaining) |
| `stock.csv` | Opening, received and closing stock for 21 products |
| `promotion.csv` | 12 promotion campaigns for 2026 |
| `_Products.csv` | Electronics catalogue, unrelated to the fashion data (excluded) |

## Headline results
- Total sales: Rs. 17.03 lakh | Average bill value: Rs. 3,406 | Sales per sq ft: Rs. 568
- Women and Men give 59% of sales; 13 of 21 products give 80% of sales
- Discounts show no effect on units sold; only 8% of promo-day bills carry the campaign discount
- Overall sell-through is 50%; Jeans and Sneakers need restocking, while Schoolwear, Watch, Belt, Cap and Wallet are overstocked

## Limitations
- No cost price, so Gross Margin % is not calculated (discount leakage is used as a proxy)
- No stock receipt dates, so stock cover days replace stock ageing
- Single store and one product per bill, so store comparison and market basket analysis are not possible

## Next steps
SQL analysis (MySQL), Excel pivot summaries, Power BI dashboard with DAX, report and presentation.
