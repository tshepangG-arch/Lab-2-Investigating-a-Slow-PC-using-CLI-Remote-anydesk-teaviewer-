# Lab-2-Investigating-a-Slow-PC-using-CLI-Remote-anydesk-teaviewer-
assisted a 2nd year student from TUT in troubleshooting their slow pc using anydesk

##Used powershell(Get process) for this process 
-command ran: Get-Process | Sort-Object WorkingSet -Descending | Select-Object -First 5 Name,Id,WorkingSet
-the command helped me to see the top 5 processes that uses a lot of ram
-chrome appeared 4 times.confusion stroke because,they only had 1 chrome open
-i asked chatgpt it turns out Chrome uses a multi-process architecture,which means Chrome runs many small processes instead of one big one.even open tabs counts.
-i extended the list to 10(-command ran 'Get-Process | Sort-Object WorkingSet -Descending | Select-Object -First 10 Name,Id,WorkingSet) more and more chrome extensions 

##solution 
-i closed the unused tabs(almost 60)

##conclusion 
-The pc became better.Also,The other problem was limited storage. 

