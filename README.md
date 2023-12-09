# Tutorial 
Text version! guide how to request aleo badge contributor. don't forget to join our Telegram channel:
- https://t.me/airdropStalkerChannel
## Preparation 🧰
- Leo Wallet https://chromewebstore.google.com/detail/leo-wallet/nebnhfamliijlghikdgcigoebonmoibm
- Github Account

## Get started
if you don't have VPS and linux you can use codespaces as well.
- Open codespaces https://github.com/codespaces
- Use blank template
- Navigate to "terminal" tab

**System upgrade:**
```
sudo apt-get update && sudo apt-get upgrade -y
```
**Install Git & Curl:**
```
sudo apt-get install git-all curl -y
```
**Setting up Cargo:**
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
Choose "1" to proceed installation
```
source "$HOME/.cargo/env"
```
**Clone Aleo Repo:**
```
git clone https://github.com/AleoHQ/leo
```
```
cd leo
```
```
cargo install --path .
```

**Run Leo**
- Go to leo wallet	
- Settings and view private key
- Save it on notepad

```
leo account import <your_private_key>
```
**Create tictactoe Program**
```
leo example tictactoe
```

```
cd tictactoe && leo run new
```

**Push tictactoe to your Github**
```
git init -b main
```
```
git add .
```
```
git config --global user.email "<your_github_email>"
```
```
git commit -m "My first commit"
```

- Create new repo here https://github.com/new
- Repository name: aleo-tictactoe
- Add a README File (checklist)
- Request github token https://github.com/settings/tokens/new
```
git remote add origin https://YOUR-GITHUB-TOKEN@YOUR-GITHUB-REPO
```
```
git remote set-url origin https://YOUR-GITHUB-TOKEN@YOUR-GITHUB-REPO
```

**What you need to change:**
- YOUR-GITHUB-TOKEN = with your github token
- YOUR-GITHUB-REPO = `https://github.com/marepo/aleo-tictactoe` without https://


it should be like this `https://ghp_sd2jkashasj@github.com/marepo/aleo-tictactoe`
```
git push -f origin main
```
- Now let's go to AleoHQ Issue page https://github.com/AleoHQ/leo/issues
- Create New issue
- Choose Leo Contributor Badge

Change title: `[Badge - your_github_username]`

Change description:
```
## 🥇 Leo Contributor Badge

Hi Aleo team! I'm claiming my contributor badge for completing a developer tutorial. 😀

Github Username: <YOUR_GITHUB_USERNAME>
Tutorial Repo: <YOUR_GITHUB_REPO>
Requested badge: TUTORIAL
```
