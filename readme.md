API documentation of pyCGM2


## Dependency

 * Python 2.7
 * sphinx
 * ghp-import (see bugfix)




## BugFix


**Bug**  raw date invalid in *ghp-import.py*

bug fix by altering *ghp-import.py*

line 120 #currtz = time.strftime('%z') need to be replaced with currtz = datetime.now(tz.tzlocal()).strftime('%z')

need to import  

  * from datetime import datetime
  * from dateutil import tz
