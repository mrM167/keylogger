# keylogger
my name is Martin Monageng my repository is a simple python based keylogger

Simple Python Keylogger
This repository contains a basic Python script that functions as a simple keylogger. It records keyboard inputs and saves them to a local file, while also printing them to the console. This tool is primarily intended for educational purposes, for understanding how keylogging works, or for personal use (e.g., monitoring your own typing for productivity analysis).

Disclaimer: This tool should only be used on systems you own and have explicit permission to monitor. Unauthorized keylogging is illegal and unethical.

Features
Captures individual key presses.

Logs regular characters and handles some special keys (e.g., Space, Backspace).

Saves all logged keys to a text file (log.txt).

Prints logged keys to the console in real-time.

Simple and lightweight, using the pynput library.

Prerequisites
Before running this script, ensure you have Python installed on your system. This script has been tested with Python 3.x.

You will also need the pynput library. You can install it using pip:

pip install pynput

How It Works
The simplekeylogger class uses the pynput.keyboard.Listener to monitor keyboard events.

When a key is pressed, the evaluate_key method is called.

evaluate_key determines if the pressed key is a regular character or a special key (like space or backspace) and converts it into a string.

This string representation of the key is then passed to the append_to_log method.

append_to_log writes the key string to log.txt and also prints it to the console.

The start method initializes and runs the keyboard listener, keeping the script active and monitoring inputs.

Setup and Usage
Follow these steps to set up and run the keylogger:

Clone the Repository (or download the script):
If you have Git installed, you can clone this repository:

git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name # Navigate into the cloned directory

Alternatively, you can just download the keylogger.py file directly.

Install Dependencies:
Make sure you have pynput installed:

pip install pynput

Run the Keylogger:
Execute the script from your terminal or command prompt:

python keylogger.py

Monitor Output:

The script will start listening for key presses.

Any key you type while the script is running will be printed to your console.

All logged keys will also be saved in a file named log.txt in the same directory as the script.

Stop the Keylogger:
To stop the keylogger, go back to the terminal where the script is running and press Ctrl + C.

Log File (log.txt)
The log.txt file will be created automatically in the directory where you run the keylogger.py script. Each key press will be appended to this file. Special keys like "space" or "backspace" will be represented as their string equivalents.

Important Considerations
Security & Ethics: This script is for educational and personal use only. Using it to monitor others without their explicit consent is illegal and unethical. Always ensure you have the necessary permissions before deploying any keylogging software.

Antivirus Software: Due to its nature, antivirus software might flag this script as malicious. This is a common behavior for tools that interact with keyboard inputs. You might need to add an exception in your antivirus settings if you intend to use it for legitimate purposes on your own system.

Persistence: This script does not include any mechanisms for persistence (e.g., starting automatically on boot). It needs to be manually run each time.

Error Handling: The script includes basic error handling for file operations. More advanced error handling (e.g., for pynput specific issues) could be added for a production-ready application.

Special Keys: The current implementation handles space and backspace. You could extend the evaluate_key method to handle other special keys (e.g., Enter, Shift, Ctrl, arrow keys) more explicitly for a more detailed log.

Contributing
If you'd like to improve this simple keylogger (e.g., add more robust special key handling, better error logging, or a GUI), feel free to fork this repository and submit pull requests.
Kindly bear in mind that the EXE file also comes with a RAR which required decompression before it<3.
