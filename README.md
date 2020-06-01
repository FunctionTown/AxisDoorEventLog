# AxisDoorEventLog
Get an event log from an AXIS A1001 Network Door Controller using the VAPIX API

## Usage
Set the username, password, and network address of your door controller as environment variables 

    AxisAddress
    AxisUser
    AxisPassword
    
or specify them on the command line 

    usage: doorcontrol.py [-h] [--fromDate FROMDATE] [--ipAddress IPADDRESS] [--user USER] [--password PASSWORD]

    optional arguments:
      -h, --help            show this help message and exit
      --fromDate FROMDATE   event date in YYYY-MM-DDTHH:MM:SS format
      --ipAddress IPADDRESS
                            ip address or DNS name of controller
      --user USER           username
      --password PASSWORD   password
      
 ## Implementation
 Developed and tested in Python 3.8.3
