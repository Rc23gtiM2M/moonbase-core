OPTS+=" --rundir=/run \
        --dbdir=/var/lib/dhcpcd" &&

OPTS+=" --libexecdir=/usr/lib/dhcpcd" &&

default_build &&

# Set Options in /etc/dhcpcd.conf
# Disable ip4vall
echo noipv4ll >> /etc/dhcpcd.conf
