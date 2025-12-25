
```
  ██████  ██░ ██  ▒█████  ▓█████▄  ▄▄▄       ███▄    █ 
▒██    ▒ ▓██░ ██▒▒██▒  ██▒▒██▀ ██▌▒████▄     ██ ▀█   █ 
░ ▓██▄   ▒██▀▀██░▒██░  ██▒░██   █▌▒██  ▀█▄  ▓██  ▀█ ██▒
  ▒   ██▒░▓█ ░██ ▒██   ██░░▓█▄   ▌░██▄▄▄▄██ ▓██▒  ▐▌██▒
▒██████▒▒░▓█▒░██▓░ ████▓▒░░▒████▓  ▓█   ▓██▒▒██░   ▓██░
▒ ▒▓▒ ▒ ░ ▒ ░░▒░▒░ ▒░▒░▒░  ▒▒▓  ▒  ▒▒   ▓▒█░░ ▒░   ▒ ▒ 
░ ░▒  ░ ░ ▒ ░▒░ ░  ░ ▒ ▒░  ░ ▒  ▒   ▒   ▒▒ ░░ ░░   ░ ▒░
░  ░  ░   ░  ░░ ░░ ░ ░ ▒   ░ ░  ░   ░   ▒      ░   ░ ░ 
      ░   ░  ░  ░    ░ ░     ░          ░  ░         ░ 
                           ░
 ██░ ██  ▒█████    ██████ ▄▄▄█████▓    ██▓     ▒█████   ▒█████   ██ ▄█▀ █    ██  ██▓███  
▓██░ ██▒▒██▒  ██▒▒██    ▒ ▓  ██▒ ▓▒   ▓██▒    ▒██▒  ██▒▒██▒  ██▒ ██▄█▒  ██  ▓██▒▓██░  ██▒
▒██▀▀██░▒██░  ██▒░ ▓██▄   ▒ ▓██░ ▒░   ▒██░    ▒██░  ██▒▒██░  ██▒▓███▄░ ▓██  ▒██░▓██░ ██▓▒
░▓█ ░██ ▒██   ██░  ▒   ██▒░ ▓██▓ ░    ▒██░    ▒██   ██░▒██   ██░▓██ █▄ ▓▓█  ░██░▒██▄█▓▒ ▒
░▓█▒░██▓░ ████▓▒░▒██████▒▒  ▒██▒ ░    ░██████▒░ ████▓▒░░ ████▓▒░▒██▒ █▄▒▒█████▓ ▒██▒ ░  ░
 ▒ ░░▒░▒░ ▒░▒░▒░ ▒ ▒▓▒ ▒ ░  ▒ ░░      ░ ▒░▓  ░░ ▒░▒░▒░ ░ ▒░▒░▒░ ▒ ▒▒ ▓▒░▒▓▒ ▒ ▒ ▒▓▒░ ░  ░
 ▒ ░▒░ ░  ░ ▒ ▒░ ░ ░▒  ░ ░    ░       ░ ░ ▒  ░  ░ ▒ ▒░   ░ ▒ ▒░ ░ ░▒ ▒░░░▒░ ░ ░ ░▒ ░     
 ░  ░░ ░░ ░ ░ ▒  ░  ░  ░    ░           ░ ░   ░ ░ ░ ▒  ░ ░ ░ ▒  ░ ░░ ░  ░░░ ░ ░ ░░       
 ░  ░  ░    ░ ░        ░                  ░  ░    ░ ░      ░ ░  ░  ░      ░              
```

# shodanHostLookup

This is a simple Python script made for educational purpose only, and during a python training course.
It will query the shodan API for detailed information about a given IP addresse.
It fetches host data using Shodan's REST API, converts the response to JSON, and provides options to display or save the results in various formats

# Features

- Retrieves Shodan host information for a specified IP.
- Supports output in raw text or formatted JSON
- Optionally saves results to a file
- Iterates and prints key details like ports, banners, vulnerabilities, and more for easy readability
- Handles nested data (e.g., service banners under 'data')

# Requirements

- Python 3.x
- Required librairies : requests, json, argparse, os (these are standard or can be installed via
`pip install requests` if needed
- You'll need a valid Shodan API key (sign up at shodan.io for a free or paid account)

# Installation

- Clone or download the script to your local machine
- Ensure Python is installed and accessible
- Install requests if not aready present :

`pip install requests`

# Usage

Run the script from the command line, providing the required arguments

`chmod +x shodanHostLookUp.py`

`./shodanHostLookup.py <host> -k <api_key> [-f <format>] [-o <output_path>]`

# Arguments

- host (required): The IP address to query (e.g., 8.8.8.8).
- -k, --key (required): Your Shodan API key.
- -f, --format (optional): Display format for the data. Options: text (raw API response) or json (pretty-printed JSON). If omitted, only the detailed iterated output is printed.
- -o, --output (optional): Path to save the JSON results as a file. The directory will be created if it doesn't exist.

I'm a noob and this is slop. Please feel free to tell me how to improve it

(real nerds listen to UwU_underground)
