# Email Standardizer

This Python application helps to convert emails into a standardized format in the style of a Tech Support operator by default, but you can modify this paramater in the menu button, using openai GPT-4 based deep learning model. This README will provide you an overview about how to setup and use the application.

## Prerequisites
Before starting with the setup, ensure the following prerequisites are met:
- Python3 installed. You can download it from [here](https://www.python.org/downloads/)
- Install required python modules using command: `pip install tkinter openai`
- An API Key from OpenAI. You can get it from [OpenAI's Website](https://beta.openai.com/signup/)

## Project Structure
- `email_standardizer.py` : Main python script where the GUI and processing functions are defined.
- `api_key.json` : JSON file which stores the API key for OpenAI. Make sure not to expose this file.

## Setup
In order to run the tool you need to follow the steps:

1. Clone the repository or download the repository as zip.
2. (Optional) If you have the OpenAI's API Key, create `api_key.json` file like:
```
{
    "api_key": "<api-key>"
}
```
Otherwise, the program will prompt you to enter it at first run.

3. Run `python3 email_standardizer.py` in the terminal from the project folder's location.

## Using the Application
After successful setup of the application, you'll see a GUI window with several text boxes, buttons and a menu.

- The large text field at the top is where you should paste the batch of emails needing standardization.
- The 'Process Email' button below the text field initiates standardization using the GPT-4 API.
- The bottom large text field displays the standardized version of the emails.
- The 'Copy to Clipboard' button copies the text shown in the result textbox to the clipboard.
- You can change the default processing parameters on 'Load Parameters' from Menu bar.

## License
This project is under MIT license. See the LICENSE.md file for more details.
