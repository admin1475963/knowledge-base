# User management

## Create user
```shell
# '*' means that this object must exists until the command

# User: user
# Home directory: /home/user*
# Group: group*
# Supplementary groups: additionalgroup1*, additionalgroup2*
# Login shell: fish*
useradd -d /home/user -g group -G additionalgroup1 additionalgroup2 -s /usr/bin/fish user

# User: user
# Home directory: /home/user
# Group: group* 
# Supplementary groups: additionalgroup1*, additionalgroup2*
# Login shell: fish*
useradd -m -g group -G additionalgroup1 additionalgroup2 -s /usr/bin/fish user

# User: user
# Home directory: /home/user
# Group: user 
# Supplementary groups: additionalgroup1*, additionalgroup2*
# Login shell: fish*
useradd -m -U -G additionalgroup1 additionalgroup2 -s /usr/bin/fish user
```

## Change user
```shell
# Change a primary group
usermod -g new_group

# Add a supplementary group
usermod -a -G new_supplementary_group

# Remove a supplementary group
usermod -r -G old_supplementary_group

# Change home directory
usermod -d /home/new_home

# Change home directory and move to it
usermod -d /home/new_home -m
```

## Delete user
```shell
# delete user, not delete home directory
userdel old_user

# delete user and it's home directory
userdel -r old_user
```

## Create group
```shell
groupadd group
```

## Change group
```shell
groupmod -n old_group new_group
```

## Delete group
```shell
groupdel group
```