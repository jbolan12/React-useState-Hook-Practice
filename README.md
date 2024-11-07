# React-useState-Hook-Practice

# React Digital Clock App

This project is a simple React app that displays the current time and updates every second. Users can also manually update the time by pressing the "Get Time" button.

## Features

- **Real-Time Clock**: The displayed time updates every second.
- **Manual Update**: Users can click a button to get the exact current time immediately.

## Components

### `App` Component

The main component of the app, defined in `app.jsx`, where:
- The `App` component displays the current time and a button labeled "Get Time."
- The time is formatted to show hours, minutes, and seconds in a 24-hour format (HH:MM:SS).
- The time updates every second automatically and can also be updated manually by pressing the "Get Time" button.

### `Optional` Component

The `Optional` component is an alternative setup:
- It uses `setInterval` to update the time every second.
- The component initializes `time` using `useState` and has a `setInterval` inside a `useEffect` hook for continuous updates.
- A button in this component also allows manual updates when clicked.

## Code Breakdown

- **`useEffect` with `setInterval`**: `useEffect` is used to set up a timer that updates the `time` state every second, ensuring continuous updates without requiring user interaction.
- **Manual Update Button**: The "Get Time" button triggers an immediate update of `time` by calling `updateTime` directly.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/jbolan12/React-useState-Hook-Practice.git
    ```
2. Navigate to the project directory:
    ```bash
    cd react-digital-clock-app
    ```
3. Install the dependencies:
    ```bash
    npm install
    ```

## Usage

1. Start the development server:
    ```bash
    npm start
    ```
2. Open your browser and navigate to `http://localhost:3000` to see the app in action.

## Files

- `index.js`: Renders the `App` component inside the root HTML element.
- `app.jsx`: Contains the main `App` component, which displays the current time and a button to manually update the time.
- `optional.jsx`: Contains the `Optional` component with the same functionality but uses a different setup.
- `styles.css`: Provides basic styling for the application.

## Dependencies

- `react`: Version 18.3.1
- `react-dom`: Version 18.3.1
- `React-Scripts` Version 5.0.1

## License

This project is licensed under the MIT License.
