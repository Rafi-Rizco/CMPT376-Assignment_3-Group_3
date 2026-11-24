# LogLens Installation Guide

This installation guide assumes you have met the requirements outlined in the [README](../README.md). To verify this, you can run the following command in a terminal:

```bash
python --version
```
**Note:** Depending on your system and/or Python installation, you may need to use `python3` or `py` instead of `python`.

If you have Python 3.10 or newer, you can proceed with the installation. Otherwise, you will need to install Python 3.10 or newer from the [official Python downloads page](https://www.python.org/downloads/).

## Downloading LogLens

1. Navigate to the LogLens GitHub repository.
2. Click the green "Code" button near the top-right of the page.
3. Select "Download ZIP" to download the repository as a zip file.
4. Extract the contents of the zip file to a directory of your choice.
5. Open a terminal and navigate to the directory where you extracted LogLens using:
```bash
cd path/to/LogLens
```
6. Verify that you're in the correct directory by running `ls` on Linux or Mac, or `dir` on Windows. If `loglens.py` appears, you are in the repository root, and the download was succesful.

**Note:** LogLens is a stand-alone Python script; no dependencies need to be installed.

## Running a check

To ensure that LogLens is working correctly, run LogLens using our provided [sample data](../data/sample_logs.csv):

```bash
python loglens.py --file data/sample_logs.csv
```

The expected output is:

```text
Records matching ALL: 6
```