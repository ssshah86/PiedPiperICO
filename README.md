# PiedPiperICO
A static website built by hugo and hosted on firebase (http://piedpiperico.com) to display the price of PiedPiperCoin (PPC) from HBO's Silicon Valley (http://www.piedpiper.com)

To deploy follow the steps below:

```
$hugo new site NAME
$cd NAME
$git init
$cd themes
$git submodule add THEME
$cd .. #now in main
#edit config.toml in main and change theme to THEME, ensure baseUrl is https://PROJECT.firebaseapp.com
#create PROJECT in firebase
$firebase login
$firebase init
#choose hosting, PROJECT, public directory? (public), single page app? (y)
#check build
$hugo server -w
#edit as desired
$hugo && firebase deploy
```
