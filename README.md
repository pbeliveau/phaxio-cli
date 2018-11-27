# Send faxes from the terminal
Script I wrote while sending fax for clients. It uses phaxio.com (not affiliated
with them). 

## Usage
Bash script to send fax using Phaxio.com service.

### Required options
* a) Path to API file. Must use YAML syntax. (e.g. see 'insert url')
* p) Phone to send the fax to. Need to specify the country code without
     the '+' symbol.
* f) Path to the file to send.
* h) Show this message output.

### Optional
t) Using the '-t' flag will use the 'test' APIs specified in the YAML file.

### Examples
Send a .PDF to a number:

        phaxio-cli -a ~/api.yml -p "12126647665" -f ~/test.pdf

Same thing but using the test APIs:

        phaxio-cli -a ~/api.yml -p "12126647665" -f ~/test.pdf -t

## License
GPLv3
