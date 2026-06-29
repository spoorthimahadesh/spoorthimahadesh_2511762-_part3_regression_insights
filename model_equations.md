# Dummy Variable Creation

Categorical variables `region` and `store_type` were converted into dummy variables to enable their use in regression analysis.

For the `region` variable, **East** was selected as the reference category. Three dummy variables were created: `Region_North`, `Region_South`, and `Region_West`.

For the `store_type` variable, **Mall** was selected as the reference category. Two dummy variables were created: `Store_HighStreet` and `Store_Residential`.

Reference categories were excluded from the regression model to avoid multicollinearity and the dummy variable trap.
