# sky-remote
Python module to send remote control commands to a Sky TV box, and receive its power status

#### Simple example
```python
from sky_remote import SkyRemote

remoteControl = sky_remote.SkyRemote('192.168.0.40')

# Just send a command
remoteControl.press('power')

# Now send sequences of commands
remoteControl.press(['channelup', 'record', 'select'])
```

### Check Power Status
```python
print(remoteControl.powerStatus())
```
### Remote control commands
`sky` `power`

`tvguide` or `home` `boxoffice` `services` or `search` `interactive` or `sidebar`

`up` `down` `left` `right` `select`

`channelup` `channeldown` `i`

`backup` or `dismiss` `text` `help`

`play` `pause` `rewind` `fastforward` `stop` `record`

`red` `green` `yellow` `blue`

`0` `1` `2` `3` `4` `5` `6` `7` `8` `9`
