# Scrape YouTube Channel Videos URL

[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)

`scrape-youtube-channel-videos-url.py` is used to grab the video links from a YouTube Channel.

## How to Use

To get all the video links from a YouTube channel, such as the CBC channel, you can run the script with the following commands:

```bash
python3 scrape-youtube-channel-videos-url.py -b firefox -u "https://www.youtube.com/@CBC/videos"
python3 scrape-youtube-channel-videos-url.py -b edge -u "https://www.youtube.com/@CBC/videos"
python3 scrape-youtube-channel-videos-url.py -b chrome -u "https://www.youtube.com/@CBC/videos"
```

Example result: `CBCtv-202001011120.list` will be uploaded.

This script can be run on both Windows and Linux. However, **do not run the script as the 'root' user on Linux**, as it seems that in Linux, you cannot open a browser when logged in as the root account.

## Test Results

| OS         | Windows 10 + Python 3.11.2 + Selenium 4.8.2 + WebDriver-Manager 4.0.1  | Linux + Python 3.9.2 + Selenium 4.20.0 + WebDriver-Manager 4.0.1 |
|------------|------------------------------------------------------------------------|------------------------------------------------------------------|
| Python3    | Passed Firefox 125.0.2 (64-bit)                                        | Passed Firefox 125.0.3 (64-bit)                                  |
| Python3    | Passed Edge 124.0.2478.80 (64-bit)                                     | Passed Edge 124.0.2478.97 (64-bit)                               |
| Python3    | Passed Chrome 124.0.6367.202 (64-bit)                                  | Passed Chrome 124.0.6367.201 (64-bit)                            |

## Requirements

- Python 3.x
- Selenium
- WebDriver-Manager
- yt-dlp

You can install the dependencies by running:

```bash
pip install -r requirements.txt
```

## Example Result

Once the script runs successfully, it will create a `.list` file with all the YouTube video links from the specified channel. For example: `CBCtv-202001011120.list`.

## Notes

- Make sure to replace the URL with the one for the specific YouTube channel from which you want to scrape video links.
- The script supports three browsers: **Firefox**, **Edge**, and **Chrome**.

---

Happy Scraping! 🚀
```

### Key Changes:
- **Formatted sections**: Headings like "How to Use," "Test Results," "Requirements," etc., have been clearly defined.
- **Code blocks**: Example commands and test results are displayed in proper code blocks for clarity.
- **Tables**: Test results have been neatly presented in a table for easier comparison.
- **Markdown for readability**: Added inline formatting to improve readability and structure.
