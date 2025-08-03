# Children-comigration
The Institutional Barriers Drive Family Separation in Urbanizing China
This repository contains the data and code for the study titled, "The institutional barriers drive family separation in urbanizing China." The multilevel regression models use a dataset derived from the 2017 China Migrant Dynamics Monitoring Survey (CMDS), which has been merged with city-level policy data.

This document provides a detailed description of the 16 variables used in the analysis.

A. Dependent Variable
MIGRANT
Description: The binary outcome variable indicating the co-migration status of a child.

Type: Binary

Coding:

1: The child co-migrates with their parent(s) in the destination city.

0: The child is left behind in their place of household registration.

B. Grouping Variable (Level 2)
city_code
Description: A unique numerical identifier for each of the 119 destination cities included in the multilevel model analysis.

Type: Categorical (Identifier)

Coding: Each number corresponds to a specific city.

C. Level 1 Variables (Individual/Household Level)
child_gender
Description: The gender of the child.

Type: Categorical (Binary)

Coding:

1: Boy (Reference group)

0: Girl

child_agegroup
Description: The age of the child, grouped into five categories corresponding to educational stages.

Type: Categorical

Coding:

1: 0-2 years (Infancy/Pre-kindergarten) (Reference group)

2: 3-5 years (Kindergarten)

3: 6-11 years (Primary school)

4: 12-14 years (Junior high school)

5: 15-17 years (Senior high school)

child_hukougroup
Description: The household registration (hukou) type of the child.

Type: Categorical (Binary)

Coding:

0: Rural Hukou (Reference group)

1: Urban Hukou

parent_gender
Description: The gender of the migrant parent respondent.

Type: Categorical (Binary)

Coding:

0: Male (Reference group)

1: Female

parent_edu2
Description: The educational attainment of the parent, measured in years of schooling.

Type: Continuous

Coding: Higher values indicate more years of education.

parent_job_ext
Description: The occupation type of the parent.

Type: Categorical

Coding:

1: Production (e.g., manufacturing, construction) (Reference group)

2: Service (e.g., retail, hospitality)

3: Business / Self-employed

4: Professional / Technical / Managerial

5: Others

6: Unemployed / Not in the labor force

household_income
Description: The natural logarithm of the total monthly household income.

Type: Continuous

Coding: Higher values indicate higher income.

household_numberofkids
Description: The total number of children under 18 in the family.

Type: Categorical

Coding:

1: One child (Reference group)

2: Two children

... and so on.

parent_migration_distance
Description: The geographic scale of the parent's migration.

Type: Categorical

Coding:

1: Inter-provincial (migration across provinces) (Reference group)

2: Intra-provincial (migration within the same province but across cities)

3: Intra-prefectural (migration within the same prefecture-level city)

household_rent
Description: The natural logarithm of the monthly household rent in the destination city.

Type: Continuous

Coding: Higher values indicate higher rent.

D. Level 2 Variables (City Level)
city_region
Description: The geographical region where the destination city is located.

Type: Categorical

Coding:

1: Eastern China (Reference group)

2: Central China

3: Western China

4: Northeastern China

city_pop_log
Description: The natural logarithm of the city's urban district (chengqu) population, based on the 2020 census.

Type: Continuous

Coding: Higher values indicate a larger city population.

city_edu
Description: A categorical index representing the stringency of the child school enrollment threshold in the destination city.

Type: Categorical

Coding:

1: Lowest barrier (e.g., no specific requirements) (Reference group)

2: Requires basic certificates (hukou book, temp. residence permit).

3: Requires a formal residence permit.

4: Requires time-based records (e.g., social security payments).

5: Requires additional proofs (e.g., housing ownership).

6: Highest barrier (points-based enrollment system).

composite_peri2_pp
Description: The Parental Hukou Settlement Threshold Index. This is a continuous measure of the difficulty for a migrant parent to obtain a local hukou in the destination city.

Type: Continuous

Coding: Higher values indicate a stricter settlement threshold (it is more difficult to obtain a local hukou).
