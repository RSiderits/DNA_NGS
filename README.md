DNA_CALC – Tumor DNA Section Estimation Calculator
Author: Richard Siderits

------------------------------------------------------------
PURPOSE
------------------------------------------------------------
This calculator estimates the number of 10-micron FFPE (formalin-
fixed paraffin-embedded) tumor tissue sections required to ensure
a minimum of 100 nanograms of evaluable tumor DNA for downstream
next-generation sequencing (NGS).

The model uses geometric assumptions and biologic approximations
to estimate tumor cell counts and DNA yield based on specimen
characteristics and laboratory performance parameters.

This tool is intended for specimen triage, planning, and workflow
standardization in molecular pathology and research laboratories.

------------------------------------------------------------
FEATURES
------------------------------------------------------------
• Calculates estimated tumor cell count based on tumor size and
  average cell size (spherical geometry assumption)

• Adjusts tumor cell count based on percent tumor-induced stroma

• Estimates total tumor DNA using a diploid approximation of
  6 picograms DNA per cell

• Models DNA yield from a 100-micron tissue depth (equivalent to
  ten 10-micron sections)

• Applies laboratory-specific DNA extraction efficiency

• Converts DNA yield into nanograms per 10-micron section

• Determines the minimum number of 10-micron sections required
  to achieve ≥100 ng of tumor DNA

• Provides report-ready output for direct use in documentation

• Includes a “Copy Results for Report” function for easy transfer
  into laboratory reports or study records

------------------------------------------------------------
INPUT PARAMETERS
------------------------------------------------------------
1. Tumor Size (mm)
   Estimated largest dimension of tumor tissue

2. Average Tumor Cell Size (µm)
   Approximate diameter of tumor cells

3. Percent Stroma (%)
   Proportion of tumor-induced stroma within the sample

4. Percent Stromal Cellularity (%)
   Cellular fraction of stromal component (informational)

5. Extraction Efficiency (%)
   Estimated DNA recovery efficiency of the laboratory method

------------------------------------------------------------
OUTPUTS
------------------------------------------------------------
• Estimated number of tumor cells (pure tumor)

• Stroma-compensated tumor cell count

• Total tumor DNA (picograms)

• DNA yield from a 100µm sample (pg and ng)

• DNA yield per 10µm section (ng)

• Required number of 10µm sections to achieve ≥100 ng DNA

------------------------------------------------------------
HOW TO USE
------------------------------------------------------------
1. Enter all required input values
2. Click “Calculate”
3. Review calculated outputs
4. Click “Copy Results for Report” to generate formatted text
5. Paste results into your report or documentation system

------------------------------------------------------------
INTERPRETATION
------------------------------------------------------------
The calculated number of sections represents a conservative
estimate based on:

• Spherical tumor geometry
• Uniform tumor distribution
• Diploid DNA content (6 pg/cell)
• Enhanced-for-tumor sampling assumption

The result ensures adequate DNA yield under expected laboratory
conditions, accounting for extraction efficiency.

------------------------------------------------------------
LIMITATIONS
------------------------------------------------------------
• Assumes uniform tumor composition and cell size
• Does not account for necrosis or heterogeneity
• Stromal DNA is not used in section calculation
• Real-world DNA yield may vary based on fixation,
  processing, and extraction conditions

------------------------------------------------------------
DISCLAIMER
------------------------------------------------------------
This calculator is intended for planning and estimation only.
It does not replace direct measurement of extracted DNA quantity
or quality prior to sequencing.

Final suitability for NGS must be confirmed by laboratory QC
metrics and validated assay requirements.
