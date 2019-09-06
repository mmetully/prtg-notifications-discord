# prtg-notifications-discord
Discord notifications from Paessler's PRTG monitoring.

 ___ ___ _____ ___
| _ \ _ \_   _/ __|
|  _/   / | || (_ |
|_| |_|_\ |_| \___|
    NETWORK MONITOR
-------------------
Description: This notification script will send to your Discord Channel  
Parameters:
   [string]$sensor        - the name of the sensor
   [string]$sensorid      - the id of the sensor
   [string]$status        - the status 
   [string]$message       - the message of the sensor 
   [string]$since         - the time since the state is like this
   [string]$lastup        - the time the sensor was up last
   [string]$device        - the device of the sensor
   [string]$sensorURL     - the sensor URL so you can access it directly
   [string]$deviceURL     - the device URL 
   [string]$serviceURL    - the service URL

Requirements
------------------
- [IMPORTANT] PRTG Sample powershell scripts must work - Guide for installing PowerShell based sensors: https://kb.paessler.com/users/my_answers/71356
- A webhook for your channel (see https://support.discordapp.com/hc/en-us/articles/228383668-Intro-to-Webhooks)
- This script located in <PRTG Home directory>\Notifications\EXE\ eg C:\Program Files (x86)\PRTG Network Monitor\Notifications\EXE
- Create a notification template
    -Sample sensor list: -sensor '%sensor' -sensorID '%sensorid' -status '%status' -message '%message' -since '%since' -lastup '%lastup' -device '%device' -sensorURL '%linksensor' -deviceURL '%linkdevice' -serviceURL '%serviceurl'

Modification Resources
The script I adapted this from (MSTeams Notifications) Full installation guide can be found here: https://kb.paessler.com/en/topic/72306#
Webhook documentation: https://discordapp.com/developers/docs/resources/webhook#execute-webhook
Example used to create sample payload: https://birdie0.github.io/discord-webhooks-guide/discord_webhook.html
Other inputs this script can recieve: https://kb.paessler.com/en/topic/373-what-placeholders-can-i-use-with-prtg
Note, In order for the script to function you will need to replace all instances of: REPLACE ME

Version History 
------------------
Version  Date        Notes
1.0      9/06/2019  Initial Release

------------------
(c) 2019 Michael Metully
