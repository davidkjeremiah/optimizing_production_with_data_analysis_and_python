# Project Title

Optimizing Production with Data Analysis and Python for a Nylon Production Company (Strong Marence Venture)

## Production Data

The production data contains the following features:

* `machine_id:` The unique identifier for each machine.
* `machine_type:` The type of machine (e.g. "cutting machine", "extruding machine", etc.).
* `production_time:` The amount of time it took to produce the nylon on this machine.
* `product_type:` The type of nylon being produced (e.g. "textile grade", "industrial grade", etc.).
* `production_volume:` The amount of nylon produced during this production run.
* `production_date:` The date on which this production run took place.
* `production_shift:` The shift during which this production run took place (e.g. "day shift", "night shift").
* `machine_maintenance:` Information about when each machine was last serviced, as well as any maintenance issues that arose during production.
* `raw_material_usage:` Information about the raw materials used in this production run, such as the type and quantity of chemicals used.
* `quality_control:` Information about any quality control measures that were taken during production, such as testing for defects or measuring the dimensions of the finished products.

## Methodology

This code provided does the following:

1. Load the production data from a CSV file into a Pandas DataFrame.
2. Calculate the total production time for each machine (e.g. "cutting machine", "extruding machine", etc.) by grouping the data by machine type and summing the production time for each group.
3. Finds the machine type with the highest production time.
4. Calculates the average production time per machine type.
5. Finds the machine types that are underperforming (production time below average).
6. Moves some of the workload from the most productive machine type to the underperforming machine types.
7. Saves the updated schedule to a new CSV file.

## Insights

The fact that the *most productive* extruding machine is `'extruding machine A'` and the *underperforming* machines include `'extruding machine B'` and `'extruding machine D'` suggests that there may be some differences in performance between these machines. It could be that `'extruding machine A'` is more efficient or has better maintenance, leading to higher production output. On the other hand, `'extruding machine B'` and `'extruding machine D'` may be performing poorly due to issues such as a lower production capacity, longer production times, or more frequent breakdowns.

To further understand the differences in performance between these machines, it might be helpful to gather more data on factors such as `production capacity`, `production time`, `maintenance frequency`, and `raw material usage`. This additional data could help identify specific areas where 'extruding machine A' is outperforming the other machines, and suggest potential improvements that could be made to increase the performance of 'extruding machine B' and 'extruding machine D'.

## Note

The project is for educational purposes only and the data are not the actual data used by the nylon-production company in consideration, and the insights and recommendations presented here are made based on the analysis of the data.
