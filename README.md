# Real-Time Sign Language Interpreter using LSTM

This project is a real-time sign language interpreter that uses a Long Short-Term Memory (LSTM) model to recognize and translate hand gestures into text and audio. Designed to aid communication for deaf and mute individuals, the interpreter converts sign language into spoken language, making communication more accessible.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Technologies Used](#technologies-used)
3. [Features](#features)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Dataset](#dataset)
7. [Model Training](#model-training)
8. [Accuracy and Results](#accuracy-and-results)
9. [Contributing](#contributing)
10. [License](#license)

## Project Overview

The Real-Time Sign Language Interpreter uses an LSTM model to recognize various sign language gestures. The system captures video frames, processes them through a trained LSTM model, and translates the gestures into readable text and audio output. Deployed using the Flask framework, the application allows users to interact with the model in real-time, achieving a 94% accuracy rate in recognizing gestures.

## Technologies Used

- **Python**
- **Flask Framework** for the web application
- **Long Short-Term Memory (LSTM)** model for gesture recognition
- **SQLite** for data storage
- **HTML, CSS** for frontend design

## Features

- **Real-Time Gesture Recognition**: Captures and processes sign language gestures in real-time.
- **Text and Audio Translation**: Converts gestures into text and audio output for ease of communication.
- **High Accuracy**: Achieves a 94% accuracy rate in recognizing sign language gestures.
- **User-Friendly Interface**: Simple web interface for easy interaction.

## Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/real-time-sign-language-interpreter.git
   cd real-time-sign-language-interpreter
   ```

2. **Install Dependencies**
   Ensure you have Python 3.x installed. Install the necessary dependencies by running:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up SQLite Database**
   Initialize the SQLite database by running the setup script (if provided) or use the existing database.

4. **Run the Application**
   Start the Flask server by executing:
   ```bash
   python app.py
   ```

5. **Access the Application**
   Open your browser and navigate to `http://127.0.0.1:5000` to interact with the application.

## Usage

1. Launch the application and access it through the provided local URL.
2. Use a webcam or connect a camera to capture sign language gestures in real-time.
3. The application will process each gesture and display the translated text.
4. The output will also be converted to audio for convenient communication.

## Dataset

The model is trained on a custom dataset of sign language gestures. If you wish to use a different dataset, make sure it includes labeled images or sequences of the gestures you want to recognize.

## Model Training

The LSTM model is trained on a sequence of sign language gesture images. For more information on training, you may review the `train_model.py` file in this repository. To train the model on a new dataset:

1. Prepare the dataset with labeled gesture sequences.
2. Run the training script:
   ```bash
   python train_model.py
   ```
3. After training, save the model weights and integrate them into the application.

## Accuracy and Results

The model achieves a **94% accuracy** in recognizing common sign language gestures. For more detailed metrics and performance analysis, refer to the evaluation script provided.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with detailed explanations of any changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
