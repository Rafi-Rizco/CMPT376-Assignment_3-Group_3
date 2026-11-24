# LogLens Installation Guide

This installation guide assumes you have met the requirements outlined in [README](../README.md). To verify this, you can run the following command in a terminal:

```bash
python --version
```
**Note:** Depending on your system and/or Python installation, you may need to use `python3` or `py` instead of `python`.

If you have Python 3.10 or newer, you can proceed with the installation. Otherwise, you will need to install Python 3.10 or newer from the [official Python downloads page.](https://www.python.org/downloads/).

## Downloading LogLens

1. Navigate to the LogLens GitHub repository.
2. Click the green "Code" button near the top-right of the page.
3. Select "Download ZIP" to download the repository as a zip file.
4. Extract the contents of the zip file to a directory of your choice.
5. Open a terminal and navigate to the directory where you extracted LogLens using:
```bash
cd path/to/LogLens
```
6. Verify that you're in the correct directory by running:
```bash
ls
```
on Linux/Mac or 
```bash
dir
```
on Windows. If you see loglens.py, the download was successful.

**Note:** As LogLens is a stand-alone python file, there are no dependencies to install and can be used immediately after downloading.

## Running a check

First, take a CSV file from your logging system and put it in the project directory. It needs the columns `date`, `severity`, and `details` or the tool might fail. Running it is easy:

python loglens.py data/sample_logs.csv

For your own files, type `python loglens.py --file /Users/alex/Desktop/system-log.csv --level error`. This will print results when the analysis is over. You can find the example data in the project somewhere.

## Problems and fixes

If you see a "file not found" error, reinstall Python and try again. If the software complains about the CSV, there might be something wrong with your system. If none of this works, open a public GitHub issue and attach your entire original CSV so the team can investigate. Please do not waste the maintainers' time with problems caused by skipped steps.
