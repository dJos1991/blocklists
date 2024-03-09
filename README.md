# blocklists

# ARCHIVE NOTE:
This repo is archived en will not updated anymore. You can find this project from now on here: https://git.geyskens.eu/sgr5/blocklists 

## Description
These are the most [UT1 blocklists](https://dsi.ut-capitole.fr/blacklists/index_en.php), converted to txt files, so that you can use it in [Pi-hole](https://pi-hole.net/), [Adguard Home](https://adguard.com/en/adguard-home/overview.html) and maybe other dns blocking software (not tested).

## Updates
Every night around 1 A.M. the UT1 list will be downloaded, and converted to TXT files, and then uploaded to this repo.

## How to use
### Pihole
- In Pi-hole admin interface, go to "Adlists" and add the raw files from the txt files (the ones you want to use) in this repo.
- Then go to "Tools" -> "Update Gravity", and click the 'Update' button. *Note: this can take some time, espessially when you download the adult list.*
- You can also run the following command to update the database from a terminal session, or run it as a cron job (Gravity database update will also run every Sunday at night by default)
  `pihole -g`

Other notes:
At this moment (maybe I change this in the feature) there are also IP's in some of the lists from UT1. Pi-hole only blocks domain names, not IP's (obviously :laughing:) You will see notes about that in the Gravity updates, but this is not a problem. Pi-hole removes those IP's from the database. 
