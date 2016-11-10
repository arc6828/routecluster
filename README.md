# Route Cluster
* Cluster your route from nodes of orders

# Usage
* Simply use jquery to send post data

# Data
* List of orders

# Order
* **_Order Option :_** information about an order
* **_Dc Option :_**  information about a distribution center or an origin place
* **_Product Option :_** information about a product or an item
* **_Customer Option :_** information about a customer or a destination place
* **_Vehicle Option :_** information about a vehicle or an a transmission method

# Order Option
field | type | example | description
--- | :---: | :---:| ---
**order_id** | string | "abc1234" |
**order_date** | date format | "2016-12-31" | 
**order_item_qty** | int |  0 | 
**order_constraints** | string | "weight" / "volume" / "time" |

# Dc Option
field | type | example | description
--- | :---: | :---: | ---
**dc_id** | string | "abc1234" |
**dc_longitude** | double |0.0 |
**dc_latitude** | double | 0.0 |
**dc_departure_time** | int | 8 |
**dc_return_after_done** | boolean | true / false |

# Customer Option
field | type | example | description
--- | :---: | :---: | ---
**customer_id** | string | "abc1234" |
**customer_longitude** | double | 0.0 |
**customer_latitude** | double | 0.0 |

# Product Option
field | type | example | description
--- | :---: | :---: | ---
**product_id** | string | "abc1234" |
**product_weight_kg** | double | 0.0 |
**product_volume_m3** | double | 0.0 |
**product_delay_unloading_minute** | int | 0.0 |
      
# Vehicle Option
field | type | example | description
--- | :---: | :---: | ---
**vehicle_id** | string | "abc1234" |
**vehicle_priority** | int | 0 |
**vehicle_quantity** | int | 0 |
**vehicle_max_working_h** | int | 0.0 |
**vehicle_max_volume_m3** | double | 0.0 |
**vehicle_max_loading_kg** | double | 0.0 |
**vehicle_max_distance_km** | double | 0.0 |
**vehicle_delay_travel_minute** | int | 0 |
