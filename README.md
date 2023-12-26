# SSL G-Series Bus Compressor Build

## Step 1: Bypass Caps and IC Sockets 

The bypass capacitors and IC sockets are handled in one pass.  The checklist below is organized
by the area of the PCB where the parts are to be installed. Subsequent sections are organized
slightly differently.

```
    Power 12V
    [ ] CB1
    [ ] CB2
    
    Outside Section
    [ ] CB3 - Lower Right of PCB
    [ ] CB4 - Lower Right of PCB
    [ ] CB5
    [ ] CB6
    [ ] IC1 - 14 Pin IC Socket Lower Right of PCB
 
    Balanced Input / Output L
    [ ] CB7_1 
    [ ] CB8_1 
    [ ] CB9_1 
    [ ] CB10_1
    [ ] IC2_1 - 8 Pin IC Socket
    [ ] IC3_1 - 8 Pin IC Socket
 
    Balanced Input / Output R
    [ ] CB7_2
    [ ] CB8_2
    [ ] CB9_2
    [ ] CB10_2
    [ ] IC2_2
    [ ] IC3_2

    Audio VCA L
    [ ] CB11_1
    [ ] CB12_1
    [ ] CB13_1
    [ ] IC4_1

    Audio VCA R
    [ ] CB11_2
    [ ] CB12_2
    [ ] CB13_2
    [ ] IC4_2

    Filter L
    [ ] CB14_1 - Bypass Cap
    [ ] CB15_1 - Bypass Cap
    [ ] IC5_1

    Filter R
    [ ] CB14_2
    [ ] CB15_2
    [ ] IC5_2

    Sidechain VCA L
    [ ] CB16_1 - Bypass Cap
    [ ] CB17_1 - Bypass Cap
    [ ] IC6_1 
 
    Sidechain VCA R
    [ ] CB16_2
    [ ] CB17_2
    [ ] IC6_2
 
    Meter
    [ ] CB18 - Bypass Cap

    Ratio
    [ ] CB19
    [ ] CB20
    
```

## Step 2: Power Sections

```
    Power 12V
    [ ] U1 7812
    [ ] U2 7912
    [ ] C5 4.7uF BP
    [ ] C6 4.7uF BP

    Power 16V
    [ ] L1 Inductor
    [ ] L2 Inductor
    [ ] C1 2200uF 25v 105c
    [ ] C2 2200uF 25v 105c
    [ ] C3 2200uF 25v 105c
    [ ] C4 2220uF 25v 105c
    [ ] J1 Female XLR-5 Pin (Power Thru)
    [ ] J2 Male XLR-5 Pin (Power In)

    [ ] Perforrm Power Rail Test
      [ ] +16v
      [ ] -16v
      [ ] +12v
      [ ] -12v
```

## Step 3: Control Boards  

```
    Control Board 1: (Threshold, Make-up)

    Resistors
    [ ] R1_CB  4K7
    [ ] R2_CB  22K
    [ ] R3_CB  16K
    [ ] R4_CB  2K7

    Connectors
    [ ] CON2_CB  16-pin Connector
    [ ] CON3_CB  12-pin Connector 

    Potentiometers
    [ ] VR1_CB  B50K Threshold
    [ ] VR2_CB  B50K Make-up

    Rotary Switches
    [ ] SW1_CB  2x6
    [ ] SW2_CB  2x6
    [ ] SW3_CB  2x6
 

    Control Board 2: (Mix) 

    Resistors
    [ ] R5_CB  4K99
    [ ] R6_CB  820R
    [ ] R7_CB  510R
    [ ] R8_CB  220R
    [ ] R9_CB  150R
    [ ] R10_CB  4K99
    [ ] R11_CB  820R
    [ ] R12_CB  510R
    [ ] R13_CB  220R
    [ ] R14_CB  150R

    Capacitors   
    [ ] C1_CB  100U
    [ ] C2_CB  100U 
    [ ] C3_CB  0.15U
    [ ] C4_CB  0.1uU
    [ ] C5_CB  68N
    [ ] C6_CB  0.15U
    [ ] C7_CB  0.1U
    [ ] C8_CB  68N
 
    Connectors
    [ ] CON4_CB  26-pin Connector

    Rotary Switches
    [ ] SW5_CB  2x6
    [ ] SW9_CB  4x3
 
   
    Pushbutton Switch Board
    [ ] SW6_CB  DPDT Switch
    [ ] SW7_CB  DPDT Switch  
    [ ] SW8_CB  DPDT Switch
    [ ] CON6B_CB  4-pin Header

    Miscellaneous
    [ ] Mount pushbutton sub-board
    [ ] Attach terminals to wires
    [ ] Attach wiring harness to IN switch

```

## Step 4: Relays and Misc

```
    Resistors
    [ ] R1_1 2K2 
    [ ] R1_2 2K2 
    [ ] R2  2K2 
    [ ] R3  10K 
    [ ] R4  20K 
    [ ] R5  20K 
    [ ] R6  2K2 
    [ ] R7  20K 
    [ ] R8  20K 
    [ ] R9  10K 
    [ ] R10 100K 
    [ ] R11 100K 
    [ ] R12 360K 
    [ ] R13 2K2 
    [ ] R14 1K 
    [ ] R15 1K 
    [ ] R16 120R 
    [ ] R17 120R 
    [ ] R18 47R 
    [ ] R19 47R 

    Capacitors
    [ ] C7  100uF 
    [ ] C8  100p 
    [ ] C9  3N3 
    [ ] C10 3N3 

    Diodes
    [ ] D1_1 1N4004 
    [ ] D1_2 1N4004 
    [ ] D2  1N4004 
    [ ] D3  1N4004 
    [ ] D11 1N4004 

    Connectors
    [ ] CON1 - 3-pin header - In meter section (lower-left)
    [ ] CON2 - 16-pin header 
    [ ] CON3 - 12-pin header
    [ ] CON4 - 26-pin header
    [ ] CON5 - 4-pin header - Lower middle section 

    Relays
    [ ] U3_1
    [ ] U3_1 
    [ ] U4
    [ ] U5
    [ ] U6  

    ICs
    [ ] IC1 - LF347N
    [ ] IC7 - LF347N

    Perform Relay Test
    [ ] Ensure LF347N are inserted in IC1, IC7
    [ ] Attach compression switch to Con5
    [ ] Attach control board 1 to Con2 and Con3 via ribbon cable
    [ ] Attach control board 2 to Con4 via ribbon cable
    [ ] For Rev 1 boards Mono SC test will fail
      Note: My board is not marked with a revision, and test failed
    
```

## Step 5: Audio Jacks
```
    [ ] J3_1 TRS Jack
    [ ] J3_2 TRS Jack
    [ ] J4_1 XLR Male
    [ ] J4_2 XLR Male
    [ ] J5_1 XLR Female Combo
    [ ] J5_2 XLR Female Combo
    [ ] J6   XLR Female Combo
``` 

## Step 6: Balanced Input / Output and Unity Trim
```
    Left Channel

    Resistors
    [ ] R20_1 4K7
    [ ] R21_1 100R
    [ ] R22_1 4K7
    [ ] R23_1 100R
    [ ] R24_1 6K8 
    [ ] R25_1 300R
    [ ] R26_1 300R
    [ ] R27_1 25K5 
    [ ] RA2_1 10K (Orientation doesn't matter on this array)
    [ ] RA2_1 10K (Orientation doesn't matter on this array)
    [ ] VR1_1 50K (Marked incorrectly as 5K on some PCBs)

    Capacitors
    [ ] C11_1 22u
    [ ] C12_1 22u
    [ ] C13_1 100u
    [ ] C14_1 22p   (Look almost identical to 100p's, examine markings.) 
    [ ] C15_1 100u
    [ ] C16_1 220u
    [ ] C17_1 100p
    [ ] C18_1 100p  (Look almost identical to 22p's, examine markings.)
    [ ] C19_1 100u
    [ ] C20_1 22u

    Integrated Circuits (Install)
    [ ] IC2_1 NE5532
    [ ] IC3_1 NE5532

    Right Channel

    Resistors
    [ ] R20_2 4K7
    [ ] R21_2 100R
    [ ] R22_2 4K7
    [ ] R23_2 100R
    [ ] R24_2 6K8 
    [ ] R25_2 300R
    [ ] R26_2 300R
    [ ] R27_2 25K5 
    [ ] RA2_2 10K (Orientation doesn't matter on this array)
    [ ] RA2_2 10K (Orientation doesn't matter on this array)
    [ ] VR1_2 50K (Marked incorrectly as 5K on some PCBs)

    Capacitors
    [ ] C11_2 22u
    [ ] C12_2 22u
    [ ] C13_2 100u
    [ ] C14_2 22p   (Look almost identical to 100p's, examine markings.) 
    [ ] C15_2 100u
    [ ] C16_2 220u
    [ ] C17_2 100p
    [ ] C18_2 100p  (Look almost identical to 22p's, examine markings.)
    [ ] C19_2 100u
    [ ] C20_2 22u

    Integrated Circuits (Install)
    [ ] IC2_2 NE5532
    [ ] IC3_2 NE5532

```

## Step 7: Audio VCA

```
    Left Channel

    Resistors
    [ ] R28_1  10K
    [ ] R29_1  3K
    [ ] R30_1  47K
    [ ] R31_1  47K
    [ ] R32_1  10K
    [ ] R33_1  10K
    [ ] R34_1  27K
    [ ] R35_1  1K
    [ ] R36_1  130K
    [ ] R37_1  5K1
    [ ] R38_1  15K
    [ ] R39_1  470R
    [ ] R40_1  10K 

    Capacitors
    [ ] C21_1  22pF
    [ ] C22_1  22uF
    [ ] C23_1  100pF
    [ ] C24_1  22uF 
 
    Diodes
    [ ] D4_1
    [ ] D5_1

    ICs
    [ ] IC4_1  NE5532
    [ ] VCA1A_1  THAT2181

```

## Step 8: Filter
```
    Left Channel

    Resistors
    [ ] R41_1  10K
    [ ] R42_1  1K
    [ ] R43_1  20K
    [ ] R44_1  20K
    [ ] R45_1  20K

    Capacitors
    [ ] C25_1  22P
    [ ] C26_1  82N
    [ ] C27_1  3N3
    [ ] C28_1  22P
    [ ] C29_1  22U

    Integrated Circuit
    [ ] IC5_1  NE5532 - Install into socket
  

    Right Channel

    Resistors
    [ ] R41_2  10K
    [ ] R42_2  1K
    [ ] R43_2  20K
    [ ] R44_2  20K
    [ ] R45_2  20K

    Capacitors
    [ ] C25_2  22P
    [ ] C26_2  82N
    [ ] C27_2  3N3
    [ ] C28_2  22P
    [ ] C29_1  22U

    Integrated Circuit
    [ ] IC5_2  NE5532 - Install into socket
 
    Tests
    [ ] Perform Filter Test - Left
    [ ] Perform Filter Test - Right
```

## 9. Sidechain VCA
```
    Left Channel

    Resistors
    [ ] R46_1  1M
    [ ] R47_1  20K
    [ ] R48_1  20K
    [ ] R49_1  20K
    [ ] R50_1  10K
    [ ] R51_1  3K9
    [ ] R52_1  15K
    [ ] R53_1  47R
    [ ] R54_1  47R
    [ ] R55_1  47K
    [ ] R56_1  470R
    [ ] R57_1  470R
    [ ] R58_1  33K

    Capacitors
    [ ] C30_1  6U8 Tantalum (long lead positive)
    [ ] C31_1  22P
    [ ] C32_1  100P

    Diodes
    [ ] D6_1  
    [ ] D7_1
    [ ] D8_1 
    [ ] D9_1
    [ ] D10_1

    Integrated Circuits
    [ ] Solder adapter to VCA
    [ ] Install VCA
    [ ] Install LF347
     

    Right Channel

    Resistors
    [ ] R46_2  1M
    [ ] R47_2  20K
    [ ] R48_2  20K
    [ ] R49_2  20K
    [ ] R50_2  10K
    [ ] R51_2  3K9
    [ ] R52_2  15K
    [ ] R53_2  47R
    [ ] R54_2  47R
    [ ] R55_2  47K
    [ ] R56_2  470R
    [ ] R57_2  470R
    [ ] R58_2  33K

    Capacitors
    [ ] C30_2  6U8 Tantalum (long lead positive)
    [ ] C31_2  22P
    [ ] C32_2  100P

    Diodes
    [ ] D6_2  
    [ ] D7_2
    [ ] D8_2 
    [ ] D9_2
    [ ] D10_2

    Integrated Circuits
    [ ] Solder adapter to VCA
    [ ] Install VCA
    [ ] Install LF347
```

## Step 10.1: Meter, Attack and Release
```
    Resistors
    [ ] R50  1K
    [ ] R60  2K2
    [ ] VR3  5K Pot

    [ ] R61  820R
    [ ] R62  2K7
    [ ] R63  8K2
    [ ] R64  27K
    [ ] R65  82K
    [ ] R66  270K
    [ ] R67  3M3

    [ ] R68  180K
    [ ] R69  270K
    [ ] R70  560K
    [ ] R71  1M2
    [ ] R72  750K
    [ ] R73  91K
 
    Capacitors
    [ ] C33  0.47U
    [ ] C34  0.47U
    [ ] C35  0.47U
    [ ] C36  0.47U
    [ ] C37  6U8
    [ ] C38  0.47U   
     
```

## Step 10.2: Ratio Compoonents
```
    Resistors
    [ ] R74  620K
    [ ] R75  68K
    [ ] R76  510K
    [ ] R77  270K
    [ ] R78  3M9
    [ ] R79  1M8
    [ ] R80  1M2
    [ ] R81  620K
    [ ] R82  68K
    [ ] R83  270K
    [ ] R84  510K
    [ ] R85  3M9
    [ ] R86  1M8
    [ ] R87  1M2
    [ ] R88  91K
    [ ] R89  470K
    [ ] R90  100R
    [ ] R91  100K
    [ ] R92  620K
    [ ] VR4  50K  Trimmer

    Capacitors
    [ ] C39  10U  (Non-polarized)
    [ ] C40  10U  (Non-polarized)
    [ ] C41  10U  (Non-polarized)
    [ ] C42  10U  (Non-polarized)
    [ ] C43  100P

    Diodes
    [ ] D12 
    [ ] D13 
```
