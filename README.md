# MechanoSorptiveCreep
Notebooks for the evaluation of mechanosorptive creep

Test_MS_decomposition_routine_Ferrara_Wittel_2025.ipyjn:
File for precalculation and validation of routine:
Incremental decomposition scheme for mechanosoprtive strain calculation
A. Ferrara and F.K. Wittel "Mechanosorptive Creep of Norway Spruce on the Tissue Scale Perpendicular to Grain", Holzforschung (2025)
This notebook implements and tests the incremental decomposition scheme proposed in Ferrara and Wittel (2025b) on calculated clean data to isolate mechanosorptive creep strain, using the MS_Creep_Tests_Dataset (10.17632/rsrsw8h7mv.1).

The dataset includes the results of:

Tensile elastic tests on Norway spruce tissue slices in all anatomical orientations (longitudinal L, radial R, tangential T) and combinations {LR, RL, RT, TR, LT} (first letter = length, second = width). Tests were performed at relative humidity (RH) levels of 30%, 65%, and 90%, corresponding to moisture contents (mc) of 0.07, 0.12, and 0.20, respectively.
Tensile creep tests on the same tissue slice orientations and moisture conditions.
Dynamic Vapor Sorption (DVS) tests on a RL-slice, following the RH profile applied in the mechanosorptive experiments.

MS_creep_tests_Ferrara_Wittel_2025.ipyjn:
File for Ploting:
Incremental decomposition scheme for mechanosoprtive strain calculation
A. Ferrara and F.K. Wittel "Mechanosorptive Creep of Norway Spruce on the Tissue Scale Perpendicular to Grain", Holzforschung (2025)
This Notebook allows to plot the data contained in MS_Creep_Tests_Dataset (10.17632/rsrsw8h7mv.1). The dataset contains experimental results from our study (Ferrara and Wittel, 2025b), in which mechanosorptive creep tests were performed on Norway spruce tissue slices in the transverse anatomical directions, radial (R) and tangential (T), under cyclic relative humidity (RH) between 30% and 90%. Samples were cut in the orientations {RL, RT, TR}, where the first letter denotes the longitudinal dimension and the second the transverse width, all comprising alternating bands of earlywood (EW) and latewood (LW). Tests were carried out at different loading degrees (LD): {RL, RT} at 30% and 50%, and {TR} at 40% of the respective tensile strength. Reference tensile strengths were taken from our earlier work (Ferrara and Wittel, 2024).

The dataset is organized by sample type, with each file containing multiple sheets corresponding to individual experiments. Each sheet reports detailed information about the sample (e.g., dimensions, loading degree, etc.), together with time, moisture content, and mechanosorptive creep strain and compliance. The mechanosorptive creep strain was calculated by applying the proposed incremental decomposition scheme to isolate them from the total strain directly measured with Digital Image Correlation (DIC).

In addition, The dataset includes two CSV files with the results of:

Tensile elastic tests on Norway spruce tissue slices, provided as mean elastic compliance values from our earlier work (Ferrara and Wittel, 2024), enabling analyses of how creep compliance scales with elastic compliance
Tensile creep tests, provided as element compliances of the Kelvin–Voigt model describing the mean viscoelastic compliances from our previous work (Ferrara and Wittel, 2025a), which serve as input for calculating the viscoelastic strain component
and one NPZ file with the results of
Dynamic Vapor Sorption (DVS) tests on a RL-slice, following the RH profile applied in the mechanosorptive experiments.
