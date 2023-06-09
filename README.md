# Fuzzer

 Fuzzer is a Python script that can be used to fuzz a web application by discovering directories on a target URL. It takes a text file containing directory paths as input and makes HTTP requests to each directory, checking for the corresponding status code. The script provides an easy way to discover potential hidden directories on a web server.

## Usage

1. Clone the repository:
`git clone https://github.com/your-username/fuzz.git`

2. Navigate to the project directory:
`cd fuzz`


3. Install the required dependencies (requests library):
`pip install requests`

4. Run the script:
`python fuzz.py <file_path> <target_url> <status_codes>`

- `<file_path>`: The path to the text file containing directory paths (one per line).
- `<target_url>`: The base URL of the target web application.
- `<status_codes>`: Optional - The desired status codes to filter the results (comma-separated).

Example:
**python fuzz.py directories.txt example.com 200,404**

5. The script will display the discovered directories and their corresponding status codes, filtered based on the provided status codes (if any).


