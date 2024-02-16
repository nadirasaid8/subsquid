# subsquid

[ Photo ]
Run Via Codespace Github | Run Network Test One

➖ Buat Codespace di Github : https://github.com/codespaces
➖ Use Blank Template
➖ Buka Codespace Yang Sudah Jadi (ane open di Vs Code) atau Buka di Browser
➖ Open Terminal

😱 Install Git :

sudo apt update
sudo apt install git

👍 Node Js :

sudo apt install nodejs -y

sudo apt install npm -y

npm install -g npm@10.2.1

👍 Install Docker :

sudo apt-get install ca-certificates curl gnupg lsb-release -y
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io -y

👍 Mainkan

mkdir global-node-packages
npm config set prefix ~/global-node-packages
export PATH="${HOME}/global-node-packages/bin:$PATH"

cd global-node-packages
npm install --global @subsquid/cli@latest

sqd init uniform-load-squid -t https://github.com/subsquid-quests/network-test-one-uniform-load-squid
cd uniform-load-squid
npm ci

di Task Web Subsquidnya Ambil File Key > Klik Get Key > Upload File di Dalem Folder /query-gateway/keys lihat Gambar : https://t.me/bangpateng_group/2572787

😱 Are You Redehh :

sqd get-peer-id

Copy Peer ID Kalian, ke Gateway : https://app.subsquid.io/profile/gateways

Kunci 10 tSQD

sqd up
sqd build
sqd run .

Tunggu Sampe Selesai di Web 100%, Back Sampe Muncul Claim di Task Website Squid

CTRL + C Lalu sqd down

Tutorial Official : https://github.com/subsquid-quests/network-test-one-uniform-load-squid

Noted : Karena Pake Spek Gratisan dari Codespace, Kalo Error Jangan Tereak, Namanya Grates
