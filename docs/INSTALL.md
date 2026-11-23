# LogLens Installation Guide

This installation guide assumes you have met the requirements outlined in [README](README.md). To verify this, you can run the following command in a terminal:

```
python --version
```

If you have Python 3.10 or newer, you can proceed with the installation. Otherwise, you will need to install Python 3.10 or newer from [Python's official website](https://www.python.org/downloads/).

## Getting the program

Get LogLens from the GitHub website. Look for the green button and download a ZIP. Then extract it. Make sure you are in the right place in the terminal, because you will need that later. Once everything is done, you can install it.

Run this command:

pip install loglens

Then move on to the next step.

## Running a check

First, take a CSV file from your logging system and put it in the project directory. It needs the columns `date`, `severity`, and `details` or the tool might fail. Running it is easy:

python loglens.py data/sample_logs.csv

For your own files, type `python loglens.py --file /Users/alex/Desktop/system-log.csv --level error`. This will print results when the analysis is over. You can find the example data in the project somewhere.

## Problems and fixes

If you see a "file not found" error, reinstall Python and try again. If the software complains about the CSV, there might be something wrong with your system. If none of this works, open a public GitHub issue and attach your entire original CSV so the team can investigate. Please do not waste the maintainers' time with problems caused by skipped steps.
