# Temperature-Forecasting-Using-Deep-Learning-on-Time-Series-Weather-Data
To predict future temperature values based on previous weather conditions using deep learning models — specifically, LSTM and GRU — which are well-suited for time series forecasting tasks.
📁 Dataset Overview:

The dataset consists of over 420,000 rows of weather data collected at 10-minute intervals, with 15 features. It includes important atmospheric variables such as:

    Temperature

    Air Pressure

    Relative Humidity

    Dew Point

    Wind Velocity and Direction

    Vapor Pressure components

    Air Density and Water Content

The dataset is complete with no missing or duplicate values, making it well-suited for modeling.
🎯 Project Goal:

To predict future temperature values based on previous weather conditions using deep learning models — specifically, LSTM and GRU — which are well-suited for time series forecasting tasks.
🧪 Data Preparation:

    The original feature names were cleaned and simplified for ease of use.

    Data normalization was applied using MinMaxScaler, scaling all feature values to a range between 0 and 1.

    Time series sequences were created using a sliding window of 24 time steps, meaning the model learns from the last 24 recorded measurements to predict the next temperature.

🧠 Model Architecture:

Two deep learning approaches were tested:

    LSTM (Long Short-Term Memory) — ideal for learning long-term dependencies in time series data.

    GRU (Gated Recurrent Unit) — a faster, more efficient alternative to LSTM with similar predictive performance.

Each model consisted of:

    A recurrent layer (LSTM or GRU) with 64 units

    A dropout layer to prevent overfitting

    A dense output layer for predicting one continuous value (temperature)

🏋️ Model Training:

    The data was split into training and testing sets (80%/20%)

    The models were trained for multiple epochs using a batch size of 64

    A portion of the training data was used for validation to monitor the model's generalization

📊 Evaluation:

The models were evaluated using:

📊 RMSE: 0.32
📊 MAE: 0.21
   

These low error values indicate high prediction accuracy, with an average prediction error of less than half a degree Celsius — excellent performance for weather forecasting.
📈 Results Visualization:

Actual vs. Predicted temperatures were plotted, showing a close match between the two — confirming the model’s effectiveness in capturing temperature patterns over time.
✅ Conclusion:

The project successfully demonstrates how deep learning models like LSTM and GRU can be applied to weather time series data to forecast temperature with high accuracy. This approach can be extended to other meteorological variables and longer forecasting horizons.
