# plex-update

Shell script for updating Plex Media Server under FreeBSD (because it's not possible from the WebUI)

Prerequisite :
- doas  

Add this line to /usr/local/etc/doas.conf  
__permit nopass :GROUP__  
where GROUP is your user group

If you have any issue, and you want to rollback:
- just remove the **/usr/local/share/plexmediaserver** directory
- move **/usr/local/share/plexmediaserver_old** to **/usr/local/share/plexmediaserver**

And restart the service
