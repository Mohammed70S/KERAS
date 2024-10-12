
**Orbital Position Prediction using Neural Network**

## **Objective**
The objective of this project is to predict the orbital position of an object over time using a Neural Network implemented with Keras. By leveraging time steps as the input and orbital position as the output, the model learns to map the relationship between the two through a series of hidden layers.

## **Dataset Description**
The dataset, named `orbit.xlsx`, consists of two main features:
- **time_steps**: The time step of the orbital simulation.
- **y**: The corresponding orbital position at each time step.

The dataset is normalized using `MinMaxScaler` to scale the values of both features between 0 and 1, improving the model's performance and training efficiency. The dataset is split into training and validation sets, with 80% of the data used for training and 20% used for validation.

## **Steps to Run the Code in Google Colab**

### Step 1: Upload your dataset
- Upload the `orbit.xlsx` file to your Google Drive or Colab environment.

### Step 2: Install Dependencies
In Google Colab, Keras, pandas, scikit-learn, and Matplotlib are pre-installed. However, if you're running this code locally, you can install the necessary libraries using:
```bash
!pip install keras pandas scikit-learn matplotlib openpyxl
```

### Step 3: Clone or Download the Repository
Clone the repository containing the code or download it as a ZIP file:
```bash
git clone <repository-url>
```

### Step 4: Upload the code and dataset to Colab
Upload the code file and dataset into your Colab workspace or link your Google Drive where the dataset is stored.

### Step 5: Run the code
1. Load the dataset and check for any missing values.
2. Normalize the `time_steps` and `y` columns using `MinMaxScaler`.
3. Split the dataset into training and validation sets using an 80/20 split.
4. Define a neural network model using Keras with two hidden layers.
5. Train the model on the training set and evaluate it on the validation set using Mean Squared Error (MSE), Mean Absolute Error (MAE), and R-squared metrics.
6. Visualize the actual vs predicted orbital positions using a scatter plot.

### Step 6: Save and Download Results
The plot of actual vs predicted orbital positions will be saved as `_actual_vs_predicted.png`. You can download this file for further analysis.

## **Dependencies and Installation Instructions**
- **Keras**: For building and training the neural network
- **Pandas**: For data manipulation and loading the dataset
- **scikit-learn**: For data preprocessing (normalization and train-test split)
- **Matplotlib**: For visualization
- **OpenPyXL**: For reading `.xlsx` files (required by pandas)

Install the necessary libraries using:
```bash
pip install keras pandas scikit-learn matplotlib openpyxl
```

### **Python Version**
- Ensure Python version 3.x is installed.

### **Colab Environment**
- If running in Google Colab, the necessary dependencies will already be installed. Simply upload your dataset and run the code cells step-by-step.

