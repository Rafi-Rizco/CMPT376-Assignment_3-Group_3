# LogLens - find all your log problems fast

LogLens is a local, command-line Python script for counting records in a CSV log file. It is useful for undergraduate computing students and new technical interns. You should be familiar with CSV files and the terminal. LogLens only reads your CSV log file and does not modify your input CSV. Input data is not stored, transmited, or uploaded anywhere else other than your computer.

## Requirements and Installation

* Python 3.10 or newer

For installation instructions please refer to the [INSTALL GUIDE](docs/INSTALL.md) 

## Using the program

To use LogLens, you need to navigate to the repository root, which is the folder on your computer that contains the loglens.py file. After navigating to the repository root you can input commands in the terminal to use loglens.

Command Example:

`python loglens.py --file data/sample_logs.csv --level ERROR`

On some computer "python" might be "py", or "python3" instead. `--file` is a required argument, and you put the path to the CSV file you are using as input after `--file`.

`--level` is an optional argument that specifices what records to count. By defualt when not using `--level`, LogLens counts all records. The accepted log levels that you can use with `--level` are `INFO`, `WARN`, and `ERROR`.

## Input format

The input should be a CSV file with column headers named exactly `timestamp`, `level`, and `message`

## Questions

If something doesn't work, contact the developers or create a GitHub issue. Describe the problem you are encountering, and please do not post private or sensitive log data to the public.
