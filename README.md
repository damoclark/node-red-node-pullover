node-red-node-pushover
======================

This is an **experimental** <a href="http://nodered.org" target="_new">Node-RED</a> node to send alerts via <a href="http://www.pushover.net/" target="_new">Pushover</a>
with image attachment support.

Please [provide feedback](https://github.com/damoclark/node-red-node-pullover/issues) on your experience with this node.  
All things going well, this experimental version will be rolled into the standard Pushover Node as part of the 
standard Node-Red installation.

Install
-------

Run the following command in your Node-RED user directory - typically `~/.node-red`

    npm install damoclark/node-red-node-pullover

Uninstall
---------

To remove this experimental version and replace it with the standard version, run the following command in the same Node-RED user directory

    npm install node-red-node-pushover


Usage
-----

Uses Pushover to push the `msg.payload` to a device that has the Pushover app installed.


Optionally uses `msg.topic` to set the configuration, if not already set in the properties:
 - `msg.device`: to set the device
 - `msg.priority`: to set the priority
 - `msg.topic`: to set the title
 - `msg.attachment`: **to specify an image to attach to message (path as a string or Buffer containing image)**
 - `msg.url`: to add a web address
 - `msg.url_title`: to add a url title
 - `msg.sound`: to set the alert sound, see the [available options](https://pushover.net/api#sounds)

The User-key and API-token are stored in a separate credentials file.

Uses Pushover. See <a href="https://pushover.net" target="_new">Pushover.net</a> for more details.
