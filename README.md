# ODI Win Predictor

## Project Overview

The ODI Win Predictor is a web application developed using Streamlit that predicts the winning probability of an ongoing One Day International (ODI) cricket match. It takes into account various factors such as the batting and bowling teams, match location (city), current score, overs completed, wickets lost, and the match target. Using these inputs, it provides the percentage probabilities for the batting and bowling teams to win.

This project leverages a machine learning model trained with historical cricket match data to compute the winning probability. The user-friendly interface allows cricket fans and analysts to quickly assess the chances of a team winning based on live match conditions.

## Features

- **Team Selection:** Choose the batting and bowling teams from a list of international cricket teams.
- **City Selection:** Select the city where the match is being played, as location can influence match dynamics.
- **Target Input:** Input the target score the batting team needs to chase.
- **Live Match Data:** Enter live match details such as the current score, overs completed, and wickets lost.
- **Winning Probability Prediction:** Get the predicted win probability of both the batting and bowling teams based on current match conditions.

## Requirements

- Python 3.x
- Libraries:
  - `streamlit`: To run the web application.
  - `joblib`: To load the machine learning model.
  - `pandas`: For data manipulation.
  
You can install these dependencies by running:
```bash
pip install streamlit joblib pandas
```

## Files

- **`pipe.joblib`:** This is the machine learning model file, serialized using the `joblib` library. It contains a pre-trained model that predicts the probabilities of each team's win.
- **`app.py`:** The main Streamlit app file that contains the code to run the front-end interface and handle the input/output logic.

## How to Run the Application

1. Clone the repository or download the project files.
2. Ensure all dependencies are installed by running `pip install -r requirements.txt`.
3. Place the machine learning model (`pipe.joblib`) in the project directory.
4. Run the Streamlit app by executing:
   ```bash
   streamlit run app.py
   ```
5. Open the web application in your browser at the local URL displayed in the terminal (typically `http://localhost:8501`).

## Application Walkthrough

1. **Team Selection:** Use the dropdown menus to select the batting and bowling teams.
2. **City Selection:** Choose the city where the match is being played from a predefined list of cities.
3. **Target Score:** Enter the target score that the batting team is aiming to achieve.
4. **Current Match Details:**
   - Input the current score of the batting team.
   - Enter the number of overs completed.
   - Enter the number of wickets that have fallen.
5. **Predict:** Press the "Predict Probability" button to get the win probability for the batting and bowling teams.
6. **Prediction Result:** The app will display the winning chances for both teams as percentages.

## Example

- Batting Team: India
- Bowling Team: Australia
- City: Melbourne
- Target: 300
- Current Score: 150
- Overs Completed: 30
- Wickets Lost: 5

Pressing the "Predict Probability" button will provide the predicted win/loss percentages for both teams based on the above inputs.

## Conclusion

The ODI Win Predictor is an exciting tool for cricket fans to simulate and predict match outcomes using machine learning. It offers real-time insights into the probable result of an ODI match based on key match statistics. Feel free to experiment with different inputs to see how the dynamics of the game change!