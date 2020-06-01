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
      
 ## Output
 
 The program's output looks like this:
 
      34567, 06/01/2020 12:14:53, BBA Front Entry                 , 'Nixon, Richard      ', StandardCredential      , AccessGranted , Credential
      34566, 06/01/2020 12:09:27, WSWW Front Entry                , 'Washington, George  ', StandardCredential      , AccessGranted , Credential
      34565, 06/01/2020 12:07:11, WSWW Front Entry                , 'Adams, John         ', StandardCredential      , AccessGranted , Credential
      34564, 06/01/2020 12:05:52, BBA Front Entry                 , 'Adams, John         ', StandardCredential      , AccessGranted , Credential
      34563, 06/01/2020 11:30:44, BBA Front Entry                 , 'Wilson, Woodrow     ', StandardCredential      , AccessGranted , Credential
      34562, 06/01/2020 11:25:49, BBA Front Entry                 , 'Ford, Gerald        ', StandardCredential      , AccessGranted , Credential
      34561, 06/01/2020 10:40:05, WSWW Front Entry                , 'Washington, George  ', StandardCredential      , AccessGranted , Credential
      34560, 06/01/2020 09:47:47, WSWW Front Entry                , 'Adams, John         ', StandardCredential      , AccessGranted , Credential
      34559, 06/01/2020 09:44:42, BBA Front Entry                 , 'Adams, John         ', StandardCredential      , AccessGranted , Credential
      34558, 06/01/2020 09:43:05, BBA Front Entry                 , 'Lincoln, Abraham    ', StandardCredential      , AccessGranted , Credential
      34557, 06/01/2020 09:34:56, WSWW Front Entry                , 'Washington, George  ', StandardCredential      , AccessGranted , Credential
      34556, 06/01/2020 09:03:03, WSWW Front Entry                , 'Adams, John         ', StandardCredential      , AccessGranted , Credential
      34555, 06/01/2020 08:00:26, BBA Front Entry                 , 'Adams, John         ', StandardCredential      , AccessGranted , Credential
      34554, 06/01/2020 07:42:18, WSWW Front Entry                , 'Adams, John         ', StandardCredential      , AccessGranted , Credential
      34553, 06/01/2020 07:41:52, BBA Front Entry                 , 'Adams, John         ', StandardCredential      , AccessGranted , Credential
      34552, 06/01/2020 07:41:28, WSWW Front Entry                , 'Adams, John         ', StandardCredential      , AccessGranted , Credential
      34551, 06/01/2020 07:40:42, BBA Front Entry                 , 'Adams, John         ', StandardCredential      , AccessGranted , Credential
      34550, 06/01/2020 07:38:41, WSWW Front Entry                , 'Washington, George  ', StandardCredential      , AccessGranted , Credential
      34549, 06/01/2020 07:37:31, WSWW Front Entry                , 'Washington, George  ', StandardCredential      , AccessGranted , Credential
      34548, 06/01/2020 07:36:28, WSWW Front Entry                , 'Washington, George  ', StandardCredential      , AccessGranted , Credential
      34547, 06/01/2020 07:35:13, WSWW Front Entry                , 'Washington, George  ', StandardCredential      , AccessGranted , Credential
      34546, 06/01/2020 07:33:54, WSWW Front Entry                , 'Washington, George  ', StandardCredential      , AccessGranted , Credential
      34545, 06/01/2020 07:33:26, WSWW Front Entry                , 'Washington, George  ', StandardCredential      , AccessGranted , Credential
      34544, 06/01/2020 07:31:52, BBA Front Entry                 , 'Washington, George  ', StandardCredential      , AccessGranted , Credential
      34543, 06/01/2020 06:52:21, BBA Front Entry                 , 'Clinton, Bill       ', StandardCredential      , AccessGranted , Credential
      34542, 06/01/2020 05:45:10, BBA Back Garage                 , 'Bush, Goerge        ', StandardCredential      , AccessGranted , Credential
      34541, 06/01/2020 05:45:01, BBA Back Entry                  , 'Bush, Goerge        ', StandardCredential      , AccessGranted , Credential
   
 ## Implementation
 Developed and tested in Python 3.8.3
