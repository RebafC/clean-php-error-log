## parselog
parselog can show lines in the php error
```
WARNING 3310
02-May-2017 02:18 PM
 PHP Warning:  a test error message in /var/www/path/to/php/file/file.php on line 313

PARSE 3311
02-May-2017 02:43 PM
 PHP Parse error:  syntax error, unexpected 'hety' (T_STRING) in /var/www/path/to/php/file/file.php on line 313
```

### Setup
Add the script to your PATH
Set the $log_file variable to the path for your php error_log
Set $linesToTail to the number of lines to look back in your log
### Usage
parselog accepts a variable number of options
```
parselog option1 option2
```
Valid options include:
```
all     show all lines
fatal   show fatal errors
notice  show notices
warning show warnings
parse   show syntax errors
logged  show lines explicitly added to the log
```
