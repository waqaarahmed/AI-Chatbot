
# Basic Rule-Based Chatbot with TensorFlow

This project demonstrates how to build a basic rule-based chatbot using TensorFlow, NLTK, and other Python libraries. The chatbot is trained on a simple set of intents and responses defined in a JSON file. The trained model can then predict the appropriate response to a user's input.

## Project Structure

- **train.py**: This script is used to train the neural network model using the intents defined in `intents.json`. It preprocesses the data, tokenizes the patterns, and trains a model that is saved as `chatbot_model.h5`.
- **chatbot.py**: This script loads the trained model and handles user input. It predicts the appropriate response based on the input and the model's predictions.
- **intents.json**: A JSON file that contains predefined intents. Each intent includes possible user inputs (patterns) and corresponding bot responses.

## Requirements

To run this project, you'll need to have the following Python packages installed:

- tensorflow
- numpy
- nltk

You can install the necessary packages using pip:

```bash
pip install tensorflow numpy nltk
```

## How to Use

### 1. Train the Model

Run the `train.py` script to preprocess the data and train the model:

```bash
python train.py
```

This will create the `chatbot_model.h5`, `words.pkl`, and `classes.pkl` files, which are required for the chatbot to function.

### 2. Start the Chatbot

Run the `chatbot.py` script to start the chatbot:

```bash
python chatbot.py
```

The chatbot will wait for user input in the console. Simply type your message and hit enter to receive a response.

### 3. Customize Intents

You can customize the bot's behavior by modifying the `intents.json` file. Add new intents, patterns, and responses as needed.

## Example Intents

Here are a few examples of intents defined in `intents.json`:

- **greetings**: Handles greetings like "Hello", "Hi", etc.
- **goodBye**: Handles farewells like "Bye", "See you later", etc.
- **age**: Handles questions about the bot's age.
- **name**: Handles questions about the bot's name.
- **shop**: Handles inquiries about available products.
- **hours**: Handles questions about operating hours.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
