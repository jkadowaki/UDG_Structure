# UDG_Structure
Estimating Redshifts by Quantifying Pixel Variations in UDG Candidates

I hypothesize that the presence of star forming knots and structural features within UDG candidates are indicators of their physical distances and sizes. If true, these features can be used to differentiate UDGs from spurious sources that contaminate our survey. To test this hypothesis, I measured pixel variations within the half-light radius of diffuse, spatially-extended galaxies to discriminate likely UDG-candidates from spurious, foreground sources. Pixel variation are measured by applying a 1D-KDE on the distribution of pixel intensities from the residual image taken between the DECaLS/DES images of candidates and their GALFIT models. I used the mean squared error to quantify how much the KDE deviates from a zero-mean Gaussian to quantify the amount of structure is in the UDG candidate. I find that the MSE (and therefore the presence of structures & knots in UDG candidate) appear to scale linearly with redshift. We can use this result to select targets for the next observational run at the Large Binocular Telescope (LBT) in mid-January 2018.



To Be Implemented/Investigated in the Very Near Future (Before 2018)
------------------------------------------------------
1. Incorporate objects we detect in our pipeline that have known velocities from NED. This may fill in the void between cz=2000-6000 km/s range. (However, most known foreground objects appear to be around cz~500-1000 km/s, placing them near the 3 other non-UDG sources we observed.)
2. Follow-up on the extreme outlier cases. Why are they outliers? (e.g. Foreground star overlaid on background UDG?) This may help reduce the variance in our result.
3. Determine ideal kernel and kernel bandwidth for every filter/band and calibrate MSE.
4. Compute pixel variation MSE for all candidate targets for the LBT 2018a observational run. Determine optimal targets & create MODS observing scripts.



To Be Implemented in the Distant Future (After 2017)
---------------------------------------
1. Apply SVMs to determine MSE cut per band.
2. Update results with LBT 2018A targets.
3. Check PU0838589 and see why we didn't get redshift.



LBT 2018 Candidates
-------------------
Stripe 82
1.  UDG0244338
2.  UDG0239472
3.  UDG0115016
4.  UDG0113177
5.  UDG0111031
6.  UDG0112072

Coma
1.  UDG1217267
2.  UDG1218389
3.  UDG1233477
4. UDG1237293
5. LBT2104 (ra:12:45:27.9, dec:18:18:01)
