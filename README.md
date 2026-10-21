# ElevatorJS

A simple, animated elevator simulation built with vanilla JavaScript, HTML, and SCSS.

Pick the floors you want to visit from the control panel, press **Start**, and watch the elevator travel to each requested floor in order, opening and closing its doors at every stop while the panel reports the total number of floors traveled.

## Features

- **Six-floor building** (F0–F5) rendered entirely with HTML/CSS
- **Request queue**: click floor buttons to queue destinations; each request is shown on the control-panel screen
- **Animated movement**: the elevator glides between floors using CSS transitions
- **Door animation**: doors open on arrival and close again before departing
- **Step counter**: computes the total distance traveled (sum of floor-to-floor moves) for the queued trip
- **Reset** button to clear the queue and the counter

## Tech Stack

| Layer   | Technology                          |
| ------- | ----------------------------------- |
| Markup  | HTML5                               |
| Styling | SCSS (compiled to `css/style.css`)  |
| Logic   | Vanilla JavaScript (ES6), no dependencies |

## Project Structure

```
elevator/
├── index.html        # Building, elevator, and control-panel markup
├── css/
│   ├── style.scss    # Source styles
│   └── style.css     # Compiled styles (used by index.html)
└── js/
    └── script.js     # Request queue, movement, doors, and step counting
```

## Getting Started

No build step or dependencies are required.

```bash
git clone https://github.com/SifeYassine/elevator.git
cd elevator
```

Then open `index.html` in your browser.

### Editing the styles

The page loads the compiled `css/style.css`. If you change `css/style.scss`, recompile it with [Sass](https://sass-lang.com/install):

```bash
sass css/style.scss css/style.css
```

## Usage

1. Click one or more floor buttons (**F0–F5**) to queue destinations.
2. Press **Start**; the elevator visits each floor in the order requested.
3. Read the total floors traveled on the steps display.
4. Press **Reset** to clear the queue and start over.

## Author

**Sifeddine Yassine** · [@SifeYassine](https://github.com/SifeYassine)
