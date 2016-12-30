Introduction

Conky configs & setup instructions.

Installation

These configs require conky (I know that's a bit obvious, but you know... users).

% sudo apt-get install -y conky

Configuration

The conky config files here, are just examples & you may want to edit them before use.

% cp -v .conkyrc_Acer_Aspire_One ~/.conkyrc

Setup Autostart

Run the following, to make conky run on login.

% echo -e '[Desktop Entry]\nType=Application\nExec=sh -c "sleep 10; conky;"\nName=Conky\nComment=Autostart conky at login' | tee > ~/.config/autostart/conky.desktop
