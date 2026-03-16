# Install Ubuntu Server
enter (english is selected by default)

done (keyboard is english by default)

Ubuntu Server (full)

make sure Eth0 is pulling DHCP

Enter (no proxy address)

Make sure mirror works and then enter

Use an entire disk

done (don’t touch anything)

user, hostname, user, password, password, Done.

Done, skip ubuntu pro

install openssh

install stable docker then done
#
**Next let’s work on getting basic docker dependencies built.**

    !
    sudo apt update
    sudo apt install -y \
        ca-certificates \
        curl \
        gnupg \
        lsb-release
    !
    sudo mkdir -p /etc/apt/keyrings
    curl -fsSL https://download.docker.com/linux/ubuntu/gpg | \
    sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
    !
    echo \
    "deb [arch=$(dpkg --print-architecture) \
    signed-by=/etc/apt/keyrings/docker.gpg] \
    https://download.docker.com/linux/ubuntu \
    $(lsb_release -cs) stable" | \
    sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
    !
    echo \
    "deb [arch=$(dpkg --print-architecture) \
    signed-by=/etc/apt/keyrings/docker.gpg] \
    https://download.docker.com/linux/ubuntu \
    $(lsb_release -cs) stable" | \
    sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
    !
    sudo apt update
    sudo apt install -y docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
    !
    docker --version
    docker compose version
    !
    #see that both docker and docker compose installed correctly
    !
    sudo systemctl enable docker
    sudo systemctl start docker
    !
    sudo usermod -aG docker USER
    !
