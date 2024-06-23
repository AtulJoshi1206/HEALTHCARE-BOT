# HEALTHCARE-BOT
# HealthCare ChatBot

This repository contains the code for a HealthCare ChatBot application built using Python and the Tkinter library. The bot interacts with users to gather information about their symptoms and provides potential diagnoses along with descriptions and precautions.

## Features
- **Graphical User Interface (GUI)**: An interactive and user-friendly experience built with Tkinter.
- **Blurred Background**: An aesthetic blurred background image.
- **Symptom Checking**: Input symptoms and get related symptoms for further clarification.
- **Disease Prediction**: Predicts possible diseases based on provided symptoms.
- **Precautionary Measures**: Offers precautionary measures for the predicted diseases.

## Prerequisites

Ensure you have the following libraries installed:
- `tkinter`
- `PIL` (Pillow)
- `pandas`
- `scikit-learn`

Install the required libraries using pip:
```sh
pip install pillow pandas scikit-learn
```

## Usage

### Running the ChatBot

1. **Clone the repository:**
    ```sh
    git clone https://github.com/yourusername/HealthCareChatBot.git
    cd HealthCareChatBot
    ```

2. **Place your background image:**
    Ensure you have an image named `health.png` in the same directory as the script.

3. **Run the script:**
    ```sh
    python chatbot.py
    ```

### Interacting with the Bot

- **Initial Greeting**: The bot greets you and asks for your name.
- **Symptom Input**: Enter the symptom you are experiencing.
- **Symptom Confirmation**: The bot provides related symptoms to confirm your input.
- **Symptom Duration**: Provide the number of days you have been experiencing the symptom.
- **Related Symptoms**: The bot asks if you are experiencing other related symptoms.
- **Result Display**: The bot displays the predicted disease, description, and precautions.

### Sample GUI Screenshot
![HealthCare ChatBot GUI](screenshot.png)

## Code Overview

### Main Components

1. **Class Definition**: The `HealthCareChatBot` class initializes the main window with a blurred background image.
2. **Message Display**: The `display_message` function displays messages in the chat area with different formatting for bot and user messages.
3. **Message Handling**: The `send_message` and `send_message_from_button` functions handle sending messages when the user presses Enter or the Send button.
4. **Process Message**: The `process_message` function processes user input and advances the conversation stage by stage.
5. **Symptom Handling**: Functions like `get_related_symptoms`, `ask_next_symptom`, and `show_results` handle symptom input, related symptom queries, and displaying results.

### Prediction Integration

- **Predict Module**: The script relies on a `predict` module that contains functions for pattern checking (`check_pattern`), secondary prediction (`sec_predict`), getting disease descriptions (`get_disease_description`), getting precautions (`get_precautions`), and calculating condition (`calc_condition`).

## Customization

### Background Image

Change the background image by replacing `health.png` with any image of your choice.

### Number of Symptoms

Adjust the maximum number of symptoms to query by changing the `self.max_symptoms` attribute.

## Contributions

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to customize the README further to better fit your specific needs and style.
