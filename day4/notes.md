Target specific wordlists can be created using tools like: cewl

It is a custom word list generator tool that spiders websites to create word lists based on the site's content. It can follow external links, scan multiple pages, a crawling depth can be specified, it can also extract emails or username identified.

    cewl http://machineIP -w output.txt

    -d specifies depth
    -m min length
    -x max length
    --offsite to follow external links

You can use wfuzz to brute force web applications

wfuzz -c -z file, usernames.txt -z file,passwords.txt -hs "Please enter the correct credentials" -u http://machineIP/login.php -d "username=FUZZ&password=FUZ2Z"

-c display colors
-z load the files az FUZZ substitutes of type file
-hs hide results that contain this string
-u url
-d payload(like it would look in the web request)