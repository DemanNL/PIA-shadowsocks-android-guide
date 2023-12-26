# PIA shadowsocks android guide
A how-to guide for using shadowsocks in combination with Private Internet Access VPN.

Download and install the Shadowsocks Android app (https://play.google.com/store/apps/details?id=com.github.shadowsocks)
Make sure you have the PIA VPN app installed (https://play.google.com/store/apps/details?id=com.privateinternetaccess.android)

Open the PIA VPN app and change the following settings using the hamburger menu top left:
- Per App Settings, search for Shadowsocks app and tap it. Make sure it has a red lock icon.
- Goto Settings, protocol and select OpenVPN.
- Goto Settings, protocol and select Transport TCP.
- Goto settings, obfuscation and select Connect via proxy. Tap on Select Proxy-app and choose Shadowsocks app. Set the proxy port to 1080, in order to match the Shadowsocks app.

Now open the Shadowsocks app and tap on the hamburger menu top left. Goto settings and set Service mode to proxy only. Make sure the SOCKS5 proxy port is 1080.

Goto Subscriptions. Tap on the plus icon top right and fill in the following URL:
https://raw.githubusercontent.com/DemanNL/PIA-shadowsocks-android-guide/main/profiles.json

Tap on ok. Now tap on the download icon top right and all the shadowsocks profiles should've been imported.
Go to the hamburger menu top left, tap on Profiles and you should be presented with a list of shadowsock servers.

To start the shadowsocks, select a profile and tap the paper plane icon at the bottom of your screen. After connecting tap the text at the bottom of your screen to test the connection. If this works, open up the PIA VPN app and connect to a VPN server.

If everything went well, the VPN should've started and the PIA VPN app will display a green bar. If you drag down from the notification bar you should see traffic going through both the VPN app and the shadowsock server.

If for some reason the shadowsock servers change or it doesn't pass the connection test. You can  manually create a profile using the information found here:
https://serverlist.piaservers.net/shadow_socks

You can create a profile manually by tapping on the Profile tab, tap the plus icon and select Manual Settings. Now fill in all the information you retrieve from the URL above.
