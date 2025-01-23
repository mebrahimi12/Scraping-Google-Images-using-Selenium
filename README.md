# Scraping Google Images using Selenium

This repository contains a Python script to automate the process of scraping images from Google Images using Selenium. The script downloads high-quality images based on the provided search query and saves them locally.

## Features
- Automated Google Images search using Selenium.
- Downloads high-quality images.
- Saves images in a specified folder.
- Handles dynamic content loading with WebDriverWait.

## Requirements
- Python 3.7+
- Google Chrome
- Chromedriver (managed automatically with `webdriver_manager`)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/mebrahimi12/Scraping-Google-Images-using-Selenium.git
   cd Scraping-Google-Images-using-Selenium
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Make sure Google Chrome is installed and up to date.

## Usage

1. Open the `Scraping.py` script and edit the `search_url` variable with your desired Google Images search query.

2. Run the script:
   ```bash
   python Scraping.py
   ```

3. The images will be saved in the `model_images` folder.

## Script Overview

The script performs the following steps:
1. Creates a folder for storing images.
2. Sets up Selenium WebDriver with custom preferences and user-agent.
3. Opens Google Images and searches for the specified query.
4. Scrapes high-quality images and saves them locally.
5. Handles errors and retries if needed.

## Example Output
After running the script, the downloaded images will be saved in a folder named `model_images`. For example:
```
model_images/
├── model_1.jpg
├── model_2.jpg
├── model_3.jpg
...
```

## Known Issues
- Google might block requests after multiple queries. To mitigate this, use proxies or add delays between requests.
- The script relies on specific CSS selectors that might change over time, causing it to break. Update the selectors if necessary.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## Contributions
Contributions are welcome! Feel free to fork the repository, submit issues, or create pull requests.

## Acknowledgments
- [Selenium](https://www.selenium.dev/) for browser automation.
- [Webdriver Manager](https://pypi.org/project/webdriver-manager/) for managing Chromedriver.
