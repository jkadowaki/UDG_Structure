# UDG_Structure
Estimating Redshifts by Quantifying Pixel Variations in UDG Candidates

I hypothesize that the presence of star forming knots or structural features within UDG candidates are an indicator of an object's physical distance (and therefore size). To test this hypothesis, I measured pixel variations within the half-light radius of diffuse, spatially-extended galaxies to discriminate likely UDG-candidates from spurious, foreground sources. Pixel variation are measured by applying a 1D-KDE on the distribution of pixel intensities from the residual image taken between the DECaLS/DES images of candidates and their GALFIT models. I used the mean squared error to quantify how much the KDE deviates from a zero-mean Gaussian to quantify the amount of structure is in the UDG candidate. I find MSE (and therefore the presence of structures in UDG candidate) appear to scale linearly with redshift. We can use this result to select targets for the next observational run at the Large Binocular Telescope (LBT) in mid-January 2018.


To Be Implemented/Investigated in the Very Near Future (Before 2018)
------------------------------------------------------
1. Incorporate objects we detect in our pipeline that have known velocities from NED. This may fill in the void between cz=2000-6000 km/s range. (However, most known foreground objects appear to be around cz=500 km/s, placing them near the 3 other non-UDG sources we observed.)
2. Follow-up on the extreme outlier cases. Why are they outliers? (e.g. Foreground star overlaid on background UDG?) This may help reduce the variance in our result.
3. Determine ideal kernel and kernel bandwidth for every filter/band and calibrate MSE.
4. Compute pixel variation MSE for all candidate targets for the LBT 2018a observational run. Determine optimal targets & create MODS observing scripts.



To Be Implemented in the Distant Future (After 2017)
---------------------------------------
1. Apply SVMs to determine MSE cut per band.
2. Update results with LBT 2018A targets.
