# Source Schema

Types as read from the raw CSV files (Bronze, unchanged).


## olist_customers_dataset.csv

| Column | Source Type | Nullable |
|---|---|---|
| customer_id | str | No |
| customer_unique_id | str | No |
| customer_zip_code_prefix | int64 | No |
| customer_city | str | No |
| customer_state | str | No |

## olist_geolocation_dataset.csv

| Column | Source Type | Nullable |
|---|---|---|
| geolocation_zip_code_prefix | int64 | No |
| geolocation_lat | float64 | No |
| geolocation_lng | float64 | No |
| geolocation_city | str | No |
| geolocation_state | str | No |

## olist_order_items_dataset.csv

| Column | Source Type | Nullable |
|---|---|---|
| order_id | str | No |
| order_item_id | int64 | No |
| product_id | str | No |
| seller_id | str | No |
| shipping_limit_date | str | No |
| price | float64 | No |
| freight_value | float64 | No |

## olist_order_payments_dataset.csv

| Column | Source Type | Nullable |
|---|---|---|
| order_id | str | No |
| payment_sequential | int64 | No |
| payment_type | str | No |
| payment_installments | int64 | No |
| payment_value | float64 | No |

## olist_order_reviews_dataset.csv

| Column | Source Type | Nullable |
|---|---|---|
| review_id | str | No |
| order_id | str | No |
| review_score | int64 | No |
| review_comment_title | str | Yes |
| review_comment_message | str | Yes |
| review_creation_date | str | No |
| review_answer_timestamp | str | No |

## olist_orders_dataset.csv

| Column | Source Type | Nullable |
|---|---|---|
| order_id | str | No |
| customer_id | str | No |
| order_status | str | No |
| order_purchase_timestamp | str | No |
| order_approved_at | str | Yes |
| order_delivered_carrier_date | str | Yes |
| order_delivered_customer_date | str | Yes |
| order_estimated_delivery_date | str | No |

## olist_products_dataset.csv

| Column | Source Type | Nullable |
|---|---|---|
| product_id | str | No |
| product_category_name | str | Yes |
| product_name_lenght | float64 | Yes |
| product_description_lenght | float64 | Yes |
| product_photos_qty | float64 | Yes |
| product_weight_g | float64 | Yes |
| product_length_cm | float64 | Yes |
| product_height_cm | float64 | Yes |
| product_width_cm | float64 | Yes |

## olist_sellers_dataset.csv

| Column | Source Type | Nullable |
|---|---|---|
| seller_id | str | No |
| seller_zip_code_prefix | int64 | No |
| seller_city | str | No |
| seller_state | str | No |

## product_category_name_translation.csv

| Column | Source Type | Nullable |
|---|---|---|
| product_category_name | str | No |
| product_category_name_english | str | No |