# LightBeam

A battery-powered RGB LED light tube.  Built on [My Bike's Got LED](https://mcqn.com/ibal234)

![Image shows an illuminated bollard fitted to a rubber stand, it is showing a chasing rainbow effect](ibal251-bollard.gif)


It was initallly designed for an active travel game for a local school. In the game participants had to deliver parcels by bike to bollards placed around the playground. Then the game controller then activated the check function. Parcels correctly delivered would show as green bollards, incorrectly delivered parcels as red. A seconf game, 'Red light, green light' was also created were the controller could switch between two light modes to indicate if the cyclists should move or pause. More details of this project can be found on the [catalouge page for lightbeam](https://mcqn.com/ibal251/)



This repositry contains the hardware and software for these games. The structure is;

### Bollard

The [Bollard](https://github.com/mcqn/lightbeam/tree/main/bollard) folder contains the software running on the My Bike's got LED board. It is developed with the ESP-IDF framework and manages Bluetooth communication and the data sent to the LEDS

### Controller

The [Controller](https://github.com/mcqn/lightbeam/tree/main/controller) folder contains the software running on [Micro:bit](https://microbit.org/) devices that are used to run the game and send instructions to the bollards. It is developed in Zephyr and sends control messages over Bluetooth.

### Parcels

The [Parcels](https://github.com/mcqn/lightbeam/tree/main/parcel) folder contatians the software running on [Micro:bit](https://microbit.org/) devices that are used as parcels in the game. It is developed in Zephyr and transmits it's identity using Bluetooth GATT services

### Physical

The [Physical]() folder contains the 3d models for the 3d printed components needed to bake the physical Lightbeam. The files are created in [Freecad](https://www.freecad.org/) The README for this folder also contains instructions to assemble the versions of Lightbeam.










