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
* **_Vehicle Type Option :_** information about a vehicle or an a transmission method

# Order Option
field | type | example | description
--- | :---: | :---:| ---
**order_id** | string | "abc1234" | ID of order
**order_date** | date format | "2016-12-31" | date of order 
**order_item_qty** | int |  0 | quantity of order item 
**order_constraint** | string | "weight" / "volume" / "time" | constraint of cluster is limit by either weight (loading capacity), volume (loading capacity) , or time (day time window)

# Dc Option
field | type | example | description
--- | :---: | :---: | ---
**dc_id** | string | "abc1234" | ID of distribution center
**dc_longitude** | double |0.0 | longitude of distribution center
**dc_latitude** | double | 0.0 | latitude of distribution center
**dc_departure_time** | int | 8 | departure time at distribution center 
**dc_return_after_done** | boolean | true / false | return to distrubution center after done

# Customer Option
field | type | example | description
--- | :---: | :---: | ---
**customer_id** | string | "abc1234" | ID of customer
**customer_longitude** | double | 0.0 | longitude of customer
**customer_latitude** | double | 0.0 | latitude of customer

# Product Option
field | type | example | description
--- | :---: | :---: | ---
**product_id** | string | "abc1234" | ID of product
**product_weight_kg** | double | 0.0 | weight of product in kilogram
**product_volume_m3** | double | 0.0 | volume of product in cubic meter
**product_delay_unloading_minute** | int | 0.0 | delay when unloading product in minute
      
# Vehicle Type Option
field | type | example | description
--- | :---: | :---: | ---
**vehicle_type_id** | string | "abc1234" | ID of vehicle type
**vehicle_type_priority** | int | 0 | Priority of vehicle type
**vehicle_type_quantity** | int | 0 | quantity of vehicle type
**vehicle_type_max_working_h** | int | 0.0 | max window time in hour, one day of vehicle type
**vehicle_type_max_volume_m3** | double | 0.0 | max volume in cubic meter of vehicle type
**vehicle_type_max_loading_kg** | double | 0.0 | max loading in kilogram of vehicle type
**vehicle_type_max_distance_km** | double | 0.0 | max distance between connected drops in kilometer of vehicle type
**vehicle_type_delay_travel_minute** | int | 0 | delay of travelling between drops in minute of vehicle type
