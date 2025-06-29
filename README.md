Lasso Regression-Based Hedging Strategy for Portfolio Risk Management

## Introduction
- This project implements a Lasso Regression-based model to construct hedging strategies for financial portfolios.
- The goal is to minimize portfolio risk by identifying the most relevant assets from historical return data.

## Motivation
- Traditional hedging methods often lead to overfitting or non-interpretable models.
- Lasso regression introduces sparsity, reducing model complexity and improving robustness.
- This project uses real-world-like data to simulate practical hedging applications.

## Objective
- Build an interpretable, automated hedging model using Lasso Regression.
- Use historical stock returns to estimate hedge ratios that reduce portfolio variance.
- Ensure selected hedge positions are sparse and economically intuitive.

## Technologies Used
- Programming Language: Python
- Libraries: pandas, numpy, matplotlib, scikit-learn
- Platform: Jupyter Notebook

## Repository Contents
- Portfolio_Hedging.ipynb : Jupyter Notebook with all code and analysis
- stocks_returns.csv : Historical return data of stocks
- portfolio_metadata.csv : Metadata and P&L data for selected portfolios
- README.md : Project overview and documentation

## Methodology
- Loaded and cleaned stock return and portfolio data
- Merged datasets based on common dates and aligned for modeling
- Built Lasso regression models using scikit-learn to predict portfolio returns
- Tuned alpha (regularization parameter) to control sparsity
- Visualized coefficient paths, residuals, and hedging impact

## Key Results
- Sparse hedge portfolios with 5 to 10 selected assets out of a large universe
- Average R² score of approximately 0.76 on validation data
- Significant reduction in portfolio variance post-hedge
- Clear interpretability of selected hedge assets and their contributions

## Visualizations
- Coefficient paths showing shrinkage under increasing regularization
- Bar charts of final selected hedge weights
- Residual plots to demonstrate variance reduction and model fit

## Future Scope
- Extend to ElasticNet regression for better regularization control
- Incorporate rolling-window dynamic hedge estimation
- Include transaction cost modeling and real-time backtesting
- Deploy using Streamlit or Dash for interactive visualization

## Learnings
- Lasso regression effectively filters out noise and identifies dominant hedging instruments
- Regularization improves generalization in financial models
- Sparse models are interpretable and easier to operationalize in real-world trading

## Contact
- Pranay Saini
- Third Year Undergraduate, Department of Civil Engineering, IIT Kanpur
- Email: pranays23@iitk.ac.in
- LinkedIn: linkedin.com/in/pranay-saini-39bb76286

## License
- This project is released under the MIT License


