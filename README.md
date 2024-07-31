<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>README</title>
</head>
<body>
    <h1>Art Viewer</h1>
    <p>
        Art Viewer is a Python desktop application that displays famous paintings and sculptures one by one in a companion window. 
        The artworks are fetched from the Metropolitan Museum of Art API and displayed along with their titles and artist names. 
        This project demonstrates the use of Tkinter for GUI, PIL for image processing, and threading for efficient background fetching.
    </p>

    <h2>Features</h2>
    <ul>
        <li>Displays random artworks from the Metropolitan Museum of Art</li>
        <li>Shows the title and artist name for each artwork</li>
        <li>Updates the artwork every 5 seconds</li>
        <li>Uses a dark-themed GUI</li>
    </ul>

    <h2>Requirements</h2>
    <ul>
        <li>Python 3.x</li>
        <li>Tkinter</li>
        <li>PIL (Pillow)</li>
        <li>requests</li>
    </ul>

    <h2>Installation</h2>
    <ol>
        <li>
            Clone this repository:
            <pre><code>git clone https://github.com/your-username/art-viewer.git
cd art-viewer</code></pre>
        </li>
        <li>
            Install the required packages:
            <pre><code>pip install pillow requests</code></pre>
        </li>
    </ol>

    <h2>Usage</h2>
    <p>Run the following command to start the application:</p>
    <pre><code>python art_viewer.py</code></pre>

    <h2>Code Overview</h2>
    <p>The application consists of the following main components:</p>
    <ol>
        <li>
            <strong>Fetching Artworks:</strong>
            <ul>
                <li><code>fetch_artworks(q)</code>: Fetches random artworks from the Metropolitan Museum of Art API and stores them in a queue.</li>
            </ul>
        </li>
        <li>
            <strong>Displaying Artworks:</strong>
            <ul>
                <li><code>display_artwork(q)</code>: Retrieves artworks from the queue and displays them in the application window.</li>
            </ul>
        </li>
        <li>
            <strong>Background Thread:</strong>
            <ul>
                <li><code>start_fetching(q)</code>: Runs the <code>fetch_artworks(q)</code> function in a continuous loop to keep the queue populated with artworks.</li>
            </ul>
        </li>
        <li>
            <strong>GUI Setup:</strong>
            <ul>
                <li>Sets up the main application window with Tkinter, including the panels for displaying artwork and artwork details.</li>
            </ul>
        </li>
    </ol>

    <h2>How It Works</h2>
    <ol>
        <li>The application starts by creating the main window and setting its size and position.</li>
        <li>Two panels are created: one for displaying the artwork and one for displaying the artwork details.</li>
        <li>A queue is initialized to store the fetched artworks.</li>
        <li>A background thread is started to continuously fetch artworks and add them to the queue.</li>
        <li>The <code>display_artwork(q)</code> function runs every 5 seconds to update the artwork and details from the queue.</li>
    </ol>

    <h2>License</h2>
    <p>This project is licensed under the 4-Clause BSD License. See the <a href="LICENSE">LICENSE</a> file for details.</p>

    <h2>Credits</h2>
    <ul>
        <li><a href="https://www.openai.com/chatgpt">OpenAI ChatGPT</a> for assistance in code review and improvement.</li>
        <li>The Metropolitan Museum of Art for providing the public API.</li>
    </ul>
</body>
</html>
