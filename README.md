# AC-Server-for-Windows
## A quick tutorial for creating a basic Assetto Corsa Server using your Windows PC.

### Locating the Built-in Server of your AC game.
  1. Open up Steam
  2. Go to the Assetto Corsa page.
  3. Hover your mouse icon above the gear icon in the right -> Manage -> Browse Local Files.
  4. Go to the folder "server"
     > Set aside the directoy link of the "server" folder. Sample: C:\WINDOWS-USER\Games\Steam\steamapps\common\assettocorsa\server

### Adding the config.yml and server-manager.exe to the "server" manager
  1. Download this git repository.
  2. Unzip the file
  3. Copy the contents of the "server-manager" into your "server" folder we located earlier.

### Editing config.yml
  1. Open the config.yml file. (Bonus: VScode is great for editing yml files.)
  2. Slowly scroll down until you see the "install_path: assetto".
  3. Remove the "assetto" and replace that with the server directory we set aside earlier. (Sample: C:\WINDOWS-USER\Games\Steam\steamapps\common\assettocorsa\server)
  4. It should look like "install_path: C:\WINDOWS-USER\Games\Steam\steamapps\common\assettocorsa\server"
  5. Then save it.

### Setting up the Server.
  1. Run the server-manager.exe.
  2. It will open up your default browser automatically.
  3. Input the default username and password.
     ```
     username: admin
     password: servermanager
     ```
  4. Create an admin password.
  5. Put your info if you'd like on the next page after creating an admin password.
  6. Navigate to the Server Options tab.
  7. Edit the Name, Password (for joining), and Admin Password (for admin commands in game) as you see fit.
  8. If this will be a private server for you and your friends, scroll down until you see the "Register to Lobby" switch, turn that off.
  9. Scroll to the bottom of the page and click save.

> If you are on static ip. Open up the ports 9600/tcp, 9600/udp, and 8081/tcp both on your Windows PC and router.
> You can now do a quick race or custom race.

### Setting up Radmin VPN.
  1. Download and install [Radmin VPN](https://www.radmin-vpn.com)
  2. Open and turn on the app.
  3. In the "Networks" tab, click on create network.
     ```
     Network Name: John Doe AC Server
     Password: password
     Confirm Password: password
     ```
  4. Click "create".

### Radmin VPN for Friends
  1. Download and install [Radmin VPN](https://www.radmin-vpn.com)
  2. Open and turn on the app.
  3. Set aside your Radmin VPN IP Address. Sample: 22.222.66.111
  4. In the "Network" tab, click "Join Network".
     ```
     Private Network
     Network Name: John Doe AC Server
     Password: password
     ```
       > Make sure to share to them the Network Name and Password you created for your radmin vpn network.

### Editing the Join link of your AC Server for Radmin VPN
  1. After running your Quick/Custom Race.
  2. In the "Live Timings", right click the "join" button and open it on a new tab.
  3. DO NOT CLICK ON THE JOIN/OPEN CONTENT MANAGER BUTTON.
  4. Click the url to edit it. Default Sample: https://acstuff.ru/s/q:race/online/join?httpPort=8081&ip=136.xxx.xxx.xxx
  5. We will edit the last part, which is the public ip the server is running on. We will change it to the Radmin VPN IP Address.
     - It will look like this: https://acstuff.ru/s/q:race/online/join?httpPort=8081&ip=22.222.66.111
  6. Share the new link to your friends. Make sure your friends are running the Radmin VPN app and has joined your network.

# Enjoy Racing!






     
