DNA_CALC – Tumor DNA Section Estimation Calculator (Updated)
Author: Richard Siderits

------------------------------------------------------------
PURPOSE
------------------------------------------------------------
This calculator estimates the number of 10-micron FFPE tumor
sections required to reach a user-selected genomic DNA target
(100–500 ng) for next-generation sequencing (NGS).

It provides a geometry-based estimate of tumor DNA yield and
translates that into a practical sectioning recommendation.

------------------------------------------------------------
KEY CONVERSION LOGIC
------------------------------------------------------------
• 1 diploid cell ≈ 6 picograms (pg) DNA  
• 6 pg = 0.006 nanograms (ng)  
• 1 ng = 1000 pg  

NGS requirements are expressed in nanograms, so all calculations
are converted to ng before determining required sections.

------------------------------------------------------------
IMPORTANT OUTPUT DISTINCTION
------------------------------------------------------------
The calculator provides TWO related but different DNA outputs:

1. Total tumor DNA from 100µm depth (10 sections combined, ng)
   → Represents DNA yield from a stack of ten 10µm sections

2. Tumor DNA per 10µm section (ng)
   → Represents DNA yield from a SINGLE section
   → THIS is the value used to calculate required sections

Relationship:
100µm value = 10 × (10µm section value)

------------------------------------------------------------
FEATURES
------------------------------------------------------------
• Tumor cell estimation using spherical geometry
• Adjustment for tumor-induced stroma
• DNA estimation using 6 pg per cell
• Extraction efficiency correction
• DNA yield modeling per 100µm and per 10µm section
• User-selectable NGS DNA target (100–500 ng)
• Automatic calculation of required section count
• Copy-ready report output

------------------------------------------------------------
INPUT PARAMETERS
------------------------------------------------------------
• Tumor size (mm)
• Average tumor cell size (µm)
• Percent stroma (%)
• Percent stromal cellularity (%)
• Extraction efficiency (%)
• Target DNA for NGS (100–500 ng)

------------------------------------------------------------
OUTPUTS
------------------------------------------------------------
• Estimated tumor cell count
• Stroma-adjusted tumor cell count
• Total tumor DNA (pg)
• DNA from 100µm depth (ng)
• DNA per 10µm section (ng)
• Required number of 10µm sections

------------------------------------------------------------
HOW THE CALCULATION WORKS
------------------------------------------------------------
1. Tumor size converted from mm → µm
2. Tumor and cells modeled as spheres
3. Cell count = tumor volume / cell volume
4. Tumor fraction adjusted for stroma
5. DNA estimated at 6 pg per cell
6. 100µm depth modeled (10 sections)
7. Extraction efficiency applied
8. pg → ng conversion performed
9. DNA per 10µm section calculated
10. Sections required:

   sections = ceil(target ng / ng per section)

------------------------------------------------------------
INTERPRETATION
------------------------------------------------------------
The section count is a conservative estimate assuming:
• Uniform tumor distribution
• Diploid DNA content
• Representative sampling
• Accurate efficiency estimate

Only the **per 10µm section DNA value** drives the section count.

------------------------------------------------------------
LIMITATIONS
------------------------------------------------------------
• Assumes uniform tumor composition
• Does not account for necrosis or heterogeneity
• Based on geometric approximations
• Actual yield varies with fixation and processing

------------------------------------------------------------
DISCLAIMER
------------------------------------------------------------
This tool is for planning purposes only. Final DNA adequacy
must be confirmed by direct measurement and laboratory QC.
