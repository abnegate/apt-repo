# APT Repository

Debian/Ubuntu packages for public projects.

## Usage

```bash
curl -fsSL https://abnegate.github.io/apt-repo/pubkey.gpg | sudo gpg --dearmor -o /usr/share/keyrings/claudear.gpg
echo "deb [signed-by=/usr/share/keyrings/claudear.gpg] https://abnegate.github.io/apt-repo stable main" | sudo tee /etc/apt/sources.list.d/claudear.list
sudo apt update
sudo apt install claudear
```
