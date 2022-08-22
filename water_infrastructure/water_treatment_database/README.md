## Data Source

The water treatment plant database contains 4 columns: Water Treatment Plants, Capacity (BG), Inflow (BGD), and Outflow (BGD). There are two water treatment plants: Catskill-Delaware Water Ultraviolet Disinfection Facility and Croton Water Filtration Plant. For clarification, the Capacity portrays how much water a plant can filter in on a daily basis. Catskill-Delaware Water UV Disinfection Facility’s Capacity was available from an article from Water-Technology [15], and Capacity for Croton Water Filtration Plant was accessible from the NYC government database [16]. While Inflow data is essentially the sum of reservoirs’ Outflows, there was no attainable data with each of the water treatment plant’s Outflow; therefore, we had to make a deduction by formulating a calculation of water demand and each plant’s capacity. 

## Data Handling

There were two water treatment plants that were handled: Catskill-Delaware Water Ultraviolet Disinfection Facility and Croton Water Filtration Plant.  The Capacity (BG) was in the desired measurement, The Inflow data measured in billion gallons per day (BGD) was calculated by adding up the Outflows from the reservoirs associated with their designated plants. The Outflow (BGD) data was not available, so we had to extrapolate this data from existing databases like the Water Demand Database. 

Catskill-Delaware Water UV Disinfection Facility Outflow:
(Demand * (CapacityCatskill-Delaware / CapacityCatskill-Delaware + CapacityCroton))

Croton Water Filtration Plant Outflow: 
(Demand * (CapacityCroton / CapacityCroton + CapacityCatskill-Delaware))

The Demand was acquired from the Water Demand Database’s total daily water use (kgal/d) and Capacity (BG) for both water treatment plants were already available. After taking the sum of the daily demand, it was converted to BGD and calculated with the Capacity values to derive to our Outflow data. 
