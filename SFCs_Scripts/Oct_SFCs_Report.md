# October/Nov SFCs Report 
Trying to find the source flux counts for two systems - Quasar and Monk in order to proceed with Zero-Point Magnitude Determination and subsequently add noise to the simulated images.

**First Results -**
![alt text](https://github.com/astroarshn2000/JWST-PhoSim-NIRCam/blob/master/SFCs_Scripts/Quasar%20vs%20Monk%20SFC%20Comparison.png)

*Findings*
- New version of PhoSim has noise already added to it while running the simulation, rather than adding it manuallly after the simulation.
- Quasar has SFCs (Old-PhoSim) which are slightly offset from the values mentioned in the fenrir guide.

*Offset*
- Comparing my results in the form of Arsh v/s Eiichi for the Old version of PhoSim on both machines

` % Offset = {abs(Eiichi_val-Arsh_val)/Eiichi_val)}*100 `

![alt text](https://github.com/astroarshn2000/JWST-PhoSim-NIRCam/blob/master/SFCs_Scripts/Percentage%20Errors%20-%20Old%20PhoSim-NIRCam%20.png)


**Second Results -**
- New PhoSim modified by replacing the geo_diff config file by geo_diff_nobkg config file. This doesn't give the pre-added background as it used to earlier.

*Findings*
- Runs fine on Quasar. 
- On Monk, simulator runs fine but gives the following error producing no files in the end.

`[astroarshn2000@monk PhoSim-NIRCam.v5.1.7]$ tail log.lw_geo_diff_star_1022 

Placing Obstructions.

Perturbing Design.

Electrifying Devices.

Contaminating Surfaces.

Diffracting.

Error opening 

mv: cannot stat â: No such file or directory`

![alt text](https://github.com/astroarshn2000/JWST-PhoSim-NIRCam/blob/master/SFCs_Scripts/NoBkg%20Quasar%20vs%20Monk%20SFC%20Comparison.png)
