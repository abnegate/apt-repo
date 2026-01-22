# APT Repository

Debian/Ubuntu packages for abnegate projects.

## Usage

```bash
curl -fsSL https://abnegate.github.io/apt-repo/pubkey.gpg | sudo gpg --dearmor -o /usr/share/keyrings/claude-watchers.gpg
echo "deb [signed-by=/usr/share/keyrings/claude-watchers.gpg] https://abnegate.github.io/apt-repo stable main" | sudo tee /etc/apt/sources.list.d/claude-watchers.list
sudo apt update
sudo apt install claude-watchers
```
