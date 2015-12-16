# Personal server built with docker

A few Ansible roles to build a server with cool images.

To install the correct packages and create the docker user.

    ansible-playbook prepare.yml

To install all the containers.

    ansible-playbook install.yml

## Additional information

### Shipyard

Credentials: admin/shipyard

### Owncloud

After run, need to set this variable into Owncloud's config.php.

    'filesystem_check_changes' => 1,

### Deluge

Credentials: admin/deluge

Need to change the download destination folder to `/downloads`.

### Plex

When first connected to Plex server, need to set the manual port to `32400` to allow remote connections.