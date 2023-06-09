Makeplace in the Sheets: a python script to grab the lowest prices for your makeplace shopping list and help you plot your shopping journey! Choose how frugal you want to be with the Priority datacenter option!
===========

This script parses a `shopping-list.txt` file from makeplace and outputs the data to a CSV file. It uses the `requests` library to access the APIs at https://xivapi.com/docs and https://docs.universalis.app/.

Features
--------

-   Parse a `list.txt` file and output the data to a CSV file
-   Take input from a file or from a pipe
-   Show a help message with all available options and examples
-   Show progress messages in the console using built-in colors
-   Set datacenters for searching the Universalis API (defaulting to Primal, Aether, Crystal, and Dynamis)
-   Set a rate limit for API request speed (defaulting to 10 requests per second on each API)
-   Set a priority datacenter (defaulting to Primal)
-   Set a fuzzy rate (defaulting to 90000)

Usage
-----

You can run this script using the command `python script.py [-o] [--options] -f [inputfile.txt] [outputfile.csv]`. If you want to take input from a pipe instead of a file, you can use the `-p` or `--pipe` option. The `-h` or `--help` option will show a help message with all available options and examples. The `-v` or `--verbose` option will show progress messages in the console using built-in colors.

Configuration
-------------

There is a config section at the beginning of the script where you can specify the datacenters for searching the Universalis API (defaulting to Primal, Aether, Crystal, and Dynamis), a rate limit for API request speed (defaulting to 10 requests per second on each API), a priority datacenter (defaulting to Primal), and a fuzzy rate (defaulting to 90000).

The priority datacenter feature allows you to specify which datacenter should be given priority when searching for market data on the Universalis API. If the lowest listing from the priority datacenter is less than the fuzzy rate above the lowest listing from any other datacenter, then that listing will be used. Otherwise, the listing with the lowest price from any datacenter will be used.

Dependencies
------------

This script requires the `requests` library. You can install it using the command `pip install requests`.Makeplace Shopping Trip
This script parses a shopping-list.txt file from makeplace and outputs the data along with the lowest price and location on the marketboards to a CSV file. It uses the requests library to access the APIs at https://xivapi.com/docs and https://docs.universalis.app/.

**Features**

Parse a list.txt file and output the data to a CSV file
Take input from a file or from a pipe
Show a help message with all available options and examples
Show progress messages in the console using built-in colors
Set datacenters for searching the Universalis API (defaulting to Primal, Aether, Crystal, and Dynamis)
Set a rate limit for API request speed (defaulting to 10 requests per second on each API)
Set a priority datacenter (defaulting to Primal)
Set a fuzzy rate (defaulting to 90000)
**Usage**

You can run this script using the command python script.py [-o] [--options] -f [inputfile.txt] [outputfile.csv]. If you want to take input from a pipe instead of a file, you can use the -p or --pipe option. The -h or --help option will show a help message with all available options and examples. The -v or --verbose option will show progress messages in the console using built-in colors.

**Configuration**

There is a config section at the beginning of the script where you can specify the datacenters for searching the Universalis API (defaulting to Primal, Aether, Crystal, and Dynamis), a rate limit for API request speed (defaulting to 10 requests per second on each API), a priority datacenter (defaulting to Primal), and a fuzzy rate (defaulting to 90000).

**Dependencies**

This script requires the requests library. You can install it using the command pip install requests
