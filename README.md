## Climate Change with ClimateWins - Part 2

#### Project Overview

ClimateWins, a fictitious non-profit organization, seeks to apply machine learning (ML) to predict the consequences of climate change in Europe and beyond. It is concerned with the acceleration of extreme weather events in recent decades, believing that such fat-tailed risk can be viably modeled and predicted with ML.

#### Scope

Timeframe: *Jan 1960 - Oct 2022*

European Weather Stations: *Basel, Oslo, Stockholm, Budapest, Debilt, Dusseldorf, MunchenB, Madrid, Belgrade, Ljubljana, Heathrow, Maastricht, Kassel, Valentia and Sonnblick.*

Omitted (from project second half analysis): Roma, Gdansk, Tours.

#### Project Objectives

For the final report:

•	Identify European weather patterns outside the regional norm

•	Determine if unusual weather patterns are increasing

•	Generate future weather scenarios (25-50 years) based on past trends

•	Project the safe habitable zones in Europe over the next 25-50 years

#### Data Sources

Weather data: European Climate Assessment & Dataset project

Pleasant Weather answers dataset: Origin not disclosed to the author.  (Red flag.)

#### Tools

•	Languages & Libraries: Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Plotly, Operator, Os, Tensorflow, Keras, Graphviz, Statsmodels, Datetime, Pylab, Mpl_toolkits)

•	Software: Jupyter Notebooks, Excel

#### Techniques Used

•	Data wrangled, merged, grouped, aggregated, summarized, subsetted, transformed (z-score normalization, 0-1 normalization, one-hot encoding of y labels, model-specific reshaping)

•	Time series data preprocessed, decomposed, stationarity-tested (ADF & KPSS tests, ACF plots), stationarized

•	Supervised & Unsupervised learning: KNN, DT, RF, ANN, CNN, GAN, RNN & LSTM models deployed for classification prediction exercises

•	Hyperparameter optimization via grid search, random search, Bayesian optimization, model fine-tuning & regularization to minimize overfit on training data

•	Data visualized in Python, varying types of plots

#### Attribution

OpenAI's ChatGPT, powered by GPT-4o, was enlisted for ML model customization, fine-tuning and regularization Python code and de-bugging; explanation of ML concepts, underlying math and methods; and for constructive criticism on model output.

#### Key Finding

To develop familiarity with supervised and unsupervised learning ML models (as above), concepts and methods, the majority of ClimateWins-required tasks centered on using historical weather data (1960-2022) to predict a daily 'Pleasant' or 'Unpleasant' weather outcome (label) at each of 15 weather stations in Europe. The "Black Box" labels (answers dataset) in the binary prediction (classification) exercises were of *undisclosed origin*.

However, the accidental discovery of 100% perfect label prediction accuracy on an imbalanced class by the Random Forests algorithm, led to an Occam's Razor explanation: the unknown-origin labels must have been created via deterministic rules and thresholds for key weather features.

The Random Forests algorithm excels at reverse-engineering such type of label.  Further LSTM model-based poking around using a timesteps=1 setting, which achieved 96-99% classification accuracy on five different metrics, revealed the likely use of same-day weather data to create each daily label outcome at a weather station.  If the labels were created as believed, then the model-specific evaluations can be limited to a specific use case (classifying deterministic rule and threshold-based labels).  Not more.

As per ClimateWins requirements, the final report presents three "thought experiments" linked to project objectives.  These experiments are translated into testable hypotheses, with potential models, methods and datasets to pursue.

#### Folders

•	01 Datasets: Original, processed and split data files.  Original weather data is in the "Dataset-weather-prediction-dataset-processed.xlsx" Excel file.  Pleasant/Unpleasant Weather answers data is in the "Dataset-Answers-Weather_Prediction_Pleasant_Weather.xlsx" Excel file of unknown provenance.

•	02 Scripts: Python scripts for sequential stages of the project's second half, differentiated by topics.

•	03 Project Management: Project Brief for project's second half, pdf format.

•	04 Final Report: Deliverable to the hypothetical non-profit management team, pdf format.



