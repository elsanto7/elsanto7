Install git ffmpeg curl

 sudo apt -y update &&  sudo apt -y upgrade 
 sudo apt -y install git ffmpeg curl
Install nodejs

sudo apt -y remove nodejs
curl -fsSl https://deb.nodesource.com/setup_lts.x | sudo bash - && sudo apt -y install nodejs
Install yarn

curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add - 
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
sudo apt -y update && sudo apt -y install yarn
Install pm2

sudo yarn global add pm2
Clone Repo and install packages

git clone https://github.com/lyfe00011/whatsapp-bot-md
cd whatsapp-bot-md
yarn install --network-concurrency 1
Enter Environment Variables

touch config.env
nano config.env
copy paste lines below (remove SESSION_ID if not needs)

SESSION_ID = Session_Id_you_Got_After_Scan_Dont_Add_This_Line_If_You_Can_Scan_From_Terminal_Itself
PREFIX = .
STICKER_PACKNAME = LyFE
ALWAYS_ONLINE = false
RMBG_KEY = null
LANGUAG = en
WARN_LIMIT = 3
FORCE_LOGOUT = false
BRAINSHOP = 159501,6pq8dPiYt7PdqHz3
MAX_UPLOAD = 200
REJECT_CALL = false
SUDO = 989876543210
TZ = Asia/Kolkata
VPS = true
AUTO_STATUS_VIEW = true
SEND_READ = false
ctrl + o and ctrl + x, To save and exit

start and stop bot

To start bot npm start, To stop bot npm stop

Thanks To
