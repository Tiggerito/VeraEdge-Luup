# VeraEdge-Luup
My home automation scripts

references to good stuff:
http://wiki.micasaverde.com/index.php/Luup_Intro 
http://wiki.micasaverde.com/index.php/Luup_Variables
http://wiki.micasaverde.com/index.php/Luup_Scenes_Events 

PLEG. I first got things working with this:
http://forum.micasaverde.com/index.php/topic,21603.0.html 

Log File Analysis
==================
http://wiki.micasaverde.com/index.php/Logs 

Login via PuTTY (linux) - note: right click seems to be paste
Enter IP of Vera
root
your veras wifi password

To see logs...
cd /var/log/cmh
tail -f LuaUPnP.log

Ctrl C to stop
Expect logs not to be instant

Can filter logs with grep ocmmands...
tail -f LuaUPnP.log | grep "^04\|^08"

tail -f LuaUPnP.log | grep "sl_CentralScene"