# Explanation on how to kill a terminal (pycharm terminal running on another place )

n the terminal type:

``` 
sudo lsof -i -P | grep LISTEN | grep 5000
```
Then 
```
kill #port you will see in the results
```
Explanation:
```
lsof stands for "list open files," and is a command that displays a list of all open files in use by the system
```
grep is a command that searches for a specified pattern in a file or stream of output.

So, the full command is telling the system to list all open network connections, filter the results to show only those that are listening on port 5000, and display the output to the user.
