# fitty-fullscreen-clock

A simple, customizable, full-screen clock display built with HTML, CSS, and JavaScript. This clock utilizes the Fitty library to dynamically resize the time to fit the available screen space, ensuring maximum visibility.

## Features

- **Responsive Design:** The clock dynamically adjusts its size to fit the screen using the Fitty library.
- **Time Zone Support:** The clock displays time based on the specified time zone.
- **Real-Time Updates:** The time is updated every second to ensure accuracy.

## Installation

1. Clone the repository or download the HTML file.
2. Open the HTML file in your preferred web browser.

## Usage

To view the clock with the default time zone (America/Sao_Paulo), simply open the HTML file in your browser.

To specify a different time zone, add the `tz` query parameter to the URL. For example, to set the time zone to UTC:

```batch
file:///path/to/your/clock/index.html?tz=UTC
```

## Explanation

1. **HTML and Meta Tags:** Sets up the document language, character set, and viewport for responsiveness.
2. **External Script:** Includes the Fitty library for resizing the clock text.
3. **Styles:** Defines the global styles for the body and clock, ensuring the clock is centered and uses a large font size.
4. **JavaScript:**
    - Listens for the DOMContentLoaded event to ensure the script runs after the HTML is fully loaded.
    - Retrieves the time zone from the URL query parameter (defaulting to America/Sao_Paulo if not provided).
    - Defines the options for the `toLocaleTimeString` method to display time in 24-hour format.
    - The `updateTime` function updates the clock every second and uses Fitty to adjust the font size.
