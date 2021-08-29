# Farsi-Phonetic-Keyboard-Linux
Adding a Farsi/Persian QWERTY Phonetic keyboard layout for Ubuntu similar to MacOS.

# Installation

On ubunto:

1. Open your keyboard folder.

cd /usr/share/X11/xkb/symbols

2. Make a backup of the existing Farsi Layout

sudo cp ir ir.back

3. Copy the contenet of the ir file here to the end of the original layout file.

4) Add the variation to rules/evdev.xml

cd /usr/share/X11/xkb/rules

Open the file evdev.xml and base.xml and Search for Persian, find the existing configItem and add the following lines under it.

        <variant>
          <configItem>
            <name>qwerty</name>
            <description>Persian (QWERTY)</description>
          </configItem>
        </variant>

5) Reboot
