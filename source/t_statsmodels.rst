
Stats with statsmodels
=========================

`statsmodels` is the go-to library for doing econometrics (linear regression, logit regression, etc.). 

You can find a `good tutorial here <http://nbviewer.ipython.org/urls/s3.amazonaws.com/datarobotblog/notebooks/multiple_regression_in_python.ipynb>`_.

The most important things are also covered on `the statsmodel page here <http://statsmodels.sourceforge.net/devel/>`_, especially the pages on OLS `here <http://statsmodels.sourceforge.net/devel/example_formulas.html>`_ and `here <http://statsmodels.sourceforge.net/devel/examples/notebooks/generated/ols.html>`_.

(If you want to do machine learning, by the way, the library is `scikit-learn <http://scikit-learn.org/stable/>`_.)

Here are some simple illustrative examples of standard OLS:

On with the show:

.. ipython:: python

   @suppress   
   import os
   @suppress
   os.chdir("source/_data")

   # Load pandas and statsmodels
   import pandas as pd
   import statsmodels.formula.api as smf
   
   # Load a csv dataset of World Development Indicators
   my_data = pd.read_csv('wdi_indicators.csv')

   # Look at first three lines
   my_data.head(3)
               
   # OLS
   results = smf.ols('life_expectancy ~ population_density + gdp_per_cap',
                     data=my_data).fit()
   print(results.summary())
     

   # Categorical Vars are easy
      # Make categorical var
   my_data['low_income'] = my_data['gdp_per_cap'] < 4000

   results2 = smf.ols('life_expectancy ~ population_density + gdp_per_cap + C(low_income)', data=my_data).fit()

   print(results2.summary())
   

   # Heteroskedastic-Robust Standard Errors
   results2_robust = results2.get_robustcov_results()
   print(results2_robust.summary())
   
   
   # Output to LaTeX
   latex = results2_robust.summary().as_latex()
   latex
   
   # Save to disk
   with open("regression_table.tex", "w") as text_file:
       text_file.write(latex)
   
   

   