# FlexNextBike-research
WIP Research About Flexnest Fitness Bike. This is not affliated to FLexnest brand. Proceed with your own caution.

I have created this repo to share details about Flexnest bike, a fitness brand based in India. They have  3 variants as of now: Lite, Standard, Premium. I have the Standard version where you can  connect to their app on iOS / Android.


## Product Information on Website

• Country of origin: China

• Common or generic name of the commodity contained in the package: Exercise Cycle for home use

• Retail sale price in the form of Maximum Retail Price (MRP) Rs Inclusive of all taxes: Rs 59,999

Site: https://www.theflexnest.com/products/the-flexbike?variant=40096907329699

## Technical Specifications

Net Weight - 31Kg

Gross Weight - 36Kg

Floor Space - 1000 x 510 x1165mm

Carton Size - L1005 x W260 x H945mm

Flywheel Weight - 16.5lb

Max User Weight - 120Kg

Max User Height - 6ft 4in

Max Tablet Size - 11"

Min iOS Version -  iOS 13.4

Min Android Version - Android 10


## Hidden Features

* The Bike runs on a single link Bluetooth Fitness Machine Service (FTMS) Protocol. So it can connect to any BLE-FTMS compatible app. However, cannot connect to Apple Watch since the FTMS protocol is unsupported. Unless Apple comes up with an update to work with FTMS machines which is unlikely since it competes with their gymkit system.
* The Motherboard Firmware is based on a Yesoul Magnetic resistance Spin bike.
* Requires a CR2477N 3V Battery (this is very ineffective for the long run in my opinion). With No physical switch to turn on the machine, it will drain quickly within a couple of months.

## Work arounds for Apple Watch

QDomyos Zwift - https://github.com/cagnulein/qdomyos-zwift

   Initially, developed as a bridge to connect proprietory Exercise Bikes to Zwift. It now supports FTMS protocol too. The Developer @cagnulein is very kind and responds very quicky.

   The Bridge reads your power and cadence value and sends the via a Bluetooth Cycle Power Service (CPS) server to Apple Watch.

   Visualisation:

   Flexnest Bike    ----BLE FTMS---->    QDomyos-Zwift    -----BLE CPS---->   watchos 10



## To Do 

* Alternate battery mod
* Data Dump of BLE service
* Integrate Speed and Distance Natively to watchOS 10 Workouts app



## Notable projects

* https://github.com/ptx2/gymnasticon
* https://github.com/cagnulein/qdomyos-zwift - Virtual Bridge to connect the machine to many services at once
* https://github.com/dbsqp/bluetooth-reebok-57e
* https://github.com/BigJinge/Multi-BLE-Sensor
