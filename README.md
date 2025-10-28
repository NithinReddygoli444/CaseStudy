Health Survey Analysis: Social and Health Determinants in India 🇮🇳

This project presents a comprehensive, data-driven analysis of the interdependencies between core social, environmental, and health indicators across various Indian States and Union Territories (UTs). The primary goal of this research is to move beyond simple reporting by identifying strong correlations and determinants of key public health challenges, notably **Child Stunting**, using aggregated data from a large-scale district health survey.

---

##  Methodology and Data Framework

The foundation of this analysis rests upon the **`district_health_survey_updated_2024.csv`** dataset, which compiles vital statistics across six key indicators: **Female School Attendance**, **Improved Sanitation**, **Clean Fuel** usage, **Early Marriage** prevalence, **Modern Family Planning** method adoption, and **Child Stunting**.

The analysis employs a robust data processing pipeline built with **PySpark** to handle the large, district-level data efficiently. Following initial data cleaning and transformation, the metrics were aggregated to the State/UT level using PySpark's distributed capabilities. This aggregated data was then passed to **Pandas** for intensive statistical analysis, including the calculation of descriptive statistics and a **Correlation Matrix**. Finally, **Matplotlib** and **Seaborn** were used to generate compelling visualizations, such as correlation heatmaps and bivariate scatter plots, to communicate the derived insights effectively.

---

##  Key Findings and Interpretive Discussion

The project’s findings underscore that health outcomes in India are fundamentally linked to socio-economic development, with clear regional disparities persisting across the country.

### The Education-Health Nexus

The analysis reveals a significant **negative correlation** between **Female School Attendance** and **Child Stunting**. This is a powerful demonstration of the returns on investing in girls' education. Educated women are more likely to possess the health literacy and decision-making authority necessary to ensure proper nutrition, sanitation, and healthcare for their children, thereby breaking the intergenerational cycle of undernutrition.

### Environmental Health as a Stunting Determinant

Stunting is shown to be a multidimensional problem extending beyond mere food intake. The strong **negative correlations** between Stunting, **Improved Sanitation**, and **Clean Fuel** usage confirm the role of the environment. In regions lacking proper sanitation, children are vulnerable to chronic infections and diarrhoeal diseases, which prevent nutrient absorption, a condition known as Environmental Enteropathy (EE). Similarly, low access to clean cooking fuel exposes mothers and children to household air pollution (HAP), which is linked to respiratory illness and poor maternal health, further compounding the risk of stunting. The visualization of the **positive relationship between Improved Sanitation and Clean Fuel** usage highlights that states successfully implementing one form of infrastructure improvement tend to succeed in others, reflecting a convergence of modernization efforts.

### The Impact of Early Marriage

The data exposes **Early Marriage** as a key driver of poor social and health outcomes. It exhibits a **positive correlation with Child Stunting** and a **negative correlation with welfare indicators** like school attendance, improved sanitation, and clean fuel use. Girls who marry early are often denied further education, have limited agency in household decisions, and face the biological risks of early, high-frequency pregnancies, all of which directly contribute to poor maternal health and higher rates of stunted children.

### Regional Disparity

The visualization of state performance clearly identifies that while the Southern and certain Northeastern states tend to lead on key development indicators, central and eastern states like **Bihar, Jharkhand, and Uttar Pradesh** continue to face the highest burden of stunting and lag significantly in school attendance and sanitation access. This necessitates targeted, multi-sectoral policy interventions that address these deep-seated, intersecting deprivations simultaneously.

---

##  Limitations and Future Scope

While the analysis successfully identifies robust correlations, it is important to acknowledge certain limitations. First, the cross-sectional nature of the survey only allows for the identification of statistical **correlation, not causation**. Second, state-level aggregation masks significant sub-state heterogeneity, potentially overlooking localized successes or pockets of extreme deprivation. Future work should focus on incorporating time-series data to track progress, employing causal inference models, and utilizing interactive dashboards to allow for deeper, on-demand exploration of district-level variations.
