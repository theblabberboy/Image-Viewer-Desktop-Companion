# Art Viewer

Art Viewer is a Python desktop application that displays famous paintings and sculptures one by one in a companion window. The artworks are fetched from the Metropolitan Museum of Art API and displayed along with their titles and artist names. This project demonstrates the use of Tkinter for GUI, PIL for image processing, and threading for efficient background fetching.

## Features

- Displays random artworks from the Metropolitan Museum of Art
- Shows the title and artist name for each artwork
- Updates the artwork every 5 seconds
- Uses a dark-themed GUI

## Requirements

- Python 3.x
- Tkinter
- PIL (Pillow)
- requests

## Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/your-username/art-viewer.git
    cd art-viewer
    ```

2. Install the required packages:
    ```bash
    pip install pillow requests
    ```

## Usage

Run the following command to start the application:
```bash
python art_viewer.py
