# Assessing the perfomance of the JWST Image Simulator - PhoSim-NIRCam
## *Arsh R. Nadkarni - Steward Observatory, UArizona*
## *Adviser: Dr. Eiichi Egami - Steward Observatory, UArizona*

<img src="https://github.com/astroarshn2000/JWST-PhoSim-NIRCam/blob/master/Images/Visuals/NIRCam_Logo_AZ.png" height="350" width="500"/> <img src="https://github.com/astroarshn2000/JWST-PhoSim-NIRCam/blob/master/Images/Visuals/JWST%20Decal.png" height="350" width="350"/> 

PhoSim-NIRCam is a full end-to-end JWST/NIRCam image simulator built on the framework of the LSST image simulator PhoSim. It contains a comprehensive physical model of the JWST telescope + NIRCam, and simulates photons propagating through the whole system using a Monte Carlo approach.  PhoSim-NIRCam is easy to use, allowing the user to start creating realistic NIRCam images with minimal preparation.  It also provides a variety of advanced features that allow direct control of any element in the system.

## More about PhoSim-NIRCam
Although developed primarily for LSST, PhoSim itself is a physics-based code that can simulatie any optical/IR observing system when used with appropriately constructed configuration files. PhoSim-NIRCam has been developed by taking advantage of this feature, and is essentially PhoSim that comes with a particular set of configuration files constructed for JWST + NIRCam. Despite its complex inner working, PhoSim-NIRCam is easy to use, and is typically run as a one-line command with a CatalogFile and a CommandsFile.

**Disclaimer**: PhoSim-NIRCam is still in the early phase of develpment, and has not been tested extensively!

## Information/References
**LSST PhoSim**

* PhoSim Reference Paper: [Peterson, J. R. et al. 2015, ApJS, 218, 14](https://iopscience.iop.org/article/10.1088/0067-0049/218/1/14/pdf)
* PhoSim Reference Document: [The Photon Simulator (PhoSim)](https://lsst.rcac.purdue.edu/doc/phosim_reference.pdf)
* PhoSim SED library (star/galaxy SEDs): [SEDs (6 GB)] (https://lsst.rcac.purdue.edu/doc/SEDs.tar.gz)
* Websites: [PhoSim](https://confluence.lsstcorp.org/pages/viewpage.action?pageId=4129126), [PhoSim@LSST](https://www.lsst.org/scientists/simulations/phosim)

**JWST PhoSim-NIRCam**

* PhoSim-NIRCam Homepage: [https://fenrir.as.arizona.edu/phosim/](https://fenrir.as.arizona.edu/phosim/)
* PhoSim-NIRCam Reference Document: [Implementation of the JWST/NIRCam in PhoSim](https://fenrir.as.arizona.edu/phosim/docs/phosim-nircam.pdf)
* PhoSim Diffraction Algorithm: [Modification to the Diffraction Algorithm in PhoSim for Space Telescopes](https://fenrir.as.arizona.edu/phosim/docs/diffraction_doc_final.pdf)
* Quick Guide (up-to-date instruction): [Full Guide](https://fenrir.as.arizona.edu/phosim/docs/PhoSim_QuickGuide.pdf)
* Examples of PhoSim-NIRCam output files: [mkimage.tar.gz (6.7 MB)](https://fenrir.as.arizona.edu/phosim/images/mkimage_example.tar.gz)
