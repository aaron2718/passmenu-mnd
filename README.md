# passmenu-mnd
minimalist dash script for Xorg that uses dmenu to select a password from pass

It can also be used to select a username by modifying line 3 (password -> username)
and line 11 ('1p' -> '2p').
In this case, the pass file should contain the password on the first line and the username on the second line.

When the copied information is pasted into a terminal application, such as neomutt, it may immediately enter upon pasting.
To avoid this behavior, add the following additional code after the second pipe symbol in line 11:
 tr -d '\n'|
