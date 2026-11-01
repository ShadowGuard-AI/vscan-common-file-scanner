# vscan-common-file-scanner
A command-line tool that checks for the existence of common configuration files, backups, or log files at specified paths or directories on a target web server by sending HTTP HEAD requests. - Focused on Lightweight web application vulnerability scanning focused on identifying common misconfigurations and publicly known vulnerabilities through header analysis, default credentials testing, and basic HTML scraping for vulnerable components. Does not include brute-forcing or invasive testing.

## Install
`git clone https://github.com/ShadowStrikeHQ/vscan-common-file-scanner`

## Usage
`./vscan-common-file-scanner [params]`

## Parameters
- `-h`: Show help message and exit.
- `-u`: Target URL (required).
- `-w`: Path to a wordlist file. A built in default list, `common_paths.txt`, ships in this repo and is used when `-w` is not given. An operator supplied list overrides the default. A run naming a wordlist file that does not exist fails with status 1.
- `-o`: Output file to save the scan results.
- `--timeout`: Timeout for HTTP requests in seconds. Default is 5 seconds.
- `--verbose`: Enable verbose logging.

## License
Copyright (c) CY83R-3X71NC710N
