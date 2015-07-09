# DNS Server on Windows

Attention: This tutorial is old and should be considered depreciated. DEDServer now has a DNS server built in. This has been kept purely for advanced/archival purposes.

This tutorial will help you create a DNS server for unrooted/unjailbroken devices to connect to your DED server. This tutorial will require the following:
  
  * A legal copy of Windows Server 2012 R2
  * Port 53 forwarded to your server (TCP and UDP)

This tutorial will not work on Windows 10, 8, 7, or any other version made for consumer use. You need an actual server operating system to run a DNS server. Amazon AWS and other server hosting companies will provide this for free, so have a look there.

  1. Open 'Server Manager' and click 'Add roles and features' at the top. Click 'Next' 3 times, then check the box next to 'DNS Server'. It may give you a warning about Static IPs, just ignore it. Click Next twice, then click Install. 
  2. Open the charms bar and click search. Search for "DNS" and click the one with the Globe with 6 windows below it. It may be the second option.
  3. In the DNS Manager window, double click forward lookup zones. In Forward Lookup Zones, click Action in the top bar and click New Zone.
  4. Select Primary zone in the wizard that pops up, and click Next. Under zone name, enter [b]gamea.clashofclans.com[/b]. Click next three times, and then finish. 
  **Repeat step 3 and 4 now, replacing gamea.clashofclans.com with game.clashofclans.com. Now you should have two zone files.**
  5. In the sidebar, right click the icon next to your server name. It should look like a grey server icon. Select Properties. Click advanced and check the box next to "Disable recursion". It should be the first on the list.
  6. Back in forward lookup zones, double click gamea.clashofclans.com. In the top bar, click the notebook icon that says "New record". In the dropdown select "Host (A or AAAA)".
  7. In the next page, leave the Host field blank, and change the IP address to your **external** Clash of Clans DEDServer IP Address. This is [b]not[/b] a 192.168.x.x, 127.0.0.1, or 10.x.x.x IP address! It's the public IP address of your server.
  **Repeat steps 6 and 7 with game.clashofclans.com.**
  **If you are using a patching server, see the note at the bottom in red before rebooting!**
  8. Reboot and you're done! Just set your DNS server settings on your phone to your Windows server, and enjoy!
