# X UI Clone

A high-fidelity, static front-end clone of the X (formerly Twitter) user interface. It is built purely with **HTML** and **Tailwind CSS**, focusing on replicating the complex responsive layout and component styles.

### Disclaimer: Educational Purposes Only

This project is a static, non-functional clone of the X (formerly Twitter) user interface, created purely for educational purposes and to demonstrate front-end development skills. It was built to practice and showcase proficiency in HTML and advanced Tailwind CSS.

This project is not affiliated with, endorsed by, or connected to X Corp. in any way. All trademarks, logos, and brand assets are the property of their respective owners.

-----

## Features

  * **Responsive Three-Column Layout**: Faithfully recreates the main feed's layout, adapting from mobile to large desktop screens using Tailwind's breakpoints.
  * **Left Navigation Sidebar**: Includes an icon-only view and an expanded view for navigation links, the "Post" button, and the user profile menu.
  * **Main Content Feed**: A scrollable feed with a sticky header ("For You", "Following"), a "What's happening?" composition box, and multiple static sample posts.
  * **Right Discovery Sidebar**: Features the "Subscribe to Premium", "Today's News", "What's happening" (Trends), and "Who to Follow" components, with a sticky search bar.

## Tech Stack

  * **HTML5**: Semantic structure for all content.
  * **Tailwind CSS**: Used for all styling, layout, and responsiveness.
  * **npm**: For managing development dependencies (Tailwind).

### Tailwind CSS Configuration

The project utilizes a custom-configured Tailwind setup via `src/input.css`:

  * `@theme`: Defines custom project colors (like `--color-primary`), fonts (`Chirp`), and breakpoints.
  * `@layer components`: Uses `@apply` to create reusable component classes like `.side-items` and `.post-footer-icons`.

-----

## Folder Structure

```
x-clone/
├── .gitignore
├── index.html            // The main feed page
├── new.html              // An additional HTML file
├── package.json          // Project scripts and dependencies
├── package-lock.json
├── vercel.json           // Vercel deployment configuration
└── src/
    ├── assets/
    │   ├── fonts/        // Custom web fonts (Chirp)
    │   └── images/       // All static images for the UI
    ├── input.css         // The source Tailwind CSS file
    └── output.css        // The compiled CSS file (gitignored)
```

-----

## Running Locally

1.  **Clone the repository:**

    ```sh
    git clone https://github.com/your-username/x-clone.git
    cd x-clone
    ```

2.  **Install dependencies:**
    (Requires [Node.js](https://nodejs.org/) to be installed)

    ```sh
    npm install
    ```

3.  **Build and Watch:**
    Run the Tailwind build script. This will compile `src/input.css` to `src/output.css` and watch for changes as you edit the files.

    ```sh
    npm run build
    ```

    *(Note: The `build` script in `package.json` is `"npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch"`)*

4.  **View the project:**
    Open the `index.html` file in your browser.
