# Crontab
How to use Crontab

1. How to edit your own crontab file

    crontab -e
    
2.show current all crontabs
    
    crontab -l
    
 # Crontab file
 
![crontab](https://user-images.githubusercontent.com/47558327/145251444-8d1ef4ea-491d-4ce5-9839-e2cc025336fb.png)


# Example - 

1). Everyday at 2.00 a.m

    0   2   *   *   *
    
2). 3.30 p.m on the first of every month

    30  15  1   *   *
    
3). 15 minuts after mid night everyday

    15  10  *   *   *
    
4). 2 p.m on week days

    0  14  *   *   1-5
    
5). Run Every 15 minuts 

    */15  *  *   *   *

6). Run every hour

    0   *   *   *   *
    
6). Run at every 3 hours

    *   */3   *   *   *
    
# you can use https://crontab.guru/ to verify your cronjobs


Remove All cronjobs
    
    crontab -r

-----------------------------------------------------------------

example -> create directory at 10.30 am using bash script

    10 22 * * * ./cron1.sh

-------------------------------------------------------------------
cronsh1.sh bash script file --->

#!/bin/bash

mkdir testdirectory


