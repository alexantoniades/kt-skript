# StaffAuth
*A staff authentication script, written for sponge using Kt-Skript in Kotlin*

## Features
- Invite based staff member registration
- SHA-256 password hashing
- Local databases
- Simple command authorisation
- Adds an extra layer of security in case a staff member's account is compromised.

## Examples
Invite a player to register, specifying their role.
```
/staff invite <player> <role>
```
An invite code is generated and stored, the player can either use the invite code to register or click on the chat link.
```
/staff register <invite code>
```
A temporary password is generated and given to player. Their first login is done using their temporary password.
```
/staff login <password>
```
Staff can then change their password using the temporary password.
```
/staff changepassword <old password> <new password>
``` 
If a staff member forgets their old password, the admin can execute:
```
/staff forcechangepassword <player>
```
and a new temporary password is sent to the player.

Once logged-in the mute command can be executed.
```
/staff mute <player> <duration> <reason>
```
