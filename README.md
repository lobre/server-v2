# Personal server built with docker

A few Ansible roles to build a server with cool images.

To install the correct packages and create the docker user.

    ansible-playbook prepare.yml

To install all the containers.

    ansible-playbook install.yml

## Additional information

### Shipyard

URL: shipyard.lobr.fr

Default credentials: admin/shipyard

### Owncloud

URL: cloud.lobr.fr

After run, need to set this variable into Owncloud's config.php.

    'filesystem_check_changes' => 1,

### Deluge

URL: torrent.lobr.fr

Default credentials: admin/deluge

Need to change the download destination folder to `/downloads`.

### Plex

URL: plex.lobr.fr

When first connected to Plex server, need to set the manual port to `32400` to allow remote connections.

### Couchpotato

URL: couchpotato.lobr.fr

### Sonarr

URL: sonarr.lobr.fr

### Minecraft

URL: minecraft.lobr.fr

Default credentials: admin/password