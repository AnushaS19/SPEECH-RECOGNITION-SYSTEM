# SPEECH-RECOGNITION-SYSTEM
COMPANY : ``CODTECH IT SOLUTIONS

NAME : ANUSHA S

INTERN ID :CT04DH1155

DOMAIN : ARTIFICIAL INTELLIGENCE

DURATION : 4 WEEKS

MENTOR : NEELA SANTHOSH

DESCRIPTION : This project is a simple yet effective demonstration of a real-time speech-to-text converter with voice feedback, built using Python. It showcases the integration of speech recognition and text-to-speech (TTS) technologies to create an interactive voice-enabled application. The core idea is to allow the user to speak into a microphone, convert that speech into text, and then have the program read the recognized text back to the user in real time. This creates a loop where the user receives immediate audible feedback, making the application useful for both accessibility and educational purposes.

At the heart of the project are two powerful Python libraries: speech_recognition and pyttsx3. The speech_recognition library is used to process spoken audio and convert it into text using the Google Web Speech API, which is known for its high accuracy in recognizing natural language. This API is cloud-based, meaning it requires an active internet connection. On the other hand, pyttsx3 is an offline text-to-speech engine that enables the program to speak out the recognized text without needing an internet connection. It supports different voices, speech rates, and volume settings, making it flexible for various user needs.

The flow of the application is straightforward. It starts by initializing a recognizer object (r) using the speech_recognition module. Inside a while True loop, the program continuously listens for audio input from the default system microphone. Before recording audio, the program performs ambient noise adjustment using r.adjust_for_ambient_noise(), which helps in reducing background noise interference and improves transcription accuracy. The audio is then captured using the r.listen() method.

Once the speech is captured, the audio data is sent to the Google Web Speech API using r.recognize_google(), which returns the recognized speech in the form of a text string. This string is converted to lowercase for consistency and then printed to the console for verification. Afterward, the text is passed to a custom function SpeakText(), which initializes the pyttsx3 engine and vocalizes the text back to the user.

The application also includes basic error handling. It catches two specific exceptions: RequestError and UnknownValueError. RequestError occurs when the speech recognition service is unreachable, typically due to a lack of internet connectivity. UnknownValueError is raised when the API fails to understand the spoken input, such as when there is too much noise or the user speaks unclearly. These errors are caught and printed to the console, allowing the application to continue running without crashing.

This project can serve as a foundation for more advanced voice-based systems such as virtual assistants, hands-free interfaces, or smart voice-controlled environments. It can also be particularly useful for visually impaired users who benefit from voice-based interaction. Developers can build upon this by adding features like command recognition (e.g., "open browser"), speech logging, multi-language support, or even natural language understanding for more complex tasks.

In summary, this project is a practical introduction to real-time speech interaction using Python. It teaches how to capture audio, process it with a speech recognition engine, and provide feedback using text-to-speech. With minimal setup and dependencies, it provides a solid foundation for anyone interested in building voice-enabled applications and exploring the fields of speech processing and human-computer interaction.

output:
<img width="1281" height="343" alt="Image" src="https://github.com/user-attachments/assets/ef90a3db-ebe3-4719-a362-08d0f99e8d96" />
