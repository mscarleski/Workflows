Task

This sample pings yahoo.com every 20 seconds, parse and log the result.  Of course, in case of error (loss > 0) it is simple to add an email activity to announce you about it.

Steps
1. Open cmd.exe
2. Type into cmd.exe "ping www.yahoo.com"
3. Wait 20s
3. Extract the result using Get Text
4. Parse the result string with Regex
5. Log the result
6. Clear the console
7. Return to step 2   
