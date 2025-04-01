@echo off

del %programdata%\AnyDesk\*.conf

taskkill /IM Anydesk.exe /F

net stop AnyDesk

net start AnyDesk

start "" "C:\Program Files (x86)\AnyDesk\AnyDesk.exe"
