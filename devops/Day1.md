Create a non interactive user 'siva' on server stapp02. 

How to do it?
-  to create a user we can use adduser or useradd <name>
- passwd <name>, then set password

----------------------------------------

- to create a non interactive user we need to use the '-s' flag
- useradd -s /sbin/nologin siva
- passwd siva, then set password

-----------------------------------------

- then check ssh siva@stapp02 -> password -> connection failed
- connection fail because non interactive user.