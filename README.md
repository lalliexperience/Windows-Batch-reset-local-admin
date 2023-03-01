# Windows-Batch-reset-local-admin

```
REM Delete the user if it exists
net user /delete localuser

REM Add a new user and set password
net user /add localuser qwe123
net accounts /MaxPWAge:unlimited

REM Add this user to administrators group
net localgroup administrators localuser /add

```
