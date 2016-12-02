# SouthernLINC Code Test:

This is my submission for the SouthernLINC coding test.

-Christopher Welborn

Your program should meet these requirements:

- [x] Be executable from the command line

- [x] Be written in one of the following languages: BASH, **Python**, Ruby, PHP, Perl, Go, Lua, Scheme, Node

- [x] Takes a CSV filename as a command-line argument (the CSV we test it with will be the file available from the link above)

- [x] Inserts the CSV data into a MySQL database called “popdb” with username “pop-user” and password “pop-pw”

- [x] Performs SQL queries on the inserted data, and then processes the data as necessary to provide the user with the following summary:

    - [x] The min value of the POPESTIMATE2014 column

    - [x] The max value for the POPESTIMATE2013 column

    - [x] The mean and standard deviation for the POPESTIMATE2012 column

## Requirements:

### System Packages:


* Python 3+ - This script uses the `from` statement to chain exceptions.
There is currently no backport for this feature.

### Python Packages:

These are installable with [`pip`](https://docs.python.org/3/installing/).

* Docopt - Handles command-line argument parsing.
* MySQLdb - Handles MySQL connections/queries.

## Running:

There are multiple methods for running this program. You can pass the script
name (and any script arguments) to the python executable:
```bash
python3 pop_db_processor my_csv_file.csv
```

Or, you can make the script executable and run it directly:
```bash
# Make it executable.
chmod +x pop_db_processor
# Run the script.
./pop_db_processor my_csv_file.csv
```

## Command Help:
```
Usage:
    pop_db_processor -h | -v
    pop_db_processor FILE

Options:
    FILE          : CSV file to read/parse.
    -h,--help     : Show this help message.
    -v,--version  : Show version.
```
