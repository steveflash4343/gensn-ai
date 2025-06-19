# gensn-ai


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


