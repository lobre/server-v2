# Personal server built with docker

A few Ansible roles to build a server with cool images.

To install the correct packages and create the docker user.

    ansible-playbook prepare.yml

To install all the containers.

    ansible-playbook install.yml

You can also clean/delete all containers.

    ansible-playbook clean.yml

## Additional information

### Shipyard

Default credentials: admin/shipyard

### Owncloud

After run, set this variable into Owncloud's config.php.

    'filesystem_check_changes' => 1,

### Deluge

Default credentials: admin/deluge

Change the download destination folder to `/downloads`.
Allow remote connections under `daemon` tab.
Enable `Label` plugin.

Add a user in the daemon file (`/config/auth`) and restart the container.

    admin:deluge:10

### Plex

When first connected to Plex server, set the manual port to `32400` to allow remote connections.

### Couchpotato

Add download client.

    username: admin
    password: deluge
    host: lobr.fr:58846

### Sonarr

Add download client.

    host: lobr.fr
    port: 8112
    password: deluge

### Headphones

### Minecraft

Default credentials: admin/password