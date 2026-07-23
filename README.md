![Thor suite image](https://github.com/CraftKontrol/Thor-Suite-for-Max4Live/blob/main/Images/ThorSuite.png?raw=true)
# Thor suite for Max4Live
Thor is a modular suite of OSC plugins
(require Max/Msp 8.0 or higher)

with a full set of listeners: dynamic, midi, transport,
spectrum, frequency, clip names
and a powerfull OSC sender allowing up to 8 IPs.

Thor suite is designed to be modular, and allow the user to make it’s own system. The transport device allows to send all synchronisation data to the third party software. Bars, beats, tempo and ticks.

Thor allows to make 8 tracks fully monitored with midi, frequency and dynamic, 8 tracks with tracking of clip names and a single spectrum analyser on the master, with a minimum latency over the network.

---

I have designed Thor for my own usage in live shows, with the objective to have a full control on a third party visual software via OSC messages throug a ethernet connexion. 

The listeners can be used in standalone or remote mode. The stand alone mode send the data via OSC directly from the device. Usefull for litlle projects. The remote mode, allows to send all the data to the master device witch send the data to several IP’s. Ideal for big projects.

Thor suite is designed to be modular, and allow the user to make it’s own system. 
The transport device allows to send all synchronisation data to the third party software. Bars, beats, tempo and the most important for me, the ticks.

Thor allows to make 8 tracks fully monitored with midi, frequency and dynamic, 8 tracks with tracking of clip names and a single spectrum analyser on the master, with a minimum latency over the network.
    

## Transthor
![Transthor image](https://github.com/CraftKontrol/Thor-Suite-for-Max4Live/blob/main/Images/Transthor_Usage.png?raw=true)

Transthor is a live transport listener.
It uses the Live Object Model to watch
the live beat, bars and ticks.

### Usage:
Transthor is an audio effect.
Drop it anywhere.

Instances max : 1

## Midithor
![Midithor image](https://github.com/CraftKontrol/Thor-Suite-for-Max4Live/blob/main/Images/Midithor_Usage.png?raw=true)

Midithor is a simple midi note analyser.
It sends the last played note, without velocity.

### Usage:
Midithor is a midi effect.

Drop it on a desired midi track.

Instances max : 8

## Freckthor
![Freckthor image](https://github.com/CraftKontrol/Thor-Suite-for-Max4Live/blob/main/Images/Freckthor_Usage.png?raw=true)

Frecktor is a frequency analyser.

It’s based on a fundamental spectral estimation.

### Usage:
Freckthor is an audio effect.

Drop it on a desired track.

Instances max : 8

## Dynathor
![Dynathor image](https://github.com/CraftKontrol/Thor-Suite-for-Max4Live/blob/main/Images/Dynathor_Usage.png?raw=true)

Dynathor is a dynamic audio analyser.

It sends a numeric value of the volume.

### Usage:
Dynathor is an audio effect.

Drop it on a desired track.

Instances max : 8

## Clipthor
![Clipthor image](https://github.com/CraftKontrol/Thor-Suite-for-Max4Live/blob/main/Images/Clipthor_Usage.png?raw=true)

Clipthor is a clip name listener.

It uses le Live Object Model to watch
the name of a played clip.

Can be used in string or numeric mode with a spcace between scene and cue.
(MyScene 01, or 01 05, or 01 MyCue)

### Usage:
Clipthor is an audio effect.

Drop it on a desired track.

Instances max : 8

## Speckthor
![Speckthor image](https://github.com/CraftKontrol/Thor-Suite-for-Max4Live/blob/main/Images/Speckthor_Usage.png?raw=true)

Speckthor is a 32 bar spectrum analyser.

It’s based on a classic FFT.

### Usage:
Speckthor is an audio effect.

Drop it on desired track or master.

Instances max : 1

## Masthor
![Masthor image](https://github.com/CraftKontrol/Thor-Suite-for-Max4Live/blob/main/Images/Masthor_Usage.png?raw=true)

Masthor is the main OSC sender.

It allows to send over 8 distant machines.

### Usage:
Masthor is an audio effect.

Drop it anywhere.

Instances max : 1

## Checkthor
![Checkthor image](https://github.com/CraftKontrol/Thor-Suite-for-Max4Live/blob/main/Images/Checkthor_Usage.png?raw=true)

Checkthor is a monitor and debugger

for all messages send by thor.

### Usage:
Checkthor is an audio effect.

Drop it anywhere.

Instances max : 1