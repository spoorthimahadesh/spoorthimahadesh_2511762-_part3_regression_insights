# Model Comparison

## 1. Model Names

### Simple Regression Model

* Dependent Variable: `monthly_sales`
* Independent Variable: `marketing_spend`

### Multiple Regression Model

* Dependent Variable: `monthly_sales`
* Independent Variables:

  * marketing_spend
  * footfall
  * staff_count
  * inventory_availability_pct
  * customer_rating
  * region dummy variables

---

## 2. Variables Used

| Model               | Variables Used                                                                                   |
| ------------------- | ------------------------------------------------------------------------------------------------ |
| Simple Regression   | marketing_spend                                                                                  |
| Multiple Regression | marketing_spend, footfall, staff_count, inventory availability, customer rating, dummy variables |

---

## 3. R-squared Comparison

The simple regression model explained only a portion of the variation in monthly sales because it considered only one predictor.

The multiple regression model achieved a higher R² value, indicating stronger explanatory power because it considered multiple factors affecting sales.

| Model               | R²       |
| ------------------- | ---------|
| Simple Regression   | (0.1679) |
| Multiple Regression | (0.7476) |

---

## 4. Significant Variables

In the simple regression model, marketing spend was statistically significant.

In the multiple regression model, variables such as footfall, marketing spend, inventory availability, and customer rating were statistically significant because their p-values were below 0.05.

Variables with p-values greater than 0.05 were considered statistically weak.

---

## 5. Business Usefulness

The simple regression model helps understand the impact of a single factor on sales.

The multiple regression model is more useful for business decision-making because it simultaneously evaluates several factors influencing monthly sales.

Management can use the multiple regression model to optimize marketing spending, staffing, inventory levels, and regional strategies.

---

## 6. Limitations

### Simple Regression

* Considers only one independent variable.
* Ignores interactions among business factors.

### Multiple Regression

* Results may be affected by multicollinearity.
* Does not capture external factors such as economic conditions or competitor strategies.
* Assumes linear relationships between variables.

