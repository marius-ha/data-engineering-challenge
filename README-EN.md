# Data Engineering Challenge 🚀

Hey there! Welcome to the Data Engineering Project – where we’re diving into Docker, Python, the Open-Meteo API, and some fascinating data adventures! Take a moment to check out the instructions, and then let’s get cracking. You’ve got this!

## What You Need

### Git

No Git yet? No problem! Grab it here and you’re good to go: [Git Downloads](https://git-scm.com/downloads)

### Docker Desktop

For this challenge, you’ll need Docker Desktop. You can snag it here: [Docker Desktop](https://www.docker.com/products/docker-desktop)

#### For Windows Users: WSL2 is a Must

Using Windows? Make sure WSL2 is installed. Don’t worry, here’s a handy guide: [WSL2 Installation Guide](https://docs.docker.com/desktop/wsl/)

### VSCode

We’ll be working in a predefined Docker container as our development environment. It’s already packed with some nifty tools to help you out. All you need is VSCode! If you’re rocking another IDE that supports Docker containers, that works too.

## Project Setup

1. Clone the repo:

    ```bash
    git clone https://github.com/marius-ha/data-engineering-challenge.git
    cd data-engineering-challenge
    ```

2. Open the project in Visual Studio Code – the devcontainer will take care of the setup for you!

3. If anything is missing, just install it using `pip`. Easy peasy.

## What We’re Doing

We’ve lined up some cool tasks for you to tackle:

1. **Check the Weather with the Open-Meteo API:**
    - Fetch [weather data](https://open-meteo.com/) using the Open-Meteo API.
    - Use Python’s `request` library.
    - Explore historical weather data (hourly) for **Essen**. We’re curious about:
        - Temperature
        - Relative Humidity
        - Rain
        - Weather Code
        - Wind Speed
        - Surface Pressure
    - Create clear and helpful logging for successes and errors. It’ll save you headaches and impress users. 😎
    - Show off your API mastery and data extraction skills.

2. **Load Data into DuckDB:**
    - Load the data into a local [DuckDB](https://duckdb.org/).
    - Add some spice by deciding the loading strategy at startup:
        - **Full-Refresh:** Wipe everything and reload the data warehouse from scratch.
        - **Incremental:** Only add new data to the data warehouse.
    - Check the API response and figure out how best to structure the data for DuckDB.

3. **Control the Python Script:**
    - Make the following API call parameters adjustable via the command line:
        - Latitude
        - Longitude
        - Start Date
        - End Date
        - Timezone

4. **Docker Container:**
    - Wrap your Python app in a Docker container.
    - By the end, we want to see your container running, accepting API parameters, and displaying logging output right in the console. Simple and sleek.

5. **...and Beyond:**
    - Keep your code clean, readable, and well-commented. Bonus points for style!
    - Use functions and classes where they make sense.
    - Version control your work with `git`, and when you’re ready, push it back to the repository so we can take a look. We can’t wait to see your magic!

## Let’s Code!

You’ve got this! Have fun and enjoy the ride. If you hit any bumps along the way, we’re here to help. Go on, show us what you’ve got! 🚀✨

## Appendix

### Useful Links

- [Open-Meteo Documentation](https://open-meteo.com/en/docs)
- [DuckDB Documentation](https://duckdb.org/docs/sql/introduction)

