HELP.TXT
DAB LOT-TO-LOT COMPARATOR
=========================

PURPOSE
-------

The DAB Lot-to-Lot Comparator is a browser-based research and quality review
tool for comparing the average intensity of DAB staining between two IHC
images.

The usual use is:

- Image 1: Reference slide, reference lot, or accepted baseline run
- Image 2: New DAB lot, candidate lot, new run, or alternate platform

The tool estimates DAB optical density from the image data and reports whether
Image 2 is darker/stronger, lighter/weaker, or similar compared with Image 1.

This tool can be used for:

- DAB lot-to-lot comparison
- New DAB reagent lot check
- Run-to-run staining comparison
- Platform-to-platform comparison
- Scanner or microscope acquisition comparison
- Research assay optimization
- IHC quality review
- Documentation of relative DAB staining intensity differences

This is a practical relative comparison tool. It is not a validated clinical
diagnostic image analysis system.

INTENDED USE
------------

Use this comparator when you want to answer a simple but important question:

"Does the new DAB lot, new staining run, or alternate platform produce DAB
staining intensity that is acceptably similar to the reference condition?"

Examples:

1. Reference DAB lot versus new DAB lot
2. Previous accepted run versus current run
3. Leica platform versus Ventana platform
4. Manual stain versus automated stain
5. Existing scanner setting versus new scanner setting
6. Before/after maintenance run comparison
7. Same marker stained on different days
8. Same antibody protocol after a detection-system change

WHAT THE TOOL COMPARES
----------------------

The tool compares two images:

Image 1 / Reference Lot

This should be the accepted reference image. It may represent the current DAB
lot, accepted reagent lot, accepted staining run, accepted platform, or known
acceptable baseline.

Image 2 / Candidate Lot

This should be the comparison image. It may represent a new DAB lot, new
staining run, new platform, alternate scanner, or other condition being
evaluated.

The result focuses on DAB-positive staining intensity. Negative/background is
excluded from the visible weak/moderate/strong structured result table.

WHAT THE TOOL CALCULATES
------------------------

The comparator calculates:

- Overall Image 1 mean DAB optical density
- Overall Image 2 mean DAB optical density
- Overall percent difference between Image 1 and Image 2
- Overall direction of change
- Weak staining mean DAB optical density
- Moderate staining mean DAB optical density
- Strong staining mean DAB optical density
- Percent difference for weak, moderate, and strong staining buckets
- Area percentage for each bucket
- Area delta between Image 2 and Image 1
- Greatest bucket-level intensity difference
- QC overlay images showing weak, moderate, and strong regions
- A copyable/exportable text report

BASIC CONCEPT
-------------

DAB staining appears brown. The software estimates a DAB-biased optical density
from the RGB image values. Higher DAB optical density generally corresponds to
stronger or darker DAB staining.

The tool then compares the average DAB optical density of Image 2 against Image
1. It also compares weak, moderate, and strong staining compartments separately.

The point is not to replace pathologist judgment. The point is to provide a
consistent numeric check that supports visual review.

WHEN TO USE THIS TOOL
---------------------

Use this tool when the tissue, stain, and image conditions are sufficiently
similar that a numeric DAB intensity comparison is meaningful.

Appropriate examples include:

- Same tissue block, serial sections, same marker, different DAB lot
- Same marker and tissue stained in two different runs
- Same slide or closely matched slide imaged on two platforms
- Same assay transferred from one staining platform to another
- Research comparison where relative DAB intensity is being documented

Avoid overinterpreting results when:

- The tissue areas are not comparable
- One image has substantially more tumor, necrosis, stroma, or background
- One image is out of focus
- Exposure, white balance, or scanner settings differ substantially
- The stain includes heavy artifact, folds, bubbles, melanin, or pigment
- The images were captured at different magnifications
- The reference image is itself not acceptable

IMAGE REQUIREMENTS
------------------

For the most defensible comparison, use images that are as similar as possible.

Recommended:

- Same tissue type
- Same marker
- Same magnification
- Similar field selection
- Similar amount of target tissue
- Similar fixation and processing history
- Similar image acquisition settings
- Similar scanner or microscope settings
- Minimal artifact
- Representative staining field

Best practice for lot-to-lot comparison:

- Use serial sections from the same tissue block when possible.
- Use a known positive reference tissue or assay-relevant control tissue.
- Capture comparable regions from each slide.
- Avoid blank glass, tissue edges, folds, necrosis, overstained debris, and
  poor-focus regions.
- Use the same image acquisition procedure for both images.

STEP-BY-STEP INSTRUCTIONS
-------------------------

1. Open the DAB Lot-to-Lot Comparator

   Open the HTML file in a modern web browser.

2. Load Image 1 / Reference Lot

   Drag and drop the reference image into the Image 1 box, or use the file
   chooser.

   Image 1 should be the accepted reference image. For example:

   - Current accepted DAB lot
   - Previously accepted staining run
   - Validated platform result
   - Known acceptable reference slide

3. Load Image 2 / Candidate Lot

   Drag and drop the candidate image into the Image 2 box, or use the file
   chooser.

   Image 2 should be the condition being compared. For example:

   - New DAB lot
   - New run
   - New platform
   - New scanner setting
   - Post-maintenance run
   - Alternate protocol condition

4. Confirm the images loaded correctly

   Review the image previews before calculating.

   Make sure the images are not reversed unless that is intentional. The
   direction statement is always written as Image 2 compared with Image 1.

5. Press Calculate

   Click the Calculate button.

   The tool will estimate DAB optical density, classify the staining into
   weak, moderate, and strong buckets, calculate the overall and bucket-level
   differences, and generate QC overlays.

6. Review the status message

   The status field will confirm that analysis is complete or identify a
   problem.

   Possible issues include:

   - One or both images were not loaded
   - Too few analyzable tissue/stain pixels were detected
   - Image quality or field selection may be unsuitable

7. Review the overall metrics

   The result panel shows:

   - Overall Image 1 Mean DAB OD
   - Overall Image 2 Mean DAB OD
   - Overall Percent Difference
   - Overall Direction

   These are the main comparison outputs.

8. Interpret the overall direction

   Direction tells you whether Image 2 is:

   - darker / stronger than Image 1
   - lighter / weaker than Image 1
   - similar to Image 1

   Example:

   If Image 2 is darker / stronger, the candidate lot, run, or platform is
   producing higher average DAB optical density than the reference condition.

   If Image 2 is lighter / weaker, the candidate condition is producing lower
   average DAB optical density than the reference condition.

9. Review the structured summary table

   The table reports weak, moderate, and strong staining separately.

   For each bucket, the table shows:

   - Image 1 Mean OD
   - Image 2 Mean OD
   - Intensity % Diff
   - Image 1 Area %
   - Image 2 Area %
   - Area Delta
   - Direction

   This is useful because two images can have similar overall average DAB OD
   but different distributions of weak, moderate, and strong staining.

10. Review the greatest bucket-level intensity difference

   The callout identifies which staining bucket had the largest intensity
   difference.

   This is useful when the overall difference is modest but one staining
   compartment changed substantially.

11. Review the QC overlays

   The QC overlay shows where the tool classified pixels as weak, moderate, or
   strong DAB staining.

   Overlay colors:

   - Weak = pale blue
   - Moderate = orange
   - Strong = red

   Negative/background is intentionally not shown in the visible result table
   and is not emphasized in the overlay.

   Review the overlays before trusting the numbers. Make sure the tool is
   highlighting real DAB staining rather than artifact, background, pigment, or
   irrelevant tissue.

12. Copy the report

   Click Copy Report to place the text report on the clipboard.

   The report includes:

   - Date and time generated
   - Image 1 filename
   - Image 2 filename
   - Overall DAB optical density comparison
   - Weak/moderate/strong structured summary
   - Greatest bucket-level intensity difference
   - Internal thresholds
   - Formulas
   - Caution statement

13. Export the report

   Click Export Report to save a text file.

   Default filename:

   DAB_lot_to_lot_comparison_report.txt

14. Reset if needed

   Click Reset to clear images, results, QC overlays, and report text.

FORMULAS USED
-------------

Overall percent difference:

   |Image 2 Mean DAB OD - Image 1 Mean DAB OD|
   ------------------------------------------------ x 100
      average of Image 1 Mean DAB OD and Image 2 Mean DAB OD

Bucket intensity percent difference:

   The same formula is used, but only within the weak, moderate, or strong
   staining bucket being compared.

Area delta:

   Image 2 bucket area percentage - Image 1 bucket area percentage

Direction:

   Image 2 is darker / stronger if its mean DAB OD is higher than Image 1.
   Image 2 is lighter / weaker if its mean DAB OD is lower than Image 1.
   Image 2 is similar if the values are essentially the same.

WHY THE TOOL USES A SYMMETRIC PERCENT DIFFERENCE
------------------------------------------------

The comparator uses the average of the two values as the denominator. This is a
balanced way to describe the difference between two measurements.

This avoids the problem of making the percent difference depend entirely on
which image is chosen as the denominator.

For example, a change from 0.30 to 0.20 and a change from 0.20 to 0.30 have the
same magnitude of difference. The direction field then tells you whether the
candidate image is darker/stronger or lighter/weaker.

HOW THRESHOLDS ARE USED
-----------------------

The tool derives common weak, moderate, and strong thresholds from the combined
DAB optical density distribution of both images.

This means both images are classified on the same internal scale.

The internal thresholds include:

- Negative/Weak cutoff
- Weak/Moderate cutoff
- Moderate/Strong cutoff

Negative/background is calculated internally but omitted from the displayed
positive-staining result table. The visible structured summary focuses on weak,
moderate, and strong DAB-positive staining.

INTERPRETING LOT-TO-LOT RESULTS
-------------------------------

A good lot-to-lot comparison should show that the candidate lot behaves
similarly to the reference lot in both:

1. Overall average DAB intensity
2. Distribution of weak, moderate, and strong staining

A potentially acceptable result may show:

- Small overall percent difference
- Similar direction or only minor shift
- Similar weak/moderate/strong area distribution
- QC overlays that highlight similar tissue compartments
- No unexplained strong bucket shift
- No obvious artifact or field selection problem

A result needing review may show:

- Moderate overall percent difference
- Candidate lot is visibly darker or lighter
- One bucket shows a large difference
- Strong staining area increases unexpectedly
- Weak staining replaces expected moderate/strong staining
- QC overlays do not match visual impression
- Field selection appears mismatched

A result needing investigation may show:

- Large overall percent difference
- Candidate lot is substantially darker or weaker
- Strong staining is lost or markedly increased
- Moderate staining shifts heavily into weak or strong categories
- QC overlay highlights artifact instead of true DAB staining
- Tissue comparability is poor
- Scanner or camera settings differ between images

INTERPRETING RUN-TO-RUN RESULTS
-------------------------------

For run-to-run comparison, use Image 1 as the accepted reference run and Image 2
as the new run.

A run-to-run difference may reflect:

- Reagent variation
- Incubation time variation
- Retrieval variation
- Detection chemistry variation
- Instrument performance
- Slide drying or tissue handling
- Section thickness
- Counterstain or dehydration variation
- Imaging variation

A small difference supports run consistency. A large difference should prompt
review of the staining record, controls, instrument logs, and image acquisition
conditions.

INTERPRETING PLATFORM-TO-PLATFORM RESULTS
-----------------------------------------

For platform-to-platform comparison, use Image 1 as the accepted platform and
Image 2 as the alternate platform.

Platform differences may reflect:

- Retrieval chemistry
- Incubation timing
- Detection system sensitivity
- DAB development time
- Wash conditions
- Counterstain intensity
- Scanner or camera response
- White balance or color calibration differences

A platform-to-platform comparison should be interpreted conservatively. Numeric
similarity is useful, but platform transfer should also include pathologist
review and appropriate control material.

SUGGESTED REVIEW LANGUAGE
-------------------------

Example acceptable comparison language:

"The candidate DAB lot demonstrated comparable average DAB optical density to
the reference lot in the selected representative field. The weak, moderate, and
strong staining distributions were reviewed along with QC overlays. No
materially significant shift in DAB staining intensity was identified."

Example review-needed language:

"The candidate DAB lot showed a measurable shift in average DAB optical density
relative to the reference lot. The difference was most prominent in the
[weak/moderate/strong] staining bucket. Repeat review of field selection, stain
quality, and control material is recommended before acceptance."

Example investigation language:

"The candidate condition demonstrated a substantial difference in average DAB
optical density relative to the reference condition. The magnitude and/or
pattern of change may indicate a reagent, run, platform, acquisition, or tissue
comparability issue. Additional review and repeat testing are recommended."

RECOMMENDED ACCEPTANCE APPROACH
-------------------------------

This HTML tool reports percent differences and directions but does not impose a
fixed pass/fail cutoff. The laboratory or study team should define its own
acceptance criteria.

A practical research review framework may use:

- Less than 15% difference: generally comparable
- 15% to 25% difference: review
- Greater than 25% difference: investigate

These are practical review bands, not universal regulatory requirements. For a
formal laboratory procedure, acceptance criteria should be predefined,
documented, and appropriate for the assay purpose.

DOCUMENTATION RECOMMENDATIONS
-----------------------------

For lot-to-lot comparison, document:

- Marker name
- Antibody clone
- Antibody lot
- DAB lot/reference lot
- DAB lot/candidate lot
- Detection system
- Staining platform
- Tissue/control used
- Slide identifiers
- Date of staining
- Date of image acquisition
- Magnification or scanner settings
- Operator/reviewer
- Overall percent difference
- Overall direction
- Greatest bucket-level difference
- Final interpretation
- Acceptance decision
- Any corrective action

For run-to-run comparison, document:

- Reference run date
- Candidate run date
- Instrument/platform
- Reagent lots
- Control slide result
- Any maintenance or deviation

For platform-to-platform comparison, document:

- Platform 1 and platform 2
- Retrieval conditions
- Detection systems
- DAB development conditions
- Scanner or image acquisition conditions
- Pathologist review conclusion

LIMITATIONS
-----------

This tool has important limitations:

- It is not a validated clinical diagnostic image analysis platform.
- It performs a practical DAB-biased optical density estimate from RGB data.
- It does not perform formal validated color deconvolution.
- It does not know whether the selected tissue fields are biologically
  comparable.
- It does not replace control slide review.
- It does not replace pathologist review.
- It is affected by scanner settings, white balance, exposure, compression,
  tissue thickness, counterstain, pigment, necrosis, folds, and focus.
- It should not be used alone to release clinical results.
- It is best used as supportive documentation for research or quality review.

BEST PRACTICE SUMMARY
---------------------

For a defensible comparison:

- Use matched or comparable tissue sections.
- Use representative fields.
- Avoid artifact.
- Keep image acquisition settings consistent.
- Use Image 1 as the accepted reference.
- Use Image 2 as the new lot/run/platform.
- Review the overall percent difference.
- Review weak, moderate, and strong bucket results.
- Review QC overlays before relying on the numbers.
- Export the report and retain it with the lot-to-lot, run-to-run, or
  platform comparison record.
- Make the final decision using both numeric results and expert visual review.

SHORT VERSION
-------------

Load the reference image as Image 1 and the new lot, new run, or alternate
platform image as Image 2. Press Calculate. Review the overall mean DAB optical
density difference, direction of change, weak/moderate/strong bucket summaries,
greatest bucket-level difference, and QC overlays. Use the exported report as
supporting documentation, not as a standalone clinical decision.
