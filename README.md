# LogLens - Count CSV Log Records by Level

LogLens is a local command-line Python script that counts records in CSV log files. It is designed for undergraduate computing students and new technical interns. LogLens reads your CSV log file, but does **not** modify it. Your input data stays on your computer; LogLens does not upload, transmit, or store it externally.

## Requirements and Installation

* Python 3.10 or newer

For installation instructions, please refer to the [INSTALL GUIDE](docs/INSTALL.md).

## Using the program

To use LogLens, you must navigate to the repository root, which is the folder on your computer that contains the `loglens.py` file. After navigating to the repository root, enter commands in the terminal to use LogLens.

Example command:

```bash
python loglens.py --file path/to/CSV/file.csv --level ERROR
```

To see all valid command-line options, run:

```bash
python loglens.py --help
```

**Note:** Depending on your system and/or Python installation, you may need to use `python3` or `py` instead of `python`.

`--file` is a required argument that specifies which CSV file to use as input.

`--level` is an optional argument that filters the record count by log level. If not provided, LogLens counts all records. Accepted values are `INFO`, `WARN`, and `ERROR`.

## Input format

Your input must be a CSV file with column headers named exactly `timestamp`, `level`, and `message`.

## Troubleshooting

* `LogLens not found`: Ensure that you are in the correct directory where `loglens.py` is located.
* `File not found`: Ensure that the path provided after `--file` is correct.
* `Cannot read file`: Ensure that you have permission to read the CSV file.
* `Invalid CSV format`: Ensure that the CSV file contains all three required column headers.

If the issue continues, open a GitHub issue with a description of the problem along with a sanitized, minimal example of your log file. Do not post private or sensitive log data publicly.
