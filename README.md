# SSL G-Series Bus Compressor Build

## Step 1: Bypass Caps and IC Sockets 

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
    [ ] CB7_1 - 
    [ ] CB8_1 - 
    [ ] CB9_1 - 
    [ ] CB10_1 - 
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
    
```
