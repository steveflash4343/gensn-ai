# <h1>Gensn-ai</h1>

<h1>Device/System Requirements 🖥️</h1>

![image](https://github.com/user-attachments/assets/dc5e5e76-9a27-4779-8ac1-f5a77cc3433e)

* Open Your Vps

ssh username@ip

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    ssh username@ip
</body>
</html>

<h1>Pre-Requirements 🛠</h1>

<hr>

<h1>Install Python and Other Tools<h1>

<hr>

* For Linux/Wsl

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  
    sudo apt update && sudo apt install -y python3 python3-venv python3-pip curl wget screen git lsof

</body>
</html>

* For Mac

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    brew install python

</body>
</html>

Check Version

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    python3 --version

</body>
</html>

<h1>Install Node.js , npm & yarn</h1>

* For Linux/Wsl

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash - && sudo apt update && sudo apt install -y nodejs

</body>
</html>

* Install Yarn (linux)

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -

</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list > /dev/null

</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    sudo apt update && sudo apt install -y yarn

</body>
</html>

* Check version (Linux/Mac)

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    node  -v

</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    npm  -v
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    yarn  -v
    
</body>
</html>

<h1 style="text-align:center;">👨🏻‍💻 Start The Node (Linux/Mac)</h1>

* 1️⃣ Clone RL-SWARM Repo

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    git clone https://github.com/gensyn-ai/rl-swarm.git
    
</body>
</html>

* 2️⃣ Create a screen session (vps)

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    screen -S gensyn
    
</body>
</html>


* 3️⃣ Navigate to rl-swarm


<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    cd rl-swarm
    
</body>
</html>

* 4️⃣ Create & Activate a Virtual Environment

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    python3 -m venv .venv
source .venv/bin/activate
    
</body>
</html>

* 5️⃣ Install Left-over dependencies

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    cd modal-login
    
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    yarn install
    
</body>
</html>


<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    yarn upgrade &&  yarn add next@latest &&  yarn add viem@latest
    
</body>
</html>


* 6️⃣ Run the swarm Node 🚀

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    cd ..
    
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    ./run_rl_swarm.sh
    
</body>
</html>

* After Running the Above command it will promt >> <mark>Would you like to connect to the Testnet?</mark> [Y/n] Enter <mark>Y</mark>

* After than it will promt >> <mark>Which swarm would you like to join (Math (A) or Math Hard (B))?</mark> [A/b] Enter <mark>a</mark>

* After than it will promt >> <mark>How many parameters (in billions)?</mark> <mark>[0.5, 1.5, 7, 32, 72]</mark>

👇See below and Choose the model Depends on Your System!



- Qwen 2.5 0.5B                - Recommended 4GB RAM, (1GB DOWNLOAD)
- Qwen 2.5 1.5B                - Recommended 8GB RAM, (4GB DOWNLOAD)
- Qwen 2.5 7B                  - Recommended 16GB RAM, (15GB DOWNLOAD)
- Qwen 2.5 32B (4 bit)         - Recommended 50GB RAM, (35GB DOWNLOAD)
- Qwen 2.5 72B (4 bit)         - Recommended 100GB RAM, (70GB DOWNLOAD)

* After that A web Pop-Up will appear, It will ask u to Login ( if no web pop-up then u have to paste this on ur brower <mark>http://localhost:3000/</mark>

* Now Login With Your Email Id, Enter OTP and back to ur Terminal/Wsl? ( <h1>VPS users check FAQ1</h1> )

* Now U can see A <mark>ORG_ID</mark> On ur Terminal..Save it!

* Now It will promt<mark> Would you like to push models you train in the RL swarm to the Hugging Face Hub?</mark> [y/N] Enter <mark>N</mark>

* After that it will ask u to select 3 choices related to <mark>W&B</mark> Account just enter 3 - wandb: (3) (Don't visualize my results )

* If u have to see your node's details or logs on WANDB WEB then u can choose 1 and enter your api key there, so it will sync your node to wandb web!

![image](https://github.com/user-attachments/assets/abfc9d90-af8c-4526-8d2a-5321c460d803)


Here we go🚀

Its Done ✅

It will Generate Logs Soon🙌

* Detach from <mark>screen session</mark> (vps)
  
Use <mark>Ctrl + A</mark> and then press <mark>D</mark>

* Attach to gensyn Screen to see Logs

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    screen -r gensyn
    
</body>
</html>
  
<h1 style="text-align:center;">🛠 FAQ & Troubleshoot 🛠</h1>

<hr>

<h1>1️⃣ How to Login or access http://localhost:3000/ in VPS? 📶</h1>

<hr>

* Open a new Terminal and login ur vps

* Allow Incoming connection on VPS

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    sudo apt install ufw -y
sudo ufw allow 22
sudo ufw allow 3000/tcp
    
</body>
</html>

* Enable ufw

  <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    sudo ufw enable
    
</body>
</html>

* Install cloudflared on the VPS

  <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    wget -q https://github.com/cloudflare/cloudflared/releases/latest/download/cloudflared-linux-amd64.deb
    
</body>
</html>

  <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    sudo dpkg -i cloudflared-linux-amd64.deb
    
</body>
</html>

* check version

  <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    cloudflared --version
    
</body>
</html>

* Access the Link from your local machine

* ![image](https://github.com/user-attachments/assets/52658529-22ab-48ac-ad6b-f0bdc1c110ae)

* Now follow Login!

* Done!✅
  
<hr>

<h1>MOST IMPORTANT STEP</h1>

<h1>2️⃣ Save your swarm.pem file (for future login)</h1>

* open a wsl window

* If U have to copy this file to your local machine from VPS then Run this command from your local Terminal--

  <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    scp USERNAME@YOUR_IP:~/rl-swarm/swarm.pem ~/swarm.pem
    
</body>
</html>

It will save here in ur Terminal's Root Directory!

<h1>3️⃣ Solution of >> Shutting Down trainer.. at the starting of node!</h1>

❗❗This solution is not for whoes who have the terminated error after the login process!

![image](https://github.com/user-attachments/assets/bb9e8fcf-dece-4f58-88f6-eceabe1419b3)

* install pino-pretty

  <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    yarn add -D pino-pretty
    
</body>
</html>

* Make changes

  <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    rm -rf $HOME/rl-swarm/modal-login/app/layout.tsx
    
</body>
</html>

  <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

    curl -o $HOME/rl-swarm/modal-login/app/layout.tsx https://raw.githubusercontent.com/Mayankgg01/Gensyn-ai-Rl-Swarm_Guide/main/rl-swarm/modal-login/app/layout.tsx
    
</body>
</html>

* Now follow the process of starting the node.
❗❗IMP: if ur node got terminate after the login, Then just Restart your node.

Follow official Docs for more info and Errors!

Thank U! 👨🏻‍💻

Happy Coding 
