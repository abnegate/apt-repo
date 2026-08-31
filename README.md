# APT Repository

Debian/Ubuntu packages for public projects.

## Usage

```bash
curl -fsSL https://abnegate.github.io/apt-repo/pubkey.gpg | sudo gpg --dearmor -o /usr/share/keyrings/abnegate.gpg
echo "deb [signed-by=/usr/share/keyrings/abnegate.gpg] https://abnegate.github.io/apt-repo stable main" | sudo tee /etc/apt/sources.list.d/abnegate.list
sudo apt update
sudo apt install magents
```

The same repository also publishes `claudear`. Existing `claudear.gpg` keyrings remain valid; they use this key.
