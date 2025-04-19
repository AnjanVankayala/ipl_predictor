# IPL Win Predictor

The **IPL Win Predictor** is a machine learning-based web application designed to predict the outcomes of IPL matches. By analyzing historical IPL match data, this project provides cricket enthusiasts and analysts with insights and predictions, enhancing their understanding and enjoyment of the game.

---

## Features

- **Interactive Web Application**: Built using [Streamlit](https://streamlit.io/), the app allows users to input match details and receive predictions in real-time.
- **Predictive Model**: Uses a machine learning model trained on IPL match data to forecast match outcomes.
- **User-Friendly Interface**: Select teams, host city, and match details to get win probabilities for both teams.

---

## Dataset

The dataset used for this project was obtained from Kaggle: [IPL Dataset](https://www.kaggle.com/datasets/ramjidoolla/ipl-data-set). It includes:
- `matches.csv`: Contains match-level data.
- `deliveries.csv`: Contains ball-by-ball data.

---

## Technologies Used

- **Python**: Core programming language.
- **Libraries**:
  - `pandas`: For data manipulation and analysis.
  - `scikit-learn`: For building and training the machine learning model.
  - `pickle`: For saving and loading the trained model.
  - `streamlit`: For creating the interactive web application.
  - `requests`: For handling external data loading (if needed).
- **Machine Learning**:
  - Logistic Regression model implemented using `scikit-learn`.

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/ipl-win-predictor.git
   cd ipl-win-predictor
2. Install the required dependencies:
```bash
   pip install -r requirements.txt
```
3.Run the application:
```bash
python -m streamlit run app.py
```
## Usage
- Open the application in your browser (Streamlit will provide a local URL).
-Input the following match details:
- `Batting Team`: Select the team currently batting.
- `Bowling Team`: Select the team currently bowling.
- `Host City`: Select the city where the match is being played.
- `Target Score`: Enter the target score set by the batting team.
- `Current Score`: Enter the current score of the batting team.
- `Overs Done`: Enter the number of overs completed.
- `Wickets Fallen`: Enter the number of wickets lost.
Click the Predict Probabilities button to get the win probabilities for both teams.

## Model Details
- `Training`:
The model was trained using historical IPL data.
Features include batting team, bowling team, city, current score, wickets fallen, remaining balls, target score, current run rate (CRR), and required run rate (RRR).
- `Output`:
The model predicts the probabilities of each team winning the match.

## Future Enhancements
- Add support for live match data integration.
- Improve the model by incorporating additional features like player performance and weather conditions.
- Deploy the application to a cloud platform for public access.

## Acknowledgments

- **Dataset**: The IPL dataset used in this project was sourced from [Kaggle IPL Dataset](https://www.kaggle.com/datasets/ramjidoolla/ipl-data-set). It includes match-level and ball-by-ball data for IPL matches.
- **Libraries**:
  - [Streamlit](https://streamlit.io/): Used to create the interactive web application.
  - [scikit-learn](https://scikit-learn.org/): Used for building and training the machine learning model.
  - [pandas](https://pandas.pydata.org/): Used for data manipulation and analysis.
  - [pickle](https://docs.python.org/3/library/pickle.html): Used for saving and loading the trained model.
- **Inspiration**: This project was inspired by the need to provide cricket enthusiasts and analysts with a tool to predict match outcomes and enhance their understanding of the game.



