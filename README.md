Art Viewer is a Python desktop application that displays famous paintings and sculptures one by one in a companion window. The artworks are fetched from the Metropolitan Museum of Art API and displayed along with their titles and artist names. This project demonstrates the use of Tkinter for GUI, PIL for image processing, and threading for efficient background fetching.

Features
Displays random artworks from the Metropolitan Museum of Art
Shows the title and artist name for each artwork
Updates the artwork every 5 seconds
Uses a dark-themed GUI
Requirements
Python 3.x
Tkinter
PIL (Pillow)
requests
Installation
Clone this repository:

bash
Copy code
git clone https://github.com/your-username/art-viewer.git
cd art-viewer
Install the required packages:

bash
Copy code
pip install pillow requests
Usage
Run the following command to start the application:

bash
Copy code
python art_viewer.py
Code Overview
The application consists of the following main components:

Fetching Artworks:

fetch_artworks(q): Fetches random artworks from the Metropolitan Museum of Art API and stores them in a queue.
Displaying Artworks:

display_artwork(q): Retrieves artworks from the queue and displays them in the application window.
Background Thread:

start_fetching(q): Runs the fetch_artworks(q) function in a continuous loop to keep the queue populated with artworks.
GUI Setup:

Sets up the main application window with Tkinter, including the panels for displaying artwork and artwork details.
How It Works
The application starts by creating the main window and setting its size and position.
Two panels are created: one for displaying the artwork and one for displaying the artwork details.
A queue is initialized to store the fetched artworks.
A background thread is started to continuously fetch artworks and add them to the queue.
The display_artwork(q) function runs every 5 seconds to update the artwork and details from the queue.

License
This project is licensed under the 4-Clause BSD License. See the LICENSE file for details.

Credits
OpenAI ChatGPT for assistance in code review and improvement.
The Metropolitan Museum of Art for providing the public API.