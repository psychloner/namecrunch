# namecrunch
Bash script for compiling usernames for enumeration

Usage:
-f (to provide path to a list of first names)
-l (to provide path to a list of last names)
-d (to provide a domain name to append to username iterations)

Example:
./namecrunch -f path/to/firstname -l path/to/lastname -d example.com

Development notes:
1. For generating an output file, the user is provided an option to first delete a file with the same name. When this option is selected, the deletion happens regardless of successful execution of the script.
2. A user should have the option to run the script without prompts (single-line command). This would require an output argument (-o?) and an argument passing the naming convention (ex. --firstname.lastname).
3. A user should also be able to provide standard input strings as an option, separated by commas (ex. ./namecrunch -l Jones,Smith)
