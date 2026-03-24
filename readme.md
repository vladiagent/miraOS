hi guys

this is my custom made linux distro based on arch and hyprland, MiraOS. inspired by omarchy, miraos aims to be great for gaming and productivity, without the big hassle (for people who dont want to use the terminal like at all).
with the Illogical Impulse dotfiles, MiraOS is also a plug-n-play distro, with good customizability and ease. (chatgpt didnt help me i swear)

the installation is pretty manual and bad, but what do you expect from a ten year old?

first, you install arch linux using archinstall and kde plasma (MANDATORY, NO OTHER DEs)

additional packages:
kio-admin

fastfetch (optional)

in kde plasma, install all your programs and drivers, that you will use after KDE.
when you are done installing drivers, reboot for the drivers to work properly, then open another terminal and run the following install script:

bash <(curl -s https://ii.clsty.link/get) --- hyprland illogical impulse dotfiles: may also use own dotfiles

when install script is done, im assuming you hate that ugly stock sddm theme. so,

sh -c "$(curl -fsSL https://raw.githubusercontent.com/3d3f/ii-sddm-theme/main/setup.sh)" -- unofficial illogical impulse sddm theme

background directory: admin:/usr/share/sddm/themes/ii-sddm-theme/backgrounds (BACKGROUND FILE MUST BE NAMED BACKGROUND.PNG)

and done! UI installed!
but branding?
fastfetch and os branding in the repo!

for branding:
os-release directory:
/etc/os-release
replace the file with one in repo

fastfetch config directory:
~/.config/fastfetch/config.jsonc
replace the file with one in repo

fastfetch ascii directory:
~/.config/miraos      (new folder)

os logo directory:
/usr/share/icons/hicolor/scalable/apps

done. enjoy MiraOS!
