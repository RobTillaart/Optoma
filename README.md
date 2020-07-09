
# printHelpers

Arduino library to control Optoma W305ST beamer over RS232.

## Description

The Optoma library contains functions that help to controlthe beamer from 
an Arduino. 

The library is tested with an UNO and an Optoma W305ST Beamer. 
The commands can work on other Optoma Beamers 

Command structure
```
    ~XXnnn parameter

    ~        start command
    XX       2 digit ID
    nnn      command can be up to 3 char/digit
    space    space
    param    parameters, depend on command
    \r       end command
```

## Interface

The following functions are implemented:

- **Optoma(HardwareSerial = Serial)** constructor, default uses Serial, 
other HW or SW Serial are possible.
- **init(ID, baudrate)** default baudrate = 9600.  
The ID is used to address a specific beamer.
In theory one could have multiple beamers on one RS232 port (never seen or tested)
- **switchOn()** idem
- **switchOff()** idem
- **increaseVKS()** VKS - Vertical KeyStone
- **decreaseVKS()**

## Future

- More functionality will be added on a need to basis.
- Create examples.

## Operation

Straightforward

