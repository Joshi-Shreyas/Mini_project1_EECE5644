# Cleaning Decisions Log

- Kept the raw dataset unchanged as `df` and created cleaned copies for analysis.
- Standardized country names: `EIRE` to `Ireland`, `RSA` to `South Africa`, and `Unspecified` to missing.
- Renamed columns to snake_case, such as `InvoiceNo` to `invoice_no` and `UnitPrice` to `unit_price`.
- Kept missing `customer_id` rows for overall sales analysis, but excluded them from customer-level analysis.
- Removed cancellations, returns, invalid quantities, invalid prices, duplicate rows, and non-product lines from the completed-sales dataset.
- Removed non-product stock codes such as `POST`, `DOT`, `M`, `BANK CHARGES`, and `AMAZONFEE` because they are fees, postage, or adjustments.
- Cleaned product descriptions by stripping extra spaces and standardizing text format.
- Added `revenue = quantity * unit_price` for sales analysis.
- Converted `invoice_date` to datetime for monthly and weekly trend analysis.
- Merged a country-to-region lookup table using a left join so valid sales rows would not be dropped.
- Final assumption: the cleaned dataset represents completed product sales only. Missing customer IDs may limit customer-level conclusions.
