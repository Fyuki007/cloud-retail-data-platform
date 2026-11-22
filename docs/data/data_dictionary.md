# Data Dictionary

Source: Olist Brazilian E-Commerce dataset (Kaggle). Store dimension = Sellers (assumption, see Data Contract).

## orders
| Column | Description | Key |
|---|---|---|
| order_id | Unique order identifier | PK |
| customer_id | Customer identifier for this order (changes per order) | FK → customers |
| order_status | delivered, shipped, canceled, unavailable, invoiced, processing, created, approved | |
| order_purchase_timestamp | When the order was placed | |
| order_approved_at | Payment approval time | |
| order_delivered_carrier_date | Handed to the carrier | |
| order_delivered_customer_date | Delivered to the customer | |
| order_estimated_delivery_date | Estimated delivery date | |

## order_items
| Column | Description | Key |
|---|---|---|
| order_id | Order identifier | PK, FK → orders |
| order_item_id | Item sequence number within the order | PK |
| product_id | Product identifier | FK → products |
| seller_id | Seller identifier | FK → sellers |
| shipping_limit_date | Seller's shipping deadline | |
| price | Item price | |
| freight_value | Freight cost for the item | |

## customers
| Column | Description | Key |
|---|---|---|
| customer_id | Per-order customer key | PK |
| customer_unique_id | Real unique customer | |
| customer_zip_code_prefix | First 5 digits of the zip code | |
| customer_city | City | |
| customer_state | State code | |

## products
| Column | Description | Key |
|---|---|---|
| product_id | Product identifier | PK |
| product_category_name | Category (Portuguese) | FK → translation |
| product_name_lenght | Name length in characters (misspelled in source) | |
| product_description_lenght | Description length (misspelled in source) | |
| product_photos_qty | Number of photos | |
| product_weight_g | Weight in grams | |
| product_length_cm / product_height_cm / product_width_cm | Dimensions in cm | |

## sellers (used as Stores)
| Column | Description | Key |
|---|---|---|
| seller_id | Seller identifier | PK |
| seller_zip_code_prefix | Zip code prefix | |
| seller_city | City | |
| seller_state | State code | |

## order_payments
| Column | Description | Key |
|---|---|---|
| order_id | Order identifier | PK, FK → orders |
| payment_sequential | Payment sequence within the order | PK |
| payment_type | credit_card, boleto, voucher, debit_card, not_defined | |
| payment_installments | Number of installments | |
| payment_value | Payment amount | |

## product_category_name_translation
| Column | Description | Key |
|---|---|---|
| product_category_name | Category (Portuguese) | PK |
| product_category_name_english | Category (English) | |

## order_reviews, geolocation
Not used in the Star Schema (pending agreement with Member 1). Loaded to Bronze as is.