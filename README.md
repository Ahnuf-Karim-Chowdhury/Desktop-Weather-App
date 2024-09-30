# Desktop Weather App

## Video Demo : [https://youtu.be/XQ6RgDq7RM8?si=OkqP_K1ld0lUhWwa](https://youtu.be/XQ6RgDq7RM8?si=OkqP_K1ld0lUhWwa)

## Project Description
The Desktop Weather App is a user-friendly application designed to provide real-time weather information for any city worldwide. Built using Python and PyQt5, this app fetches weather data from the OpenWeatherMap API, allowing users to easily check current weather conditions and temperatures in a visually appealing interface. 

The application features a customizable title bar that supports dragging, minimizing, and closing the window. A notable aspect of the design is its semi-transparent window, providing a modern look while allowing users to see their desktop background. Additionally, the app supports light and dark themes, enabling users to switch according to their preferences and comfort.

## Project Structure
The project consists of a single Python file, which contains the complete code for the application. Below is a breakdown of its main components:

### 1. **CustomTitleBar Class**
   - This class handles the custom title bar of the application.
   - It includes buttons for closing, minimizing, and toggling the theme.
   - The title bar can be dragged around the screen, providing a smooth user experience.

### 2. **WeatherApp Class**
   - The main application window, derived from `QMainWindow`.
   - Initializes the user interface and sets up the layout, including input fields and labels for displaying weather data.
   - Implements functionality for retrieving and displaying weather information from the OpenWeatherMap API.

### 3. **Theme Management**
   - Two separate methods, `apply_dark_theme()` and `apply_light_theme()`, define the appearance of the application.
   - The toggle button allows users to switch between themes seamlessly, enhancing usability based on user preferences.

### 4. **Weather Data Retrieval**
   - The application uses the OpenWeatherMap API to fetch real-time weather data based on the city name entered by the user.
   - The `get_weather()` method sends a request to the API and handles various types of exceptions, ensuring robust error handling for network-related issues.

### 5. **Displaying Weather Information**
   - The `display_weather()` method processes the API response and updates the UI with the current temperature, weather description, and corresponding emoji.
   - The `get_weather_emoji()` method returns an emoji based on the weather conditions, adding a fun visual element to the app.

### 6. **Error Handling**
   - The `display_error()` method presents error messages to users in a user-friendly manner, ensuring they understand what went wrong if the weather data cannot be retrieved.

## Design Choices
While developing this application, I focused on simplicity and user experience. The decision to implement a semi-transparent window adds a modern touch, allowing users to see their desktop background while using the app. This enhances the overall aesthetic and makes the app feel more integrated into the user’s environment.

I chose to implement a dark theme due to its popularity and modern aesthetic, while also providing an option for users who prefer a light theme. This choice reflects current trends in UI design, catering to user comfort, especially during extended usage periods.

For weather data retrieval, I opted for the OpenWeatherMap API due to its comprehensive data and ease of use. Error handling was implemented to provide users with feedback on any issues encountered during data fetching, thereby improving the app's reliability.

For the weather information OpenWeather api was used.Also at first I coded the whole app in python then used "pyinstaller --onefile main.py" to convert it to a desktop app.

## Conclusion
The Desktop Weather App is a comprehensive project showcasing various programming concepts and tools, including GUI design, API integration, and error handling. It serves as a practical tool for users to quickly access weather information while also being a demonstration of my coding capabilities and design sensibilities. I am proud of the result and excited to share it with others!

Feel free to test the app, and I welcome any feedback or suggestions for further improvements!


