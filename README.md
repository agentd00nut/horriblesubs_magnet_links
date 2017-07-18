# horriblesubs_magnet_links
Dump the magnet links for any horrible subs show for easier downloading.

**NOTE:** Obviously torrenting things you don't own is illegal.  Also don't go pull every mag link for every show off [horrible subs](http://horriblesubs.info/) that'd be dumb.  Use at your own risk blah blah blah not my fault if your isp gets upset blah blah blah.

# Install
Requires [Requests](http://docs.python-requests.org/en/master/user/install/) for python.

Probably works on Python 2.7 but was written with Python 3.6.

`git clone https://github.com/agentd00nut/horriblesubs_magnet_links.git`

`cd horriblesubs_magnet_links`

`chmod +x horrible_links`

`./horrible_links [URL]`

Optionally `cp horrible_links /usr/local/bin/` and then you can just `horrible_links "new-game-2"` from anywhere.

# How to Use

Either pass the full url to a show. `http://horriblesubs.info/shows/new-game-2`
Or just the name of the show as displayed in the url. `new-game-2`

If you don't want the default 1080p you may specify another resolution. `horrible_links "new-game-2" "420p"`

If you didn't know [Deluge](http://dev.deluge-torrent.org/wiki/Download) will automatically add all the magnet links found in a file if that file ends in `.magnet`.  So if deluge is configured to automatically add torrents from `/Volumes/deluge/queue/` we can do something like...

`horrible_links "new-game-2" > /Volumes/deluge/queue/new-game-2.magnet`

And before you know it your deluge client will be downloading all the 1080p torrents for "New Game!!".  Neat.

