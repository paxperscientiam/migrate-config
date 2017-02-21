This is not a script...yet!!

This extracts the deprecated variables (stored in migrate.txt) from `old/_user-settings`.
````
git grep -F -f migrate.txt -h old/_user-settings.scss | sed 's/:.*//'
````

or...
````
git grep -F -f migrate.txt -h old/_user-settings.scss | cut -d: -f1
````
