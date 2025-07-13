# NASA-CMAPSS-RUL-Prediction
RUL prediction using BiLSTM on NASA C-MAPSS FD001 dataset

# NASA-CMAPSS-RUL-Prediction

This project predicts the **Remaining Useful Life (RUL)** of aircraft engines using a Bidirectional LSTM model on the  ASA C-MAPSS FD001 dataset.


 Features

1. BiLSTM-based deep learning model
2. Sliding window time-series approach
3. Robust training using Huber Loss
4. GroupKFold cross-validation by engine ID
5. Final model achieves **MAE < 10 cycles**

 Final Result

Final MAE : 9.77 cycles  
Test Set: FD001 subset of NASA C-MAPSS dataset

 Model Architecture

1.Bidirectional LSTM (128 → 64)
2.Dropout & BatchNormalization layers
3.Dense layers with ReLU activation
4.Huber Loss + Adam Optimizer
5.EarlyStopping and ReduceLROnPlateau callbacks

 Dataset

Source: NASA C-MAPSS Dataset (FD001)
Files Used:
1.`train_FD001.txt` – Engine sensor data until failure
2.`test_FD001.txt` – Partial engine run data
3.`RUL_FD001.txt` – Ground-truth remaining life

 Libraries Used

* Python 3.x
* TensorFlow / Keras
* Scikit-learn
* Pandas & NumPy
* Matplotlib

 How to Run

1. Clone this repository
2. Open and run `NASA-CMAPSS-RUL-Prediction.ipynb` using Jupyter or Google Colab
3. Download or provide access to:
   * `train_FD001.txt`
   * `test_FD001.txt`
   * `RUL_FD001.txt`
4. View final MAE and prediction visualizations

 Author

Yarlagadda Ramakrishna 

