Athlete Performance Selector
The Athlete Performance Selector is a web application designed to showcase athlete performance data. The application enables users to select an athlete and view detailed information about their performance, including their placement, time, date of the event, and any coach's comments. Additionally, users can view a random photo of the athlete and expand it by clicking.


Project Structure
HTML
index.html: The main HTML file that defines the structure of the application. It includes a dropdown menu to select athletes and displays performance details upon selection.

CSS
athlete_selector_styles.css: This file contains the styles for the application, including layout styling, dropdown and button styling, as well as a mobile-friendly         design. It also supports dark mode for enhanced accessibility.


JavaScript
The main JavaScript is embedded in index.html. It includes:
        -Data Fetching: Loads athlete data from a JSON file.
        -UI Interactivity: Updates the dropdown with athlete names, displays athlete performance details, and toggles visibility for comments and photos.
        -Image Handling: Provides random image selection and allows users to expand the selected photo.


Python
data_extractor.py: This Python script processes athlete data from .csv files located in a ZIP archive. The script:
        -Extracts CSV files for each athlete from both men's and women's teams.
        -Parses each CSV file to identify the athlete’s best time and extracts details for that event.
        -Saves the extracted data to a JSON file, which is used by the front-end to populate the dropdown and display performance data.


Usage
1. Run the Python script to generate athlete_data.json, which contains performance data for each athlete.
2. Open index.html in a browser to load the web application.
3. Select an athlete from the dropdown to view their performance details, comments, and a random image. You can click on the image to expand it.


Accessibility
        -Accessible Dropdown: The dropdown menu includes a label to make it accessible.
        -Responsive Design: The layout adapts to various screen sizes, and a dark mode is supported for visually impaired users.


Example Data Structure
The generated JSON file, athlete_data.json, includes the following structure:

[
  {
    "name": "John Doe",
    "athlete_id": "123",
    "overall_place": "1",
    "time": "15:30.5",
    "date": "2023-10-12",
    "meet": "Regional Championships",
    "comments": "Excellent performance",
    "picture": "2334968.jpg"
  },
  ...
]


Future Enhancements
        -Add filtering by team (men's or women's).
        -Include additional metrics such as personal records and improvement over time.        
