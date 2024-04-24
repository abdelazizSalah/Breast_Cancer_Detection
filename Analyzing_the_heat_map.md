# Analyzing the heat map
* Based on the above heatmap, we can see that there are some features that are highly correlated with each other, such as redius mean, and perimeter mean, and area mean, they are perfectly correleated, which mean that only one feature of them, can represent the others. 
* Here we can apply PCA algorithm, to be able to select the important features only. 
* lets make a list of highley correlated features, and then we will apply PCA algorithm to select the important features only.
* diagnosis = {radius_mean, perimeter_mean, area_mean, concavity_mean, concavity_points_mean, radius_worst, perimeter_worst, area_worst, concave_point_worst}
* redius_mean = {perimeter_mean, area_mean, concave_points_mean, radius_worst, perimeter_worst, area_worst}
* texture_mean = {texture_worst}
* perimeter_mean = {radius_mean, area_mean, concave_points_mean, radius_worst, perimeter_worst, area_worst}
* area_mean = {radius_mean, perimeter_mean, concave_points_mean, radius_worst, perimeter_worst, area_worst}
* smoothness_mean = {smoothness_worst}
* compactness_mean = {compactness_worst, concavity_worst, concavity_mean, concave_points_worst, concave_points_mean}
* concavity_mean = {compactness_worst, concavity_worst, concave_points_worst, concave_points_mean, compactness_mean,texture_worst,}
* concave_points_mean = {radius_mean, perimeter_mean, area_mean, compactness_mean, concavity_mean, radius_worst, perimeter_worst, area_worst, concave_points_worst}
* 