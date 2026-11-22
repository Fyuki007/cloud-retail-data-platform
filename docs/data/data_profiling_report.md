# Data Profiling Report


## olist_customers_dataset.csv

- Rows: 99,441  |  Columns: 5
- Duplicate rows: 0

| Column | Type | Missing | Missing % | Unique |
|---|---|---|---|---|
| customer_id | str | 0 | 0.0% | 99,441 |
| customer_unique_id | str | 0 | 0.0% | 96,096 |
| customer_zip_code_prefix | int64 | 0 | 0.0% | 14,994 |
| customer_city | str | 0 | 0.0% | 4,119 |
| customer_state | str | 0 | 0.0% | 27 |

## olist_geolocation_dataset.csv

- Rows: 1,000,163  |  Columns: 5
- Duplicate rows: 261,831

| Column | Type | Missing | Missing % | Unique |
|---|---|---|---|---|
| geolocation_zip_code_prefix | int64 | 0 | 0.0% | 19,015 |
| geolocation_lat | float64 | 0 | 0.0% | 717,360 |
| geolocation_lng | float64 | 0 | 0.0% | 717,613 |
| geolocation_city | str | 0 | 0.0% | 8,011 |
| geolocation_state | str | 0 | 0.0% | 27 |

## olist_order_items_dataset.csv

- Rows: 112,650  |  Columns: 7
- Duplicate rows: 0

| Column | Type | Missing | Missing % | Unique |
|---|---|---|---|---|
| order_id | str | 0 | 0.0% | 98,666 |
| order_item_id | int64 | 0 | 0.0% | 21 |
| product_id | str | 0 | 0.0% | 32,951 |
| seller_id | str | 0 | 0.0% | 3,095 |
| shipping_limit_date | str | 0 | 0.0% | 93,318 |
| price | float64 | 0 | 0.0% | 5,968 |
| freight_value | float64 | 0 | 0.0% | 6,999 |

## olist_order_payments_dataset.csv

- Rows: 103,886  |  Columns: 5
- Duplicate rows: 0

| Column | Type | Missing | Missing % | Unique |
|---|---|---|---|---|
| order_id | str | 0 | 0.0% | 99,440 |
| payment_sequential | int64 | 0 | 0.0% | 29 |
| payment_type | str | 0 | 0.0% | 5 |
| payment_installments | int64 | 0 | 0.0% | 24 |
| payment_value | float64 | 0 | 0.0% | 29,077 |

## olist_order_reviews_dataset.csv

- Rows: 99,224  |  Columns: 7
- Duplicate rows: 0

| Column | Type | Missing | Missing % | Unique |
|---|---|---|---|---|
| review_id | str | 0 | 0.0% | 98,410 |
| order_id | str | 0 | 0.0% | 98,673 |
| review_score | int64 | 0 | 0.0% | 5 |
| review_comment_title | str | 87,656 | 88.3% | 4,527 |
| review_comment_message | str | 58,247 | 58.7% | 36,159 |
| review_creation_date | str | 0 | 0.0% | 636 |
| review_answer_timestamp | str | 0 | 0.0% | 98,248 |

## olist_orders_dataset.csv

- Rows: 99,441  |  Columns: 8
- Duplicate rows: 0

| Column | Type | Missing | Missing % | Unique |
|---|---|---|---|---|
| order_id | str | 0 | 0.0% | 99,441 |
| customer_id | str | 0 | 0.0% | 99,441 |
| order_status | str | 0 | 0.0% | 8 |
| order_purchase_timestamp | str | 0 | 0.0% | 98,875 |
| order_approved_at | str | 160 | 0.2% | 90,733 |
| order_delivered_carrier_date | str | 1,783 | 1.8% | 81,018 |
| order_delivered_customer_date | str | 2,965 | 3.0% | 95,664 |
| order_estimated_delivery_date | str | 0 | 0.0% | 459 |

## olist_products_dataset.csv

- Rows: 32,951  |  Columns: 9
- Duplicate rows: 0

| Column | Type | Missing | Missing % | Unique |
|---|---|---|---|---|
| product_id | str | 0 | 0.0% | 32,951 |
| product_category_name | str | 610 | 1.9% | 73 |
| product_name_lenght | float64 | 610 | 1.9% | 66 |
| product_description_lenght | float64 | 610 | 1.9% | 2,960 |
| product_photos_qty | float64 | 610 | 1.9% | 19 |
| product_weight_g | float64 | 2 | 0.0% | 2,204 |
| product_length_cm | float64 | 2 | 0.0% | 99 |
| product_height_cm | float64 | 2 | 0.0% | 102 |
| product_width_cm | float64 | 2 | 0.0% | 95 |

## olist_sellers_dataset.csv

- Rows: 3,095  |  Columns: 4
- Duplicate rows: 0

| Column | Type | Missing | Missing % | Unique |
|---|---|---|---|---|
| seller_id | str | 0 | 0.0% | 3,095 |
| seller_zip_code_prefix | int64 | 0 | 0.0% | 2,246 |
| seller_city | str | 0 | 0.0% | 611 |
| seller_state | str | 0 | 0.0% | 23 |

## product_category_name_translation.csv

- Rows: 71  |  Columns: 2
- Duplicate rows: 0

| Column | Type | Missing | Missing % | Unique |
|---|---|---|---|---|
| product_category_name | str | 0 | 0.0% | 71 |
| product_category_name_english | str | 0 | 0.0% | 71 |