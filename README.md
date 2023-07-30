# m4rv4x' caplets
Some custom caplets for `bettercap` made with 💜

## Update caplets from bettercap
```
> sudo bettercap
192.168.0.0/24 > 192.168.0.101  » caplets.update
[sys.log] [inf] caplets downloading caplets from https://github.com/bettercap/caplets/archive/master.zip ...
[sys.log] [inf] caplets installing caplets to /usr/local/share/bettercap/caplets ...
```

## Add custom caplets from bettercap github
```
git clone https://github.com/bettercap/caplets.git
cd caplets
sudo cp *.cap /usr/local/share/bettercap/caplets
sudo bettercap
caplets.show
┌─────────────────────────────────────┬────────────────────────────────────────────────────────────────────────────┬────────┐
│                Name                 │                                    Path                                    │  Size  │
├─────────────────────────────────────┼────────────────────────────────────────────────────────────────────────────┼────────┤
│ wifimon                             │ /usr/local/share/bettercap/caplets/wifimon.cap                             │ 81 B   │
│ blemon                              │ /usr/local/share/bettercap/caplets/blemon.cap                              │ 79 B   │
└─────────────────────────────────────┴────────────────────────────────────────────────────────────────────────────┴────────┘
```

## Run caplets
from parameters :
```
bettercap --iface wlan0 -caplet wifimon
bettercap --iface ble -caplet blemon
```
from CLI : 
```
192.168.0.0/24 > 192.168.0.101  » wifimon
192.168.0.0/24 > 192.168.0.101  » blemon

```
