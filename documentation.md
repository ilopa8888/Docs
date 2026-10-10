#LEARNED STUFF:







#CTF CHALLENGES
  1) A little something to be started:  It was easy just checked and fiddled with all the files..
  
MICRO CMS v1....
  I have tried this before on my past account I know the general walkthrough.. 
I found the forbidden page I will use the dit method to go to it again
 and yep found the first flag on forbidden page. Used dirbuster but that makes the site crash when I do a lot of threads .
Found second flag by creating a page that alerts me
Found third flag by using on hover thingy..wait why am i not getting the flag?
OH I used basic sql testing on the edit page and yaay it worked god damn took me a while testing everything
imma go to portswiggers cheat sheet of xss
I had to cheat ffs and use the IMG thingy like why doesn't it work with on hover or body
found all four had to check document.cookie ig it was there


MICROCMS v2 ( I have found one flag I believe before Idk others)

First of all I need access as admin. I know the page is vunerable to sql injection 
I will try to use sql mapper to see further even though I know the structure by cheating before

alr we're testing random data from sql mapper
sum fuzzy test idk 
Also found MySQL dbms 
' ORDER BY 2;-- gives error so we only get returned one column which we need to append some password to..!!!
Password: 
I feel like the structure should be SELECT password from ____ where username =''; because putting ' doesn't crash the internal server
 so how shold wthis world this select wont return anything if se use ' user or some random ass user so we should use UNION to appent one column which we figured ...  just add pass without bother 
like ' union select 'pass' should work finesince se know the columps we get
yep logged in god I hadn't done that before yayy first flag found ig

Saved the session l2session	"eyJhZG1pbiI6dHJ1ZX0.asm_BA.2jdmHw-z2JeIlT1RP7mg-1zto6k"
Iwill do rest later on not in the environment to