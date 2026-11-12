           Weather Temperature Prediction Using SimpleRNN

##Project Overview


This project uses a Simple Recurrent Neural Network (SimpleRNN) to predict the next day's 

average temperature based on previous weather data.


The model uses the past 7 days of temperature, humidity, and wind speed data to predict 

temperature.



##Dataset



File name: weather_daily.csv



Selected city: Thiruvananthapuram



Input features:



 .Average Temperature



  .Relative Humidity



  .Maximum Wind Speed



Target: Next day's Average Temperature



##Technologies Used



.Python



.Pandas



.NumPy



.Matplotlib



.Scikit-learn



.TensorFlow / Keras



.Jupyter Notebook



##Project Workflow



1.Loaded and explored the weather dataset.



2.Checked missing values.



3.Selected Thiruvananthapuram city data.



4.Sorted data by date.



5.Applied MinMaxScaler for data normalization.



6.Created 7-day input sequences.



7.Split the data into training, validation, and testing sets.



8.Built a SimpleRNN model with 64 units.



9.Added Dropout and Dense layers.



10.Trained the model for 50 epochs.



11.Evaluated model performance.



12.Forecasted the next 7 days' temperature.



##Model Architecture



.Input Layer: 7 time steps, 3 features



.SimpleRNN: 64 units



.Dropout: 0.2



.Dense: 1 output neuron



##Model Performance



#Evaluation Metric



RMSE   0.5423 °C



MAE   0.4256 °C



R² Score  0.6958



##Next 7 Days Temperature Forecast



The model generated temperature predictions for the next 7 days.



.Day 1: 26.75 °C



.Day 2: 26.79 °C



.Day 3: 26.80 °C



.Day 4: 26.74 °C



.Day 5: 26.72 °C



.Day 6: 26.76 °C



.Day 7: 26.75 °C



Note: Future humidity and wind speed values were assumed to remain at their last observed values for forecasting.




##Conclusion



The SimpleRNN model was successfully developed and trained to predict daily average temperature using historical weather data. The model achieved an RMSE of 0.5423 °C, an MAE of 0.4256 °C, and an R² score of 0.6958.



This project demonstrates how Recurrent Neural Networks can be used for time-series weather forecasting.



#How to Run



1.Install the required Python libraries.



2.Place weather_daily.csv in the notebook folder.



3.Open the Jupyter Notebook.



4.Run all cells in sequence.



#nstall Libraries



pip install pandas numpy matplotlib scikit-learn tensorflow