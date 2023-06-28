# Text-to-Speech Python Script

This is a Python script that utilizes the Eleven Labs Text-to-Speech API to convert text into speech. It prompts the user for an API key, text input, and voice selection, and then generates an audio file with the speech output.

## Prerequisites

To use this script, you need to have the following:

- Python installed on your system (version 3 or above).
- An API key from Eleven Labs Text-to-Speech API. If you don't have an API key, you can sign up for an account at [Eleven Labs](https://www.elevenlabs.io) and obtain one.

## Setup

1. Clone or download the repository from GitHub.
2. Make sure you have the `json` and `http.client` libraries installed. You can install them using pip:

   `pip install json http.client`

3. Place the script file in your desired directory.

## Usage

1. Open a terminal or command prompt and navigate to the directory where the script is located.

2. Run the script using the following command:

   `python main.py`

3. The script will prompt you to enter your API key. If you haven't entered it before, provide the key and press Enter. If you have already saved the key in a file named `api_key.txt`, the script will load it automatically.

4. Enter the text you want to convert to speech when prompted.

5. The script will display the available voices. Enter the number corresponding to the desired voice and press Enter.

6. The script will send a request to the API and generate the speech. If the request is successful, the audio file will be saved as `output.mp3` in the same directory.

7. Once the speech generation is complete, the script will display a success message or an error message if there was a problem with the request.

## Customization

### Adding/Modifying Voices

You can add or modify the available voices in the `voices` list defined in the script. Each voice object should have a `voice_id` and a `name` attribute. You can obtain the `voice_id` from the Eleven Labs Text-to-Speech API.

### Adjusting Voice Settings

If you want to customize the voice settings, you can modify the `payload` dictionary in the `generate_speech` function. The `stability` and `similarity_boost` settings can be adjusted to control the speech output.

## Contributing

If you find any issues or have suggestions for improvements, please feel free to create an issue or submit a pull request on the GitHub repository.

## License

This project is licensed under the [MIT License](LICENSE).
