# 32.Channel.Amp
  
-----------------  
## Table of Contents
- 🔲 [Tile Boards]  
  - [Single Channel Boards]  
  - [Digi-Key Component List]
  - [Schematic]  
  - [Test Board]  
  - [Cell Board]  
- 🔲 [32 Cell Channel Receiver Board]  
  - [Cell Receiver Board]
  - [Cell Tester]
  - [Capacitance Fix]  
- 🔲 [Resources]  
  - [ Board Reference ]  
  - [ Amp Details ]  
  - [ Expected Connector ]  
  - [ Connections ]

----------------
## 🔲 ::: Tile Boards :::  
### :: Single Channel Boards ::  
**: Layers :** 4 Layer PCB Board  [ Power Layer , Power Ground , Signal Ground, Signal Layer ]  
<img src="./z.ReadMeImages/BoardStackUp.png" width="75%">  
  
### : Component List :  
: Diodes :  
[ 1N4148W ](https://www.digikey.com/en/products/detail/smc-diode-solutions/1N4148W/6022450)  
[ MMSZ5236B-7-F ](https://www.digikey.com/en/products/detail/diodes-incorporated/MMSZ5236B-7-F/717790)  
: Transistors :  
[ MMBT3904 ](https://www.digikey.com/en/products/detail/anbon-semiconductor-int-l-limited/MMBT3904/17284363)  
[ MMBT3906 ](https://www.digikey.com/en/products/detail/nte-electronics-inc/MMBT3906/11652283)  
: Capacitor :  
[ CL10A106MP8NNNC ](https://www.digikey.com/en/products/detail/samsung-electro-mechanics/CL10A106MP8NNNC/3887529)  
: Resistors :  
[ RC0402JR-071KL ](https://www.digikey.com/en/products/detail/yageo/RC0402JR-071KL/726408)  
[ RL0510S-4R7-F ](https://www.digikey.com/en/products/detail/susumu/RL0510S-4R7-F/567247)  
: Cremat Holder :   
[ SMC-1-08-1-GT ](https://www.digikey.com/en/products/detail/adam-tech/SMC-1-08-1-GT/9830825)  
: DSUB Connector :  
[50 D-Sub](https://www.digikey.com/en/products/detail/harting/09665627811/4322749)  
[9 D-Sub](https://www.digikey.com/en/products/detail/te-connectivity-amp-connectors/2311765-1/7794751)  

### : Schematic :  
<img src="./z.ReadMeImages/Schematic.png" width="60%">  
  
### :: Test Board ::  
<img src="./z.ReadMeImages/TestBoard1.png" width="15%"> <img src="./z.ReadMeImages/TestBoard2.png" width="15%"> <img src="./z.ReadMeImages/TestBoard3.png" width="15%">  
Dimensions :  20 x 60 mm  

### :: Cell Board ::  
<img src="./z.ReadMeImages/Cell1.png" width="16%"> <img src="./z.ReadMeImages/Cell2.png" width="15.5%"> <img src="./z.ReadMeImages/Cell3.png" width="16%">  
Dimensions : 20 x 40 mm  


-------------------
## 🔲 :: 32 Cell Channel Receiver Board ::
<img src="./z.ReadMeImages/32ChannelPreview3.png" width="45%">  <img src="./z.ReadMeImages/32ChannelPreview.png" width="45%">   
File Dimensions : 177 x 152 mm  
  
  
### : Cell Receiver Board :  
<img src="./z.ReadMeImages/32ChannelPreview2.png" width="60%">   
Dimensions : 142 x 152 mm   
   
### : Cell Tester :  
Cell Tester allows for easy and quick cell testing.  
<img src="./z.ReadMeImages/CellTester.png" width="25%">  

  
### : Capacitance Fix :  
Different trace length create variances on capacitance. To correct this variance the width of each trace has been modified using the following method.  
<img src="./z.ReadMeImages/CapacitanceDemo.png" width="80%">  

- [(Vertical Aspect) In reference to the height of the trace and what it contributes to the total capacitance and why I neglected this measurement]  
   - [The distance between the side of the traces and the adjacent ground plane are equivalent on all]  
   - [The distance between the side of the traces and the adjacent ground plane is greatly larger than the height of the traces]  
     - [Conclusion: There is variance in the side capacitance but it's contribution is extremely small compared to the next argument]  
- [(Horizontal Aspect) In reference to the width of the trace and what it contributes to the total capacitance]  
   - [Since I used ratios, the surface area of each horizontal plane will remain equivalent]  
   - [The surface area of this aspect is greatly larger than the vertical contribution]  
   - [The distance between this trace and the ground layer is equivalent on all traces]  
     - [Conclusion: The horizontal aspect is equivalent on all traces and it is greatly larger than the vertical contribution]  

: Excel Calculator : (Included in the Repository)    
<img src="./z.ReadMeImages/Capacitance.png" width="110%">    
  
## 🔲 ::: Resources :::    
:: Board Referenced ::  
[CR-150-R5](https://www.cremat.com/CR-150-R5.pdf)  
  
:: Amp Details ::  
[CREMAT CR-11X](https://www.cremat.com/CR-110-R2.1.pdf)  
  
:: Expected Connector ::  
[IFDGG501056AX](https://www.lesker.com/feedthroughs/instrument-feedthroughs-mpdt-subd/part/ifdgg501056ax)  
  
### :: Connections ::  
###[SMC-1-08-1-GT](https://www.digikey.com/en/products/detail/adam-tech/SMC-1-08-1-GT/9830825)###  
: Drawing :  
<img src="./z.ReadMeImages/PinConnDraw.png" width="60%">  
: Generated Footprint :  
<img src="./z.ReadMeImages/PinConn.png" width="60%">  
  
###[50 Position D-Sub Plug, Male Pins Connector](https://www.digikey.com/en/products/detail/harting/09665627811/4322749)###    
: Drawing :  
<img src="./z.ReadMeImages/CONN50Draw.png" width="60%">  
: Generated Footprint :  
<img src="./z.ReadMeImages/CONN50.png" width="60%">  
