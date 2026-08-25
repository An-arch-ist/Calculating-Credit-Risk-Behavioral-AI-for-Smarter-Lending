# Calculating-Credit-Risk-Behavioral-AI-for-Smarter-Lending
💳 Transaction-Augmented Credit Risk: From Borrower Profiles to Behavioral Alpha

This project develops a machine-learning credit risk framework integrating traditional borrower/loan information with high-frequency transaction behavior. Using 58,645 unique borrowers and 231,735 transaction records, the analysis engineered 20 features from 11 static application variables and 9 behavioral indicators, including transaction volume, volatility, frequency, geographic diversity and spending intensity. A Random Forest classifier with stratified 80:20 validation achieved 95.11% accuracy, 0.9323 ROC-AUC and 0.8052 F1-score.

Beyond prediction, the project investigates whether behavioral data provides incremental risk information and uncovers several economically meaningful patterns. The Transaction Volatility Coefficient (TVC) revealed a 120.76% behavioral polarity shift between defaulters and non-defaulters, while Intraday Spending Velocity showed that defaulters' spending accelerated 9.36% faster throughout the day.

The analysis further identified housing ownership as a major structural risk moderator: renters were 16.2× more likely to default than homeowners despite only a 2.8% difference in average spending volatility. For borrowers with DTI above 0.30, default rates were 95.7% for renters versus 4.9% for homeowners, creating a 90.8-percentage-point risk gap. Logistic regression reinforced the finding, with renters showing an adjusted odds ratio of 30.49 (p < 0.001) after controlling for income, age and employment length.

The project also tested 5-fold stratified cross-validation, producing a mean ROC-AUC of 0.9247 with only ±0.42% variation, and a 20% Gaussian-noise stress test reduced AUC by just 0.007, demonstrating strong model stability and robustness.

Key outcome: rather than simply adding more data to improve prediction, the project demonstrates how behavioral analytics can reveal hidden risk dynamics and inform credit-policy design, culminating in a housing-adjusted DTI framework: a 0.30 cap for renters and 0.45 for homeowners
