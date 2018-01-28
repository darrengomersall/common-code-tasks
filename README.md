# common-code-tasks
A list of common commands often used across local and servers

# copy ssh keys to server for password-less ssh access
eval "$(ssh-agent -s)"

ssh user@hostname 'cat >> ~/.ssh/authorized_keys' < ~/.ssh/id_rsa.pub


# to run composer on a hetzner server - do inside folder containing composer.json
curl -sS https://getcomposer.org/installer | php -dallow_url_fopen=on

php -dallow_url_fopen composer.phar install
