<p align="center">
<i>If you are not viewing this readme file on the main github repository for FreQ (https://github.com/hansenjn/FreQ), please visit the main github repository to view the latest information on the plugin.</i>
</p>

# ![FreQ](https://github.com/hansenjn/FreQ/blob/master/FreQ%20Logo%20Small.png?raw=true)
(previously called **Cilility_JNH**)

An ImageJ plugin to analyze pixel intensity oscillations in time-lapse 2D images. For example, this allows to characterize the ciliary beat of multi-ciliated cells in time-lapse images acquired with a bright-field or phase-contrast microscope.

Note that initial versions of FreQ (v0.0.1-v0.2.3) were called "Cilility_JNH" - From v0.3.0 on, the plugin is called FreQ.

Copyright (C) 2019-2026: Jan N. Hansen

Contacts: jan.hansen ( at ) uni-bonn.de

This program was developed in the research group Biophysical Imaging, Institute of Innate Immunity, Bonn, Germany ([Lab homepage](https://www.iiibonn.de/dagmar-wachten-lab/dagmar-wachten-lab-science)).

## Plugin description
This ImageJ plugin extracts periodic changes of pixel intensity, such as those evoked by ciliary beating. These periodic changes are further analyzed using a Fast Fourier Transformation. Among other parameters the plugin determines the (ciliary beat) frequency.

To find out more about the application of the software and ouput parameters, please see our STAR protocol on the measurement of ciliary beating:

> Jeong I, Hansen JN, Wachten D, Jurisch-Yaksi N. Measurement of ciliary beating and fluid flow in the zebrafish adult telencephalon. STAR Protoc. 2022 Jul 15;3(3):101542. doi: [10.1016/j.xpro.2022.101542](https://doi.org/10.1016/j.xpro.2022.101542).

The underlying analysis methods were inspired by the MATLAB-based analysis presented in [Olstad et al., Curr. Biol, 2019](https://doi.org/10.1016/j.cub.2018.11.059), and [D'Gama et al., Cell Rep. 2021](https://doi.org/10.1016/j.celrep.2021.109775).

## How to use the FreQ plugin?
In 2026, we introduced a wiki to the FreQ github repository that provides instructions on how to install and apply FreQ:
https://github.com/hansenjn/FreQ/wiki.

Furthermore, please also take a look at the STAR protocol ([Jeong et al. 2022](https://doi.org/10.1016/j.celrep.2021.109775)) describing application of FreQ to study the ciliary beating in the zebrafish. For any additional questions, please contact jan.hansen(at)uni-bonn.de.

## How to cite the FreQ plugin?
Please acknowledge the methodology of the analysis by citing the following protocol:

> Jeong I, Hansen JN, Wachten D, Jurisch-Yaksi N. Measurement of ciliary beating and fluid flow in the zebrafish adult telencephalon. STAR Protoc. 2022 Sep 16;3(3):101542. PMID: 35842868. doi: [10.1016/j.xpro.2022.101542](https://doi.org/10.1016/j.celrep.2021.109775).

The source code for the software is archived on zenodo (all software versions are accessible via the DOI: <a href="https://doi.org/10.5281/zenodo.5138071"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.5138071.svg" alt="DOI"></a>).

The zenodo archive also allows to cite/refer a very specific software version through specific DOIs:
- v0.3.0: <a href="https://doi.org/10.5281/zenodo.5911902"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.5911902.svg" alt="DOI"></a>
- v0.2.3: <a href="https://doi.org/10.5281/zenodo.5865182"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.5865182.svg" alt="DOI"></a>
- v0.2.2: <a href="https://doi.org/10.5281/zenodo.5138072"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.5138072.svg" alt="DOI"></a>

## Staying up-to-date
The most recent information and latest updates on the software are available through the main github repository for FreQ: 
https://github.com/hansenjn/FreQ. 

If you install FreQ via the update manager in FIJI (see above), with every update of FIJI your FreQ version will be updated as well (in case a newer release of FreQ is available).

## LICENSE NOTES
The newly developed software is licensed under GNU General Public License v3.0. However, this software includes packages derived from others, for which different licenses may apply. The different licenses and the authors of theses code parts are clearly stated in the headers of the respective classes. This applies to the following packages\classes:
- edu.emory.mathcs.jtransforms.fft\DoubleFFT_1D.java & edu.emory.mathcs.utils\ConcurrencyUtils.java (MPL 1.1/GPL 2.0/LGPL 2.1, Mozilla Public License Version 1.1, author: Piotr Wendykier)
