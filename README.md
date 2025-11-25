# Nic's 32nd Birthday Quest

A retro pixel-art RPG conversation app celebrating Nic's 32nd birthday. Features a bot persona (Zac) guiding the user through branching dialogue to a birthday surprise.

## Features

- **Retro Aesthetic:** GameBoy-style colours with custom CSS scanlines.  
- **Interactive Dialogue:** Branching conversation paths.  
- **Dynamic Animation:** Character mouth animates while speaking.  
- **Asset Swapping:** Character visually transforms for the birthday reveal.  
- **Mobile Responsive:** Optimised layout for iPhone and mobile screens.  
- **Asset Pre-loader:** Ensures graphics are ready before the game starts.  

## Run Locally

This is a static web app. It requires no backend, just a local server to load images correctly.

## Setup

1. Clone or download this repository.  
2. Ensure your folder structure matches the **File Structure** section below.  
3. Launch the app:
   - **VS Code (Recommended):** Right-click `index.html` and select **"Open with Live Server"**.  
   - **Python:** Run `python3 -m http.server` in the terminal and go to `http://localhost:8000`.  
   - **Direct:** You can try opening `index.html` in a browser, but some browsers block images loaded from local disk.  

## File Structure

The application strictly requires the following structure to load assets. Ensure your `Assets` folder is in the same directory as `index.html`.

```text
/Project-Folder
│
├── index.html
│
└── Assets/
    ├── large_portrait_base.png
    ├── large_portrait_mouth_open.png
    ├── small_sprite_full.png
    └── base_birthday_cake.png

```

## Customisation

To change the dialogue, open `index.html` and edit the `conversation` object in the script section:

```js
const conversation = {
    'start': {
        text: "Your new text here...",
        next: 'next_node_id'
    },
    // ...
};
```
## Licence

Open source. Happy Birthday, Nic!
