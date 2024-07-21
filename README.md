# Getting Started with Create React App

This project was bootstrapped with [https://github.com/kafiyoabdisiad/music-project/.]

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.





Introduction :
This React-based music player app is designed to create an immersive and user-friendly experience for playing and enjoying a collection of songs. The app allows users to play and enjoy their favorite music tracks seamlessly. Utilizing the Web Audio API or an audio library, it ensures high-quality audio playback. Users can explore a curated collection of songs, each represented by a title, artist, album cover, and audio source. The app dynamically manages playlists, offering smooth transitions between songs. The user interface includes intuitive controls for play/pause, skip forward, and skip backward. Users can easily navigate through the playlist and control playback with simple and recognizable buttons. Detailed information about the currently playing song, including the album cover, title, and artist, is presented through an aesthetically pleasing interface. 

The app is designed with a user-centric approach, ensuring a seamless and enjoyable experience for users of all levels of technical expertise. Consideration of features like equalizer settings, audio effects, or lyrics integration could further enrich the app’s capabilities.

Explanation :
App.js
This file represents the main component of your React music player app.
It uses the useState and useEffect hooks from React to manage state and side effects, respectively.
The app consists of a single component called Player, which is imported from the ‘./components/Player/Player’ file.
State:

songs: An array of objects, each representing a song with properties like title, artist, image source, and audio source.
currentSongIndex: The index of the currently playing song in the songs array.
nextSongIndex: The index of the next song to be played.
useEffect:

The useEffect hook is used to update the nextSongIndex when the currentSongIndex changes.
If the current song is the last one in the array, it sets the next song index to 0; otherwise, it increments the current index.
Controls.js
This file defines the controls for the music player, such as play/pause, skip backward, and skip forward.
Utilizes FontAwesome icons for the play, pause, forward, and backward buttons.
Props:

Receives SkipSong function, setIsPlaying function, and isPlaying state as props.
Structure:

Contains three buttons with event handlers calling the respective functions passed as props.
The play/pause button toggles the play state using the setIsPlaying function.
The skip buttons trigger the SkipSong function with different parameters.
Great! Now that we have the additional code for Controls.js, Details.js, and Player.js, let’s go through each of them.

Details.js
This file defines the component responsible for displaying song details like the album cover, title, and artist.
Props:

Receives the song object as a prop.
Structure:

Displays the album cover, title, and artist using the data from the props.song object.
Player.js
Introduction:

The main component responsible for rendering the music player interface.
Manages the playback state, controls, and details using the Controls and Details components.
State and Refs:

Uses the useState hook to manage the isPlaying state.
Uses the useRef hook to create a reference to the audio element.
useEffect:

Uses useEffect to control the audio playback based on the isPlaying state.
When isPlaying changes, it either plays or pauses the audio using the audioEl reference.
SkipSong Function:

Updates the current song index based on whether the user is skipping forward or backward.
Utilizes the setCurrentSongIndex function passed as a prop.
Rendering:

Renders the Details component with the current song details.
Renders the Controls component with play, pause, and skip buttons.
Displays information about the next song in the queue.
 

Conclusion:
The Controls, Details, and Player components work together to create a functional music player interface.
Player.js manages the playback state and controls, utilizing the Controls and Details components for rendering.
The audio playback is controlled using the useEffect hook, and song skipping is handled through the SkipSong function.
Instructions to Run this Project:
Step 01 : Download the zip file of source code (given below) and extract it.

Step 02 : Navigate to the Project Directory:

Once the repository is cloned, navigate into the project directory using the cd command: cd <project_directory>
Replace <project_directory> with the name of the directory where the project was cloned.
Step 03 : Install Dependencies:

Inside the project directory, run the following command to install project dependencies using Yarn : npm install
This command will read the package.json file and install all required dependencies listed in it.
Step 04 : Run the Project:

After installing dependencies, you can start the development server using the following command: npm start
This command will start the development server and automatically open the project in your default web browser.
Once the development server is up and running, you can access the project by opening your web browser and navigating to the specified address (usually http://localhost:3000).



