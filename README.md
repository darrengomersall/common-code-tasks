# common-code-tasks
A list of common commands often used across local and servers

# copy ssh keys to server for password-less ssh access
eval "$(ssh-agent -s)"
ssh user@hostname 'cat >> ~/.ssh/authorized_keys' < ~/.ssh/id_rsa.pub
