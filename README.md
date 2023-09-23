# dirobash-fortunes

Fortune files for posts to dirobash


To include fortune files beside default files, copy `dirobash` and `dirobash.dat` to `/usr/share/games/fortune/`


To generate the fortune files (`dirobash` and `dirobash.dat`):

1. run `scrape-dirobash`
2. open `dirobash-entries` with a text editor and perform the following substitution
    `:%s/\n  \(\S\)/%\n\1/g`
3. save the modified file as `dirobash`
4. run `strfile -c % dirobash dirobash.dat`
