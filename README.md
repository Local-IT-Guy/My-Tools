This is a PowerShell script designed to loop a basic 'ping' to each IP listed in a .csv file and output the status of the connection into the same or new (same if the date is the same, new if it isn't) .csv file. 

The resulting .csv can be screened for status changes. Status 'changes' are determined by the notes. No notes would simply mean the device was previously 'up', and as recommened; applied notes would mean it was previously 'down'. 

Using this logic, one can format the .csv into a table with headers and save it as a (.xls) Excel doc to filter for changes or more specific statuses. Any 'blank' notes with an 'up' status, would mean the devices are up as intended. Any 'down' without notes, would mean it had went down since the last scan. 

Here you would add notes to identify the downage and/or why it is down. Inversely, any 'up' status with a note will mean that it is back up after having been previously down. Here you can remove the notes. 

After screening and updating any notes, you will need to clear the status column to blank cells and remove the header. Save this version as a .csv again in the orginal location and it will serve as the next scan's database.  

Saving the Excel version in a different location is a great way to retain a record or to share as a report.

*This code is pending edits to incorporate Excel instead of .csv to better automate scan reports.*
