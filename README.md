# Prerequisites

- Hetzner Account
- Github Account

## Step 1 - Generate SSH Keys

- Run command "ssh-keygen -t ed25519" in terminal

## Step 2 - Hetzner Project

- Select ``Console` and create a new Project

### SSH-Key

- Select `Security` and add a SSH-Key. Copy the whole content of the id_ed25519.pub file into the input field

### Server

- Select `Server` and add a Server.
- Choose a Server-type and location.
- For a Image klick on `Apps` and select Docker CE.
- Add yor SSH-Key and scroll down `Name`.

### Firewall 

- Klick on the new Server and select Tab `Firewalls`. Then `Create Firewall`.
- The presets can stay. Just add one new incoming-rule with port `3000`. Then click `Create Firewall` again.

## Step 3 - Connect to Server via SSH

- Open the Terminal and type `ssh root@<Server-IP>`

## Step 4 - Install Dokploy

Run `curl -sSL https://dokploy.com/install.sh | sh` in the Terminal