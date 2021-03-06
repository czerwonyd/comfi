### Comfi

#### About
Comfi (comfortable configurator) is written to help system administrators manage variety of servers.
Using Comfi you can create kind of alias to commands you use in system. It is fully customizable, but the true power is its config file written in JSON.

#### Features
My goal is to create a tool to use on variety of servers which helps you with:
* remembering all of config files paths (what is a nightmare)
* adding sudo if you are not root
* in cases when we use some repeatable commands an we do not want to remember complicated structures
* if you have an idea it would be great if you could send me some mail

#### Configuration
You can config almost everything in `commands_file` (default: `commands.json`) and `config.py`.

#### How To
For now it is important to add directory you download comfi to your $PATH variable. After that it is able to run systemwide.

Comfi is able to open apache22 main config file with your favourite editor.

For example:

`comfi apache22 config main`

will run suitable command that is assigned to it in commands file depending on OS you are using.

For FreeBSD 9.1 this will run:

`sudo vim /usr/local/etc/apache22/httpd.conf`

And for CentOS 6.5:

`sudo vim /etc/httpd/conf/httpd.conf`

