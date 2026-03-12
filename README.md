# Logistics-Route-Optimization-and-Transport-Cost-Analysis
This project focuses on analyzing transportation costs and optimizing delivery routes in a logistics network using Python. The main objective is to reduce logistics expenses by identifying the most cost-effective truck assignments and determining efficient routes between delivery locations.


#Transport Cost calculation
<img width="244" height="64" alt="transport cost calculation" src="https://github.com/user-attachments/assets/bb280d3e-f9b1-4f8a-ac12-9c6de3ab0b3a" />

For locations such as “52” and “52 Mine,” the 30-ton truck is cheaper (12.60) compared to the 20-ton truck (14.40). This means using the larger truck is the more cost-efficient option for these routes.
For locations like “20 Resort-Murombedzi,” “Alabama,” and “Banket,” the cost is the same for both truck types. This means the company can use either truck without affecting transportation cost.
The costs vary widely between locations. For example:
Deliveries to 52 cost around 12.60, which is very low.
Deliveries to Banket cost over 5191, which is much higher.

#Optimal Truck Assignment (Hungarian Algorithm)
<img width="185" height="33" alt="Hungarian Algorinthm" src="https://github.com/user-attachments/assets/6127d318-4074-4ec7-af8f-f1e13b169bb6" />

This result shows the best truck choice for delivering to each area in order to keep transportation costs as low as possible.

For Blue Bird, the analysis recommends using a 30-ton tipper truck, with an estimated transport cost of 11.2.
This means the larger truck is the most cost-efficient option for delivering to this location.
For Blue Bird Claim 14, the recommended vehicle is a 20-ton tipper truck, with a transport cost of 9.6.
In this case, the smaller truck is cheaper to operate for that route.
The analysis shows that different locations may require different truck sizes to minimize cost. Instead of using the same truck for all deliveries, the system selects the most economical vehicle for each area

#Shortest Path Algorithm (Dijkstra)
<img width="155" height="23" alt="Shortest path Algorithm" src="https://github.com/user-attachments/assets/d5299dff-4876-486a-a328-441f46e7fd26" />

This result shows the most efficient route between two delivery locations.
The shortest route from 52 to Bay-Horse is direct, meaning the best path is simply:
52 → Bay-Horse
The distance between these two locations is 103 units (for example kilometers if distance is measured in km).

Key Insight
This means that no alternative route through other locations would be shorter. Going directly from 52 to Bay-Horse is already the most efficient option.

#Vehicle Routing Model

<img width="368" height="32" alt="vehicle routing problem" src="https://github.com/user-attachments/assets/95bea1e6-d716-41f8-93d2-5137d384a52e" />

These results show how delivery locations have been grouped and assigned to three different trucks to make transportation more organized and efficient.
Truck 1 Route
Truck 1 will deliver materials to the following locations in order:
52 → Alabama → Cricket 5-BF-Ores → Battle Fields → Berks 14.
Truck 2 Route
Truck 2 will handle deliveries to:
20 Resort-Murombedzi → Banket → Cricket 5-BF → Bay-Horse → Berks 13.
Truck 3 Route
Truck 3 will deliver to:
52 Mine → Barkley Chase → Yellow Snake-BF → Berks 11 → Eagle Press.
Key Insight
Instead of sending one truck to every location separately, the system groups nearby locations into routes for each truck

#Route Distance calculation
<img width="114" height="31" alt="Route distance calculation" src="https://github.com/user-attachments/assets/adc56dbf-2b35-4777-a9d5-72fbe5cdd69f" />

These results show the total travel distance each truck will cover to complete its assigned deliveries.
Truck 1 will travel about 362 distance units to deliver materials to all the locations assigned to it.
Truck 2 will travel about 199 distance units, which means it has the shortest route among the three trucks.
Truck 3 will travel about 488 distance units, making it the longest route.

Key Insight
The distances are not equal, which means some trucks are covering more locations or traveling farther than others. Truck 3 has the heaviest travel workload, while Truck 2 has the lightest route.

In simple terms, the analysis shows how far each truck must travel to complete its deliveries. This helps the logistics team see which routes are longer and where improvements could be made to save fuel, reduce costs, and balance truck workloads more efficiently.

#Route Visualization

<img width="341" height="252" alt="Route visualizations" src="https://github.com/user-attachments/assets/48fab7d2-5019-47db-918c-782f36beea6a" />

Key Insight
The chart clearly shows that Truck 3 has the heaviest travel workload, while Truck 2 has the lightest route. This means Truck 3 is likely using more fuel and time compared to the other trucks.

In simple terms:
Some trucks are working harder than others in terms of travel distance.
Longer routes can increase fuel costs, driver time, and maintenance.
The company may consider balancing the routes better so that distances are more evenly distributed among trucks.

Simple Summary
The visualization helps logistics managers quickly see which trucks travel the most and which travel the least, making it easier to improve route planning, reduce transport costs, and manage the fleet more efficiently.

#Overall Transport cost analysis
<img width="197" height="22" alt="transport cost analysis" src="https://github.com/user-attachments/assets/03aab734-5efa-4fb2-827e-59c1450da9de" />

These results summarize the overall transportation spending for all deliveries in the logistics operation.

What the Numbers Mean
The Total Transport Cost (689,904) represents the estimated amount of money required to transport materials to all delivery locations combined.
The Average Cost per Delivery (about 2,623) shows the typical cost of making one delivery to a location.

Key Insight
This means that, on average, each delivery costs the company around 2,623, although some locations may cost much more or much less depending on distance and route conditions.

From a cost-efficiency perspective:
The total cost figure helps management understand the overall transportation budget required.
The average delivery cost acts as a benchmark to identify expensive routes.
If some deliveries cost far above the average, they may need better route planning, different truck allocation, or grouped deliveries to reduce costs.

Simple Summary
In simple terms, the analysis shows how much the company spends on transportation overall and how much each delivery typically costs. This information helps logistics managers identify opportunities to reduce costs and improve transport efficiency across mining supply routes.
