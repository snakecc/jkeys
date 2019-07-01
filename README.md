# jkeys
Automatically exported from code.google.com/p/jkeys


Translate joystick axis/buttons to xserver key pushes
Note: You will need to install python-xlib and python-pygame first

For this, in Ubuntu:
```shell
sudo apt-get install python-xlib python-pygame
```

A lot of linux games dont have joystick support so this little app will map you joystick buttons/axis to key presses

You run a game or an app by using this command:
```shell
./jkeys example-config.joy gameprogram
```
Where example-config.joy is a simple xml file with the key mappings like so
Code:
<config>
    <joystick id="0">
        <axis number="0" low="Left" high="Right" />
        <axis number="1" low="Down" high="Up" />
        <button number="0" key="Space" />
        <button number="1" key="Return" />
        <button number="2" key="a" />
        <button number="3" key="b" />
        <button number="4" key="c" />
        <button number="5" key="d" />
        <button number="6" key="z" />
        <button number="7" key="x" />
        <button number="9" key="Escape" />
        <button number="10" key="p" />
    </joystick>
</config>

It should allow for multi axis any number of buttons and multiple joysticks.
