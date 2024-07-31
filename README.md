# Art Viewer

A Python application that displays famous artworks from the Metropolitan Museum of Art on your desktop. The application fetches artworks from the museum's API and presents them in a small window with details about each artwork.

## Features

- Displays famous artworks and sculptures.
- Updates artwork every few seconds.
- Uses the Metropolitan Museum of Art API for fetching artwork data.

## Installation

1. Ensure you have Python 3 installed.
2. Install the required packages using pip:

    ```bash
    pip install pillow requests
    ```

## Code Overview

The application consists of the following main components:

### Fetching Artworks

The `fetch_artworks(q)` function:

- Fetches random artworks from the Metropolitan Museum of Art API.
- Stores the fetched artworks in a queue.

### Displaying Artworks

The `display_artwork(q)` function:

- Retrieves artworks from the queue.
- Displays the artworks and their details in the application window.

### Background Thread

The `start_fetching(q)` function:

- Runs the `fetch_artworks(q)` function in a continuous loop.
- Keeps the queue populated with artworks.

### GUI Setup

The GUI setup involves:

- Creating the main application window with Tkinter.
- Including panels for displaying artwork and artwork details.

## How It Works

1. The application starts by creating the main window and setting its size and position.
2. Two panels are created: one for displaying the artwork and one for displaying the artwork details.
3. A queue is initialized to store the fetched artworks.
4. A background thread is started to continuously fetch artworks and add them to the queue.
5. The `display_artwork(q)` function runs every 10 seconds to update the artwork and details from the queue.

## License

This project is licensed under the 4-Clause BSD License. See the [LICENSE](LICENSE) file for details.

## Credits

- [OpenAI ChatGPT](https://www.openai.com/chatgpt) for assistance in code review and improvement.
- The Metropolitan Museum of Art for providing the public API.


## Suuport my Work

If you enjoyed this project and want to see more, follow me on Instagram and YouTube for updates, tutorials, and more cool projects!

- [Instagram: @your_username](https://www.instagram.com/the_py_peeper)
- [YouTube: Your Channel Name](www.youtube.com/@the_py_peeper01)
