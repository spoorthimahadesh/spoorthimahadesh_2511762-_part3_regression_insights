# Dummy Variable Creation

Categorical variables `region` and `store_type` were converted into dummy variables to enable their use in regression analysis.

For the `region` variable, **East** was selected as the reference category. Three dummy variables were created: `Region_North`, `Region_South`, and `Region_West`.

For the `store_type` variable, **Mall** was selected as the reference category. Two dummy variables were created: `Store_HighStreet` and `Store_Residential`.

Reference categories were excluded from the regression model to avoid multicollinearity and the dummy variable trap.


# TASK 8

# Model Equations

## 1. Simple Regression Equation

The simple regression model was developed to understand the relationship between marketing spend and monthly sales.

### Equation

Monthly Sales = Intercept + (Marketing Spend Coefficient × Marketing Spend)

Example:

Monthly Sales = 120000 + (1.25 × Marketing Spend)

### Business Interpretation

* **Intercept (120000):**
  When marketing spend is zero, the model predicts baseline monthly sales of approximately ₹120,000.

* **Marketing Spend Coefficient (1.25):**
  For every additional ₹1 invested in marketing, monthly sales are expected to increase by approximately ₹1.25.

---

## 2. Multiple Regression Equation

The multiple regression model includes several business factors influencing sales.

### Equation

Monthly Sales = Intercept

* (β1 × Marketing Spend)
* (β2 × Footfall)
* (β3 × Staff Count)
* (β4 × Inventory Availability)
* (β5 × Customer Rating)
* (β6 × Region_North)
* (β7 × Region_South)
* (β8 × Region_West)
* (β9 × Store_HighStreet)
* (β10 × Store_Residential)

Example:

Monthly Sales =
50000

* (1.20 × Marketing Spend)
* (27.38 × Footfall)
* (3483.41 × Staff Count)
* (3060.20 × Inventory Availability)
* (12450 × Customer Rating)
* (15000 × Region_North)
* (21040 × Region_South)
* (25260 × Region_West)

- (24300 × Store_HighStreet)
- (44680 × Store_Residential)

---

## 3. Explanation of Each Coefficient

| Variable               | Business Interpretation                                                    |
| ---------------------- | -------------------------------------------------------------------------- |
| Marketing Spend        | Higher marketing investment is associated with increased sales.            |
| Footfall               | More customer visits lead to higher sales.                                 |
| Staff Count            | Additional staff can improve customer service and increase revenue.        |
| Inventory Availability | Maintaining stock availability helps prevent lost sales.                   |
| Customer Rating        | Better customer satisfaction contributes positively to sales.              |
| Region Dummies         | Sales performance differs across regions compared to the reference region. |
| Store Type Dummies     | Some store formats perform differently than the reference store type.      |

---

## 4. Explanation of Dummy Variables

Dummy variables were created to convert categorical variables into numeric form.

### Region Dummy Variables

* Region_North = 1 if store belongs to North region, otherwise 0.
* Region_South = 1 if store belongs to South region, otherwise 0.
* Region_West = 1 if store belongs to West region, otherwise 0.

### Store Type Dummy Variables

* Store_HighStreet = 1 if the store is High Street, otherwise 0.
* Store_Residential = 1 if the store is Residential, otherwise 0.

---

## 5. Reference Categories Used

To avoid the dummy variable trap, one category from each categorical variable was excluded.

| Variable   | Reference Category |
| ---------- | ------------------ |
| Region     | East               |
| Store Type | Mall               |

All dummy coefficients are interpreted relative to these reference categories.

---

## 6. Final Model Selected

The **Multiple Regression Model** was selected as the final model.

---

## 7. Reason for Selecting the Final Model

The multiple regression model was chosen because:

* It achieved a higher R² value than the simple regression model.
* It considers multiple business factors simultaneously.
* It provides more comprehensive insights for decision-making.
* It offers better predictive accuracy for monthly sales.

Therefore, the multiple regression model is more suitable for supporting business decisions related to marketing, staffing, inventory management, and regional planning.
