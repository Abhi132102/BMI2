# Body Mass Index Calculator

This project is a simple web application to calculate Body Mass Index (BMI) using Flask for the backend and HTML/CSS for the frontend.

## Project Structure

- `app.py`: The main Flask application file.
- `index.html`: The HTML template for the BMI calculator.
- `requirements.txt`: Python dependencies required for the project.

## Features

- Accepts user input for weight (in kg) and height (in cm).
- Validates the user input to ensure it is numeric.
- Calculates BMI based on the provided weight and height.
- Displays the calculated BMI and the corresponding weight status.

## Setup Instructions

### Prerequisites

Ensure you have Python and pip installed. You can download Python from [here](https://www.python.org/downloads/).

### Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/bmi-calculator.git
    cd bmi-calculator
    ```

2. **Create a virtual environment and activate it:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3. **Install the dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4. **Run the application:**
    ```bash
    python app.py
    ```

5. **Open your web browser and go to:**
    ```
    http://127.0.0.1:5000
    ```

## Deployment on Vercel

To deploy this Flask application on Vercel, follow these steps:

1. **Install Vercel CLI:**
    ```bash
    npm install -g vercel
    ```

2. **Create `vercel.json` configuration file:**

    ```json
    {
      "version": 2,
      "builds": [
        {
          "src": "app.py",
          "use": "@vercel/python"
        }
      ],
      "routes": [
        {
          "src": "/(.*)",
          "dest": "app.py"
        }
      ]
    }
    ```

3. **Deploy the application:**
    ```bash
    vercel
    ```

## Usage

1. **Open the application in your web browser.**
2. **Enter your weight (in kg) and height (in cm).**
3. **Click on the "Calculate" button.**
4. **The calculated BMI and weight status will be displayed.**

## Example

![BMI Calculator]("C:\Users\vasam\OneDrive\Pictures\Screenshots\Screenshot 2024-07-07 144451.png")

## Contributing

Feel free to fork this repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
