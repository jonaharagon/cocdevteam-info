# Installing DEDServer

This is a detailed guide on how to install the DEDServer software.

## Getting Started

### Prerequisites
 
  * [Java 8](http://www.java.com/en/) or another JRE (OpenJDK, ...)

### Installation

  1. Download the latest copy of DEDServer from [cocdevteam.info/latest.html](https://cocdevteam.info/latest.html).
  2. Unzip its contents to a folder.
  3. Open `config.dedserver` with your favorite text editor.
    1. Change the `startingGold`, `startingElixr`, `startingDarkElixr`, and `startingGems` values to their desired values. This is how many resources your players will start out with.
    2. All other configurations are purely technical, and don't need to be changed.
      * Note: You may need to change `h2` to `h2-server` in saving methods if you want to use a GUI or other program that requires API access.
  4. Double click `DEDServer_release.jar`. The server will initialize. You can now connect to your server.
 
## Connecting

### Android

  1. Download and install [Hosts Editor](https://play.google.com/store/apps/details?id=com.nilhcem.hostseditor&hl=en) from the Google Play Store
  2. Open the app, and press the **+** button at the top of the page.
    1. In the **IP Address** field, type the IP address of the computer DEDServer is running on.
    2. In the **Hostname** field, type `gamea.clashofclans.com`.
  3. Open Clash of Clans and you should be connected. In some cases you may need to reinstall Clash of Clans before it connects.
  
### iOS

  1. Open `/etc/hosts` with a file browser like iFile.
  2. Add a new line at the bottom of the page: `SERVER_IP game.clashofclans.com` (Replacing `SERVER_IP` with the IP address of the computer DEDServer is running on).
  3. Open Clash of Clans and you should be connected. In some cases you may need to reinstall Clash of Clans before it connects.

## Opening your server to the public

Now that you have a server, you might want other people to connect!

  1. In your router, port forward port `9339` to your computer. 
    * Note: This process is different for every router, we cannot provide support. Try googling "`your router model` port forwarding"
  2. Browse to [ipchicken.com](http://ipchicken.com/) and note your IP address.
  3. Give your IP address to any users that want to join. They should enter that IP in their hosts file.
 
## Notes

We are not providing support for this at cocdevteam.info. You can try asking for support at the [CoC Developers Forum](http://cocdevteam.com/forum/).

We are not responsible for any damage caused to any device, account, server, etc.

Some portions of this webpage were originally located at [ultrapowa.info](https://ultrapowa.info).
