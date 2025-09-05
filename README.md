# CognitiveRadio-LSTM
## Prediction of Channel States Using an LSTM (Long Short-Term Memory) Model  
Using PyTorch technology, we simulate multiple frequency channels as well as their availability over time. We use an LSTM model that we train on the simulation of one spectrum and make predictions about the future states of the spectrum based on its previous states.

The work consists of the following parts:
- Import the necessary libraries  
- Simulate the spectrum and its state over time using the `simulate_multiple_channels` function  
- Prepare/process the data into a format suitable for LSTM model input  
- Define the LSTM model  
- Prepare the DataLoader and training data  
- Training loop – train the model on the simulated data  
- Randomly select a part of the previously simulated data and predict the future state of the channel using the LSTM model  
- Check the model’s accuracy  
- Compare the real channel states with the predicted states  

