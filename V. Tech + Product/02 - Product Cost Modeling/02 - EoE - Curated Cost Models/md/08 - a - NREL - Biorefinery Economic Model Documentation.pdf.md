Here's an example of a description that appears under a link.

15 MIN READ || This paper by the National Renewable Energy Lab (NREL) details a technoeconomic model that describes the costs of ethanol production to monitor competitiveness and market potential. 

Credit: [National Renewable Energy Laboratory](http://www.nrel.gov/)

{! search-content: !}


NREL
National Renewable Energy Laboratory

Process Design and Economics for Biochemical Conversion of Lignocellulosic Biomass to Ethanol

Dilute-Acid Pretreatment and Enzymatic Hydrolysis of Corn Stover

D. Humbird, R. Davis, L. Tao, C. Kinchin,
D. Hsu, and A. Aden
National Renewable Energy Laboratory
Golden, Colorado

P. Schoen, J. Lukas, B. Olthof, M. Worley,
D. Sexton, and D. Dudgeon
Harris Group Inc.
Seattle, Washington and Atlanta, Georgia

NREL is a national laboratory of the U.S. Department of Energy, Office of Energy
Efficiency & Renewable Energy, operated by the Alliance for Sustainable Energy, LLC.

Technical Report
NREL/TP-5100-47764
May 2011

Contract No. DE-AC36-08GO28308




Process Design and Economic for Biochemical Conversion of Lignocellulosic Biomass to Ethanol
Dilute-Acid Pretreatment and Enzymatic Hydrolysis of Corn Stover

D. Humbird, R. Davis, L. Tao, C. Kinchin,
D. Hsu, and A. Aden
National Renewable Energy Laboratory
Golden, Colorado

P. Schoen, J. Lukas, B. Olthof, M. Worley,
D. Sexton, and D. Dudgeon
Harris Group Inc.
Seattle, Washington and Atlanta, Georgia

Prepared under Task No. BB07.2410

NREL is a national laboratory of the U.S. Department of Energy, Office of Energy Efficiency & Renewable Energy, operated by the Alliance for Sustainable Energy, LLC.

National Renewable Energy Laboratory
1617 Cole Boulevard
Golden, Colorado 80401
303-275-3000 • www.nrel.gov

Contract No. DE-AC36-08GO28308
Technical Report
NREL/TP-5100-47764
May 2011




NOTICE
This report was prepared as an account of work sponsored by an agency of the United States government. Neither the United States government nor any agency thereof, nor any of their employees, makes any warranty, express or implied, or assumes any legal liability or responsibility for the accuracy, completeness, or usefulness of any information, apparatus, product, or process disclosed, or represents that its use would not infringe privately owned rights. Reference herein to any specific commercial product, process, or service by trade name, trademark, manufacturer, or otherwise does not necessarily constitute or imply its endorsement, recommendation, or favoring by the United States government or any agency thereof. The views and opinions of authors expressed herein do not necessarily state or reflect those of the United States government or any agency thereof.

Available electronically at http://www.osti.gov/bridge

Available for a processing fee to U.S. Department of Energy and its contractors, in paper, from:

U.S. Department of Energy
Office of Scientific and Technical Information

P.O. Box 62
Oak Ridge, TN 37831-0062
phone: 865.576.8401
fax: 865.576.5728
email: mailto:reports@adonis.osti.gov

Available for sale to the public, in paper, from:
U.S. Department of Commerce
National Technical Information Service
5285 Port Royal Road
Springfield, VA 22161
phone: 800.553.6847
fax: 703.605.6900
email: orders@ntis.fedworld.gov
online ordering: http://www.ntis.gov/help/ordermethods.aspx

Cover Photos: (left to right) PIX 16416, PIX 17423, PIX 16560, PIX 17613, PIX 17436, PIX 17721
Printed on paper containing at least 50% wastepaper, including 10% post consumer waste.




iii
Executive Summary

The U.S. Department of Energy (DOE) promotes the production of ethanol and other liquid fuels from lignocellulosic biomass feedstocks by funding fundamental and applied research that advances the state of technology in biomass collection, conversion, and sustainability. As part of its involvement in the program, the National Renewable Energy Laboratory (NREL) investigates the production economics of these fuels.

This report describes in detail one potential biochemical ethanol conversion process, conceptually based upon core conversion and process integration research at NREL. The overarching process design converts corn stover to ethanol by dilute-acid pretreatment, enzymatic saccharification, and co-fermentation. Ancillary areas—feed handling, product recovery, wastewater treatment, lignin combustion, and utilities—are also included in the design. Detailed material and energy balances and capital and operating costs were developed for the entire process, and they are documented in this report and accompanying process simulation files, which are available to the public.

As a benchmark case study, this so-called technoeconomic model provides an absolute production cost for ethanol that can be used to assess its competitiveness and market potential. It can also be used to quantify the economic impact of individual conversion performance targets and prioritize these in terms of their potential to reduce cost. Furthermore, by using the benchmark as a comparison, DOE can make more informed decisions about research proposals claiming to lower ethanol production costs. 

Building on design reports published in 2002 and 1999, NREL, together with the subcontractor Harris Group Inc., performed a complete review of the process design and economic model for the biomass-to-ethanol process. This update reflects NREL’s current vision of the biochemical ethanol process and incorporates recent progress in the conversion areas (pretreatment, conditioning, saccharification, and fermentation), optimizations in product recovery, and an improved understanding of the ethanol plant’s back end (wastewater and utilities). The major process updates in this design report are the following: 

* Feedstock composition is updated to a carbohydrate profile closer to the expected mean.
* Pretreatment reactor configuration is revised with significant new detail.
* Whole-slurry pH adjustment of the pretreated biomass with ammonia replaced the previous conditioning practice of overliming, eliminating a solid-liquid separation step.
* Enzymatic hydrolysis and fermentation are modeled as a batch process with a continuous high-solids hydrolysis reactor upstream of the batch reactors.
* On-site enzyme production is included to increase transparency on the cost of enzymes.
* Wastewater treatment section is redesigned to handle inorganics in the ethanol stillage.

The conceptual design presented here reports ethanol production economics as determined by 2012 conversion targets and “nth-plant” project costs and financing. For the biorefinery described here, processing 2,205 dry ton/day at 76% theoretical ethanol yield (79 gal/dry ton), the ethanol selling price is $2.15/gal in 2007$.




Ethanol Production Process Engineering Analysis
Corn Stover Design Report Case: 2012 model DW1102A
Dilute Acid Pretreatment with Enzymatic Hydrolysis and Co-Fermentation
All Values in 2007$
Minimum Ethanol Selling Price (MESP): $2.15 /gal
Gasoline-Equivalent MESP: $3.27 /gal gasoline equivalent
Contributions: Feedstock $0.74 /gal
Enzymes $0.34 /gal
Non-Enzyme Conversion $1.08 /gal
Ethanol Production 61.0 MMgal/yr (Ethanol at 68 °F)
Ethanol Yield 79.0 gal / dry U.S. ton feedstock
Feedstock + Handling Cost $58.50 /dry U.S. ton
Internal Rate of Return (After-Tax) 10%
Equity Percent of Total Investment 40%

Capital Costs
Pretreatment $29,900,000
Neutralization/Conditioning $3,000,000
Saccharification & Fermentation $31,200,000
On-site Enzyme Production $18,300,000
Distillation and Solids Recovery $22,300,000
Wastewater Treatment $49,400,000
Storage $5,000,000
Boiler/Turbogenerator $66,000,000
Utilities $6,900,000
Total Installed Equipment Cost $232,000,000
Added Direct + Indirect Costs $190,500,000
(% of TCI) 45%
Total Capital Investment (TCI) $422,500,000
Installed Equipment Cost/Annual Gallon $3.80
Total Capital Investment/Annual Gallon $6.92
Loan Rate 8.0%
Term (years) 10
Capital Charge Factor (Computed) 0.131
Denatured Fuel Production (MMgal/yr) 61.7
Denatured Fuel Min. Sales Price $2.18
Denaturant Cost ($/gal denaturant) $2.10
Maximum Yields (100% of Theoretical)
Ethanol Production (MMgal/yr) 80.3
Theoretical Yield (gal/U.S. ton) 103.9
Current Yield (Actual/Theoretical) 76.0%

Manufacturing Costs (cents/gal ethanol)
Feedstock + Handling 74.1
Sulfuric Acid 2.4
Ammonia 6.5
Glucose (enzyme production) 19.3
Other Raw Materials 12.9
Waste Disposal 2.5
Net Electricity -10.8
Fixed Costs 17.5
Capital Depreciation 22.0
Average Income Tax 12.3
Average Return on Investment 56.6
Manufacturing Costs ($/yr)
Feedstock + Handling $45,200,000
Sulfuric Acid $1,500,000
Ammonia $4,000,000
Glucose (enzyme production) $11,800,000
Other Raw Materials $7,900,000
Waste Disposal $1,500,000
Net Electricity -$6,600,000
Fixed Costs $10,700,000
Capital Depreciation $13,400,000
Average Income Tax $7,500,000
Average Return on Investment $34,600,000
Specific Operating Conditions
Enzyme Loading (mg/g cellulose) 20
Saccharification Time (days) 3.5
Fermentation Time (days) 1.5
Ethanol titer (wt%) 5.4%
Excess Electricity (kWh/gal) 1.8
Plant Electricity Use (kWh/gal) 3.9
Plant Water Usage (gal/gal) 5.4

Figure ES-1. Economic summary for ethanol production




v
Table of Contents
1 Introduction........................................................................................................................................... 1
1.1 Background and Motivation ................................................................................................1
1.2 Process Overview.................................................................................................................2
1.3 Technoeconomic Analysis Approach ..................................................................................5
1.4 About nth-Plant Assumptions...............................................................................................6
1.5 Review of Related Technoeconomic Studies ......................................................................7
1.6 About the NREL Aspen Model..........................................................................................10
2 Design Basis and Conventions......................................................................................................... 12
2.1 Plant Size ...........................................................................................................................12
2.2 Feedstock Composition......................................................................................................12
2.3 Design Report Conventions ...............................................................................................15
2.3.1 Units ..........................................................................................................................15
2.3.2 Total Solids Loading.................................................................................................15
2.3.3 Ethanol Density.........................................................................................................15
2.3.4 Theoretical Yields and Conversions .........................................................................15
3 Process Design and Cost Estimation Details.................................................................................. 16
3.1 Area 100: Feedstock Storage and Handling.......................................................................16
3.1.1 Overview...................................................................................................................16
3.1.2 Design Basis..............................................................................................................17
3.1.3 Cost Estimation.........................................................................................................17
3.2 Area 200: Pretreatment and Conditioning .........................................................................19
3.2.1 Overview...................................................................................................................19
3.2.2 Design Basis..............................................................................................................20
3.2.3 Cost Estimation.........................................................................................................22
3.2.4 Achieving the Design Case .......................................................................................23
3.3 Area 300: Enzymatic Hydrolysis and Fermentation..........................................................26
3.3.1 Overview...................................................................................................................26
3.3.2 Design Basis..............................................................................................................27
3.3.3 Cost Estimation .........................................................................................................31
3.3.4 Achieving the Design Case .......................................................................................32
3.4 Area 400: Cellulase Enzyme Production ...........................................................................36
3.4.1 Overview...................................................................................................................36
3.4.2 Design Basis..............................................................................................................37
3.4.3 Cost Estimation.........................................................................................................40
3.4.4 Enzyme Cost Discussion...........................................................................................40
3.5 Area 500: Product, Solids, and Water Recovery ...............................................................44
3.5.1 Overview...................................................................................................................44
3.5.2 Design Basis..............................................................................................................45
3.5.3 Cost Estimation .........................................................................................................46
3.6 Area 600: Wastewater Treatment (WWT).........................................................................47
3.6.1 Overview...................................................................................................................47
3.6.2 Design Basis..............................................................................................................48
3.6.3 Cost Estimation .........................................................................................................50
3.6.4 Wastewater Challenges .............................................................................................50
3.7 Area 700: Product and Feed Chemical Storage .................................................................51
3.7.1 Overview...................................................................................................................51
3.7.2 Design Basis..............................................................................................................51
3.7.3 Cost Estimation.........................................................................................................51
3.8 Area 800: Combustor, Boiler, and Turbogenerator ...........................................................52
3.8.1 Overview...................................................................................................................52
3.8.2 Design Basis..............................................................................................................52
3.8.3 Cost Estimation.........................................................................................................53
3.9 Area 900: Utilities..............................................................................................................54
3.9.1 Overview...................................................................................................................54
3.9.2 Design Basis..............................................................................................................54
3.9.3 Cost Estimation .........................................................................................................56
4 Process Economics ........................................................................................................................... 57
4.1 About Cost-Year Indices....................................................................................................57
4.2 Total Capital Investment (TCI)..........................................................................................58
4.3 Variable Operating Costs...................................................................................................62
4.4 Fixed Operating Costs........................................................................................................64
4.5 Discounted Cash Flow Analysis and the Minimum Selling Price of Ethanol ...................65
5 Analysis and Discussion ................................................................................................................... 70
5.1 Carbon and Energy Balance...............................................................................................70
5.2 Water Balance....................................................................................................................74
5.3 The Cost of Sugar ..............................................................................................................76
5.4 Cost Sensitivity Analysis ...................................................................................................79
5.5 State of Technology Back-Casting ....................................................................................81
6 Concluding Remarks.......................................................................................................................... 83
6.1 Summary............................................................................................................................83
6.2 Variance from the 2002 Design .........................................................................................84
6.3 Future Work.......................................................................................................................85
References................................................................................................................................................. 87
Appendix A. Individual Equipment Costs Summary ............................................................................. 96
Appendix B. Discounted Cash Flow Rate of Return Worksheet........................................................ 103
Appendix C. Process Parameters/Operating Summary...................................................................... 106
Appendix D. Aspen Properties .............................................................................................................. 107
Appendix E. Process Flow Diagrams.................................................................................................... 114

vii
List of Figures
Figure 1. Simplified flow diagram of the overall process, PFD-P120-A000 ................................. 4
Figure 2. NREL’s approach to process design and economic analysis .......................................... 5
Figure 3. Adjusting the Kazi et al. base case ($3.40/gal) to NREL 2008 SOT assumptions........ 10
Figure 4. Structural carbohydrate distribution of the feedstock variability study [25]................. 13
Figure 5. Simplified flow diagram of the feedstock receiving system ......................................... 16
Figure 6. Simplified flow diagram of the pretreatment and conditioning process ....................... 19
Figure 7. Horizontal pretreatment reactor design scheme (Andritz, Inc.) .................................... 23
Figure 8. Simplified flow diagram of the enzymatic hydrolysis and fermentation process ......... 27
Figure 9. Simplified flow diagram of the enzyme production process......................................... 36
Figure 10. Enzyme production cost breakdown ........................................................................... 41
Figure 11. Enzyme contribution to MESP as a function of loading ............................................. 42
Figure 12. Simplified flow diagram of the separation process ..................................................... 44
Figure 13. Simplified flow diagram of the wastewater treatment process ................................... 47
Figure 14. Cooling duty distribution between major users........................................................... 55
Figure 15. Distribution of plant electricity utilization by process area......................................... 56
Figure 16. Sensitivity of MESP to IRR and % equity (8% interest on a 10-year loan)................ 66
Figure 17. Cost contribution details from each process area (per gallon EtOH).......................... 69
Figure 18. Mass, carbon, and energy balance diagram for the overall process ............................ 73
Figure 19. Economic summary for dilute sugar production ......................................................... 78
Figure 20. Single-point sensitivity tornado charts for (a) MESP and (b) ethanol yield ............... 80
Figure 21. Sugar-based pathways for conventional and advanced biofuels ................................. 86

viii
List of Tables
Table 1. Comparison of Technoeconomic Analyses and Market Studies for Existing Biofuels.... 7
Table 2. Survey of Recent Technoeconomic Studies on Biochemical Cellulosic Ethanol ............ 9
Table 3. Summary of Whole Stover Composition Data ............................................................... 13
Table 4. Corn Stover Composition from the 2002 Design [2] and the Present Design................ 14
Table 5. Pretreatment Reactor Conditions.................................................................................... 21
Table 6. Pretreatment Hydrolysis Reactions and Assumed Conversions..................................... 22
Table 7. Research Status and 2012 Targets in the Pretreatment Area.......................................... 24
Table 8. Enzymatic Hydrolysis Conditions .................................................................................. 28
Table 9. Enzymatic Hydrolysis Reactions and Assumed Conversions ........................................ 28
Table 10. Seed Train Specifications ............................................................................................. 29
Table 11. Seed Train Reactions and Assumed Conversions......................................................... 29
Table 12. Co-Fermentation Contamination Loss Reactions......................................................... 30
Table 13. Co-Fermentation Conditions......................................................................................... 31
Table 14. Co-Fermentation Reactions and Assumed Conversions............................................... 31
Table 15. Research Status and 2012 Targets in Enzymatic Hydrolysis and Fermentation .......... 32
Table 16. Summary of Integrated Whole-Slurry Enzymatic Hydrolysis Performance Using an
Advanced Enzyme Preparation..................................................................................................... 33
Table 17. Ethanol Yields from Xylose ......................................................................................... 34
Table 18. Area 400 Guiding Design Basis Assumptions.............................................................. 37
Table 19. Specifications of the Enzyme Production Bioreactors ................................................. 39
Table 20. Cellulase Production Nutrient Requirements ............................................................... 39
Table 21. Cellulase Production Electricity Requirements ............................................................ 40
Table 22. Wastewater Treatment System Design Basis ............................................................... 48
Table 23. Storage Requirements................................................................................................... 51
Table 24. Cooling Water Users..................................................................................................... 54
Table 25. Installation Factors........................................................................................................ 59
Table 26. Scaling Exponents......................................................................................................... 60
Table 27. Additional Costs for Determining Total Capital Investment (TCI).............................. 61
Table 28. Project Cost Worksheet Including Total Direct Costs and Total Capital Investment .. 62
Table 29. Chemical Costs and Sources......................................................................................... 63
Table 30. Variable Operating Costs.............................................................................................. 63
Table 31. Fixed Operating Costs .................................................................................................. 64
Table 32. Construction Activities and Cash Flow ........................................................................ 67
Table 33. Discounted Cash Flow Analysis Parameters ................................................................ 68
Table 34. Summary of Yields, Rates, and Conversion Costs ....................................................... 69
Table 35. Ethanol Plant Overall Carbon Balance ......................................................................... 70
Table 36. Ethanol Plant Overall Energy Balance ......................................................................... 71
Table 37. Ethanol Plant Water Balance ........................................................................................ 75
Table 38. Individual Contributors to Cooling Water Evaporation ............................................... 75
Table 39. Mixed Sugar Stream Composition................................................................................ 77
Table 40. Assumptions Varied in the Sensitivity Analysis........................................................... 79
Table 41. Back-Casted State of Technology Cases and Future Targets....................................... 82
Table 42. Comparison of the Previous Target Case and the Present Design (2007$/gal)............ 84
Table 43. Individual Contributors to the Change in MESP.......................................................... 85

ix
Acronyms
AFEX ammonia fiber explosion
BFW boiler feed water
BLS Bureau of Labor Statistics
C5/C6 refers to mixtures of xylose (a C5 sugar) and glucose (a C6 sugar)
CBP consolidated bioprocessing
CIP clean-in-place
COD chemical oxygen demand
CSL corn steep liquor
DAP diammonium phosphate
DCFROR discounted cash flow rate of return
DOE U.S. Department of Energy
FCI fixed capital investment
FGD flue gas desulfurization
HHV higher heating value
HMF 5-hydroxymethyl furfural
INL Idaho National Laboratory
IRR internal rate of return
ISBL inside battery limits (of the plant)
LHV lower heating value
MESP minimum ethanol selling price
MM million (e.g., MMBtu or $__MM)
MSSP minimum sugar selling price
MYPP OBP’s Multi-Year Program Plan
NPV net present value
NREL National Renewable Energy Laboratory
OBP Office of the Biomass Program
OTR oxygen transfer rate
OUR oxygen uptake rate
PCS pretreated corn stover
PFD process flow diagram
SCFM standard cubic feet per minute
SHF separate (or sequential) hydrolysis and fermentation
SOT annual State of Technology case
SSCF simultaneous saccharification and co-fermentation
TCI total capital investment
TDC total direct cost
TE technoeconomic
VOC volatile organic compound
VVM volume (of gas) per volume (of liquid) per minute
WWT wastewater treatment




1
1 Introduction

1.1 Background and Motivation

The U.S. Department of Energy (DOE) Office of the Biomass Program (OBP) promotes the production of ethanol and other liquid fuels from lignocellulosic feedstocks by sponsoring programs in fundamental and applied research that aim to advance the state of biomass conversion technology. These programs include laboratory campaigns to develop better cellulose hydrolysis enzymes and fermenting microorganisms, detailed engineering studies of potential processes, and construction of pilot-scale demonstration and production facilities. This research is conducted by national laboratories, universities, and private industry in conjunction with engineering and construction companies.

As part of its involvement in the program, the National Renewable Energy Laboratory (NREL) investigates the complete process design and economics of cellulosic ethanol manufacturing in order to develop an absolute plant-gate price for ethanol based on process and plant design assumptions consistent with applicable best practices in engineering, construction, and operation. This plant-gate price is referred to as the minimum ethanol selling price or MESP. The MESP can be used by policymakers and DOE to assess the cost-competitiveness and market penetration potential of cellulosic ethanol in comparison with petroleum-derived fuels and starch- or sugar based ethanol.

The technoeconomic analysis effort at NREL also helps to direct our biomass conversion research by examining the sensitivity of the MESP to process alternatives and research advances. Proposed research and its anticipated results can be translated into a new MESP that can be compared to the benchmark case documented in this report. Such comparison helps to quantify the economic impact of core research targets at NREL and elsewhere and to track progress toward meeting competitive cost targets. It also allows DOE to make more informed decisions about research proposals that claim to reduce MESP.

This report builds upon previous issues from 1999 [1] and 2002 [2] written by NREL engineers with Delta-T, Merrick Engineering, Reaction Engineering, Inc., and Harris Group. For the present report, NREL again contracted Harris Group to provide engineering support for estimating and reviewing the equipment and raw material costs used in the process design. This update reflects NREL’s latest envisioned biochemical ethanol process and includes recent research progress in the conversion areas (pretreatment, conditioning, enzymatic hydrolysis, and fermentation), optimizations in product recovery, and our latest understanding of the ethanol plant’s back end (separation, wastewater, and utilities). NREL worked with Harris Group to identify realistic configurations and costs for critical equipment, the pretreatment reactor system in particular. An on-site cellulase enzyme section was included in this update to permit better transparency of enzyme economics than the fixed cost contribution assumed in the last design report did.

The biomass conversion efficiencies used in the design (e.g., cellulose to glucose or xylose to ethanol) are based on a slate of research targets that NREL and DOE have committed to demonstrate by the end of 2012 in a campaign of integrated pilot-scale runs. These 2012 performance targets are discussed in detail in this report. The economics of this conceptual process use the best available equipment and raw material costs and an “nth-plant” project cost structure and financing. The projected 2012 nth-plant MESP computed in this report is $2.15/gal in 2007$.

2
Modifications to the conceptual process design presented here will be reflected annually through NREL’s State of Technology (SOT) reports. These ensure that the process design and its cost benchmark incorporate the most current data from NREL and other DOE-funded research and that equipment costs stay up-to-date.

We stress that this design report serves to describe a single, feasible cellulosic ethanol conversion process and to transparently document the assumptions and details that went into its design. This report is not meant to provide an exhaustive survey of process alternatives or cost sensitivity analyses. These will be investigated in separate papers that extend and reference the present report. Furthermore, the process models and economic tools developed for this report are available to the public, and the authors and members of NREL’s Biochemical Platform Analysis task will provide support to researchers who wish to use them for their own studies. 

1.2 Process Overview

The process described here uses co-current dilute-acid pretreatment of lignocellulosic biomass (corn stover), followed by enzymatic hydrolysis (saccharification) of the remaining cellulose, followed by fermentation of the resulting glucose and xylose to ethanol. The process design also includes feedstock handling and storage, product purification, wastewater treatment, lignin combustion, product storage, and required utilities. The process is divided into nine areas (see Figure 1).

* Area 100: Feed handling. The feedstock, in this case milled corn stover, is delivered to the feed handling area from a uniform-format feedstock supply system. Only minimum storage and feed handling are required. From there, the biomass is conveyed to the pretreatment reactor (Area 200).
* Area 200: Pretreatment and conditioning. In this area, the biomass is treated with dilute sulfuric acid catalyst at a high temperature for a short time to liberate the hemicellulose sugars and break down the biomass for enzymatic hydrolysis. Ammonia is then added to the whole pretreated slurry to raise its pH from ~1 to ~5 for enzymatic hydrolysis. 
* Area 300: Enzymatic hydrolysis and fermentation. Enzymatic hydrolysis is initiated in a high-solids continuous reactor using a cellulase enzyme prepared on-site. The partially hydrolyzed slurry is next batched to one of several parallel bioreactors. Hydrolysis is completed in the batch reactor, and then the slurry is cooled and inoculated with the co fermenting microorganism Zymomonas mobilis. After a total of five days of sequential enzymatic hydrolysis and fermentation, most of the cellulose and xylose have been converted to ethanol. The resulting beer is sent to the product recovery train (Area 500). 
* Area 400: Cellulase enzyme production. An on-site enzyme production section was included in this design. Purchased glucose (corn syrup) is the primary carbon source for enzyme production. Media preparation involves a step in which a portion of the glucose is converted to sophorose to induce cellulase production. The enzyme-producing fungus (modeled after Trichoderma reesei) is grown aerobically in fed-batch bioreactors. The entire fermentation broth, containing the secreted enzyme, is fed to Area 300 to carry out enzymatic hydrolysis.

3

* Area 500: Product recovery. The beer is separated into ethanol, water, and residual solids by distillation and solid-liquid separation. Ethanol is distilled to a nearly azeotropic mixture with water and then purified to 99.5% using vapor-phase molecular sieve adsorption. Solids recovered from the distillation bottoms are sent to the combustor (Area 800) while the liquid is sent to wastewater treatment (Area 600).
* Area 600: Wastewater treatment. Plant wastewater streams are treated by anaerobic and aerobic digestion. The methane-rich biogas from anaerobic digestion is sent to the combustor (Area 800), where sludge from the digesters is also burned. The treated water is suitable for recycling and is returned to the process.
* Area 700: Storage. This area provides bulk storage for chemicals used and produced in the process, including corn steep liquor (CSL), ammonia, sulfuric acid, nutrients, water, and ethanol.
* Area 800: Combustor, boiler, and turbogenerator. The solids from distillation and wastewater treatment and the biogas from anaerobic digestion are combusted to produce high-pressure steam for electricity production and process heat. The majority of the process steam demand is in the pretreatment reactor and distillation columns. The boiler produces excess steam that is converted to electricity for use in the plant and for sale to the grid.
* Area 900: Utilities. This area includes a cooling water system, chilled water system, process water manifold, and power systems.


4
Figure 1. Simplified flow diagram of the overall process, PFD-P120-A000
A100 FEED HANDLING
A200 PRETREATMENT & CONDITIONING
A400 ENZYME PRODUCTION
A300 ENZYMATIC HYDROLYSIS AND FERMENTATION
A500 DISTILLATION DEHYDRATION SOLIDS SEPARATION
A700 STORAGE
A800 BURNER/BOILER TURBOGENERATOR
A600 WASTEWATER TREATMENT
A900 UTILITIES
MAR 2011 PFD-P120-A000
OVERALL PROCESS: CORN STOVER TO ETHANOL
RAW FEEDSTOCK
FEEDSTOCK
RECYCLE
WATER
NUTRIENTS
AUX. FUEL
ANAEROBIC BIOGAS
STEAM
ELECTRICITY
STEAM
CELLULASE
HYDROLYSATE
AMMONIA
STEAM
ACID
GLUCOSE
NUTRIENTS
VENT
NUTRIENTS
EVAPORATION
FLASH
CONDENSATE
STILLAGE
LIGNIN
BEER
VENT
EtOH PRODUCT


5
1.3 Technoeconomic Analysis Approach

Figure 2 describes the engineering approach used here for modeling the conversion of biomass to ethanol, including process design, process modeling, and economic analysis.

Process Flow Diagrams
Rigorous Material & Energy Balances (Aspen Plus)
Capital & Project Cost Estimation
Discounted Cash Flow Economic Model
Minimum Ethanol Selling Price
Engineering Companies Consulting on Process Configuration
Estimates of Other Commercial Technology
Cost Estimation Software (e.g., ICARUS)
Engineering Company Cost Estimations
NREL or other DOE-Sponsored Research
Vendor Cost Quotations
Outside Engineering Studies (e.g., feed handling, separations)


Figure 2. NREL’s approach to process design and economic analysis

Starting from the general process flow diagram (PFD) shown in Figure 1 and the more detailed PFDs contained in Appendix E, a process simulation is developed using Aspen Plus software [3]. This process model computes thermodynamically-rigorous material and energy balances for each unit operation in this conceptual biorefinery.

The material and energy balance data from the Aspen simulation are next used to assist in determining the number and size of capital equipment items. As process conditions and flows change, baseline equipment costs are automatically adjusted in an Excel spreadsheet using a scaling exponent. These baseline costs come from vendor quotes (favored for larger or non standard unit operations and packaged or skid-mounted subsystems) or from Harris Group’s proprietary cost database (for secondary equipment such as tanks, pumps, and heat exchangers). Final equipment costs for this report are tabulated in Appendix A.

6
Once equipment costs are determined, direct and indirect overhead cost factors (e.g., installation costs and project contingency) are applied to determine a total capital investment (TCI). The TCI, along with the plant operating expenses (also developed using flow rates from the Aspen model), is used in a discounted cash flow rate of return (DCFROR) analysis to determine a plant gate price for ethanol for a given discount rate. This plant-gate price is also called the minimum ethanol selling price (MESP, $/gallon) required to obtain a net present value (NPV) of zero for a 10% internal rate of return (IRR) after taxes.

The product of the analysis described above is a technoeconomic model that reasonably estimates a product price for a pre-commercial process. The resultant MESP is unique for the set of process conditions simulated and it should be emphasized that a certain percentage of uncertainty always exists around these chosen conditions, as well as around the assumptions made for capital and raw material costs. Without a detailed understanding of the basis behind it, the absolute computed MESP has limited relevance. While the MESP can be used to assess the marketplace competiveness of a given process, it is best suited for comparing technological variations against one another or for performing sensitivity analyses that indicate where economic or process performance improvements are needed. 

1.4 About nth-Plant Assumptions

The technoeconomic analysis reported here uses what are known as “nth-plant” economics. The key assumption implied by nth-plant economics is that our analysis does not describe a pioneer plant; instead, several plants using the same technology have already been built and are operating. In other words, it reflects a mature future in which a successful industry of n plants has been established. Because the technoeconomic model is primarily a tool for studying new process technologies or integration schemes in order to comment on their comparative economic impact, we feel it is prudent to ignore artificial inflation of project costs associated with risk financing, longer start-ups, equipment overdesign, and other costs associated with first-of-a-kind or pioneer plants, lest these overshadow the real economic impact of research advances in conversion or process integration. At the very least, these nth-plant economics should help to provide justification and support for early technology adopters and pioneer plants.

In previous design reports that targeted 2012 technology, many of the nth-plant assumptions also applied to key 2012 research targets in conversion, e.g., 90% conversion of xylan to xylose, which in 2002 had not yet been experimentally demonstrated. This report will show that through research progress, current conversion performance is approaching the targets set in 2002 and that the 2012 performance targets should no longer be considered speculative. Assumptions in the previous model also extended to enzyme costs and some equipment costs, particularly those items that were not commercially available at the time (e.g., the pretreatment reactor). In the present design report, enzyme and equipment costs are considerably more well-defined. The remaining nth-plant assumptions in the present model therefore apply primarily to the factored cost model used to determine the total capital investment from the purchased equipment cost and to the choices made in plant financing. The nth-plant assumption also applies to some operating parameters, such as process uptime of 96%. These assumptions were agreed upon by NREL and DOE for this report and reflect our best estimates at the time of publication. It should be emphasized, however, that these assumptions carry a large uncertainty and are subject to refinement.

7
1.5 Review of Related Technoeconomic Studies

Tao and Aden [4] performed a survey of technoeconomic models of existing biofuels (corn ethanol, sugarcane ethanol, and conventional soy biodiesel) from the literature. These studies were normalized to a consistent year-dollar value and feedstock cost (where applicable) and compared to published market studies. This comparison, shown in Table 1, indicated that technoeconomic analysis was able to predict the actual cost of production of these biofuels within the expected accuracy of such models.

Table 1. Comparison of Technoeconomic Analyses and Market Studies for Existing Biofuels
Fuel Market Study TE Model
Corn ethanol $1.53/gal a $1.54/gal b
Sugarcane ethanol $1.14/gal a $1.29/gal c
Soy biodiesel $2.15/gal d $2.55/gal e
a F.O. Lichts, 2007 [5].
b Kwiatkowski et al., 2006 [6].
c Rodrigues, 2007 [7]; Seabra, 2007 [8].
d Graboski & McCormick, 1998 [9].
e Haas et al., 2006 [10].

The quantitative agreement in Table 1 is not altogether surprising, because the developers of these models were able to compare their results to real economics and make adjustments as necessary. (Also, for these particular fuels, feedstock makes up the largest part of the production cost, so uncertainty in the remaining non-feedstock conversion costs is not as obvious.) Developing a technoeconomic model for a pre-commercial technology, such as the corn-stover to-ethanol process described in this report, requires a more ab initio approach, rooted in a thorough understanding of the state of the technology at the time of the analysis and good engineering practice.

In the years since the last NREL design report in 2002, several newer technoeconomic studies of biochemical cellulosic ethanol production have been published. Many of these studies were based to varying degrees on NREL’s previous design report, borrowing from its process assumptions, cost information, or both. This was in fact the principal goal of the earlier NREL design reports: to establish a baseline or “zero-point” technoeconomic benchmark from which process alternatives and improvements could be evaluated by others in the public realm. The present report now aims to establish a new zero-point and thereby serve a similar purpose for analyses going forward.

A brief survey of MESPs from recent technoeconomic studies of biochemical cellulosic ethanol production is presented in Table 2; note that these studies were not normalized to a consistent cost-year but were all published between 2008 and 2010, so cost-year differences should be minor. Clearly, there is a wide range of published MESP values within this subset of papers. For the most part, these are due to differences in feedstock cost, process assumptions, and co-product values, all of which vary considerably across the studies. For example, the analysis by Laser et al. [11] assumes a fairly low feedstock cost and very high yields (indicating aggressive process assumptions) as well as improved economies of scale (if such a high feed rate can be sustained), while also receiving positive revenue from higher-value co-products such as protein and hydrogen. Furthermore, this study assumes a consolidated bioprocessing (CBP) approach, which—although less developed than separate saccharification and co-fermentation—could further improve economics by reducing enzyme costs. Conversely, studies on the high end of the MESP range such as Kazi et al. [12] and Klein-Marcuschamer et al. [13] assumed higher feedstock costs while achieving much lower ethanol yields. Compared to NREL’s 2002 design report (upon which many of its cost inputs were based), the Klein-Marcuschamer study’s base case assumes much longer batch times for saccharification and fermentation (thus higher associated capital costs), higher enzyme costs, and a lower carbohydrate fraction in the feedstock (contributing to lower yields) [14].
8

Table 2. Survey of Recent Technoeconomic Studies on Biochemical Cellulosic Ethanol
Source  MESP ($/gal)  Feedstock   Scale (dry ton/day) Feed Price ($/dry ton)  Ethanol Yield (gal/dry ton) Notes
NREL 2002 Design Report (2007$) [2] 1.49 Corn stover 2,200 51 90  Dilute-acid pretreatment, SSCF process, electricity co-product
NREL 2011 Design Report (this work) 2.15 Corn stover 2,200 59 79  Dilute-acid pretreatment, SHF process, electricity co-product
Kazi [12] 3.40-4.44 Corn stover 2,200 75 42-72 Varying pretreatment options and downstream process assumptions
Huang [15] 1.42-1.87 Aspen, poplar, corn stover, switchgrass  2,200 58-100 83-111 Dilute-acid pretreatment
Sendich [16] 1.03-1.41 Corn stover 2,200 40 70 AFEX pretreatment, SSCF process, varying process conditions
Sendich [16] 0.80-0.95  Corn stover 2,200 40 78 AFEX pretreatment, CBP process, varying process conditions
Laser [11] 0.63-0.83 Switchgrass 5,000 44 97-105 AFEX pretreatment, CBP process, varying pathways and co products
Gnansounou [17] 2.12-2.91 Straw, eucalyptus, poplar, switchgrass  1,760-2,200 57-127 70-84 Dilute-acid pretreatment
Bals [18] 1.86-2.20 Corn stover 850 45 78 AFEX pretreatment, varying pretreatment conditions
Piccolo [19] 3.43-4.03 Hardwood 2,200 65 75 Dilute-acid pretreatment, varying financial inputs 
Klein Marcuschamer [13]   3.53-4.58 Corn stover 1,700 60 52-74 Dilute-acid pretreatment, varying feed compositions and process conditions
National Academy of Sciences [20] 1.20-2.70 (COP) Poplar and “high glucan” 1,000-1,600  50-88 67-106 Hot water pretreatment, Cost of Production analysis (COP<MESP)


To further demonstrate the impact of such assumptions, we turn to the study of Kazi et al. [12], a joint effort between Iowa State University, ConocoPhillips, and NREL. While this paper examined a variety of pretreatment and downstream processing alternatives, its baseline was essentially NREL’s 2008 State of Technology (SOT) model (dilute-acid pretreatment, purchased cellulase enzyme, and C5/C6 co-fermentation) [21]. The Kazi et al. study adjusted several key parameters from the 2008 SOT model to incorporate external public data. The feedstock cost, enzyme cost, indirect capital cost factors, and reaction conversions were all modified per data external to NREL analysis. While both analyses were intended to represent near-term or “state of technology” economics extrapolated to an nth plant as discussed previously, the assumptions in the Kazi et al. study were generally more conservative than NREL’s 2008 SOT, raising the MESP considerably. Adjusting for these key economic assumptions, their MESP closely approaches that of the NREL 2008 SOT case, as shown in Figure 3. In many cases, economic variance between technoeconomic studies is easily explained by normalizing for a few important inputs

$3.40
$2.50
$0.23
$0.38
$0.29
$1.00
$1.50
$2.00
$2.50
$3.00
$3.50
$4.00
Kazi et al. (published)
Indirect capital costs (adjust to 2008 SOT)
Enzyme cost (70→32¢/gal) 
Feedstock price ($75→$60/ton)
Kazi et al. (adjusted)
MESP (2007$/gal)
2008 SOT = $2.43/gal

Figure 3. Adjusting the Kazi et al. base case ($3.40/gal) to NREL 2008 SOT assumptions


10
1.6 About the NREL Aspen Model

The final version of the Aspen model used to generate this design report is named DW1102A; this version will be made publicly available along with this design report. We note that it is not uncommon to find subtle differences in Aspen results between software versions and patch levels. The results presented here were obtained with model DW1102A on Aspen Plus V7.2, patch level 0.

While Aspen can be completely rigorous, such detail is not always warranted in our simulation. Some unit operations, particularly solid-liquid separation, were modeled with a fixed performance determined by vendor testing. Bioreactors were modeled using experimentally determined conversions of specific reactions (e.g., cellulose to glucose) rather than using rigorous kinetics or rate expressions. This simple stoichiometric model still satisfies mass and energy balances.

11
The Aspen Plus simulation uses component physical properties internal to the software as well as property data developed at NREL or from the literature [22, 23]. Since the 2002 model was created, we have taken steps to reduce the number of custom-defined components and have eliminated the external property databanks. A discussion of the components and properties used is given in Appendix D.

12
2 Design Basis and Conventions

2.1 Plant Size

The plant size in the present design is the same as in the 2002 design: 2,205 dry U.S. ton/day (2,000 metric tonne/day). With an expected 8,410 operating hours per year (96% uptime), the annual feedstock requirement is 773,000 dry U.S. ton/year. The 2002 study assumed that an ethanol plant would be responsible for collecting and storing its own corn stover supply for the year, and 2,205 dry ton/day represented a 50-mile corn stover collection radius, assuming that 10% of the biomass within that radius was available to the plant.

In the present design, feedstock is assumed to be delivered to the plant from a satellite storage and processing facility like the pioneer uniform-format facility described by Idaho National Laboratory (INL) [24]. That facility is designed to supply 882,000 dry U.S. ton/yr of biomass; enough to supply one of the ethanol plants described here or multiple smaller facilities. We have not repeated the plant-size sensitivity study from the 2002 report, which indicated that only modest cost reductions due to economies of scale could be achieved beyond 2,205 ton/day. Although the absolute MESP is different in the present report, we expect that the plant-size trends observed in the 2002 report are still valid.

2.2 Feedstock Composition

The feedstock type and composition can have significant impacts on the overall process design and economics. Feedstock type may influence the design of key components in the conversion process, e.g., the pretreatment reactor. Feedstock composition, from a potential sugar perspective, clearly affects the ethanol yield. The feedstock used for this analysis was corn stover. Stover is a generic term that refers to the “rest” of the corn plant, i.e., everything above the ground that is not a kernel of corn: leaves, stalks, husks, cobs, etc. NREL biochemical conversion research has focused on corn stover primarily because it is the most abundant agriculture residue in the U.S. and is thus readily available. While dedicated energy crops like switchgrass may ultimately have sustainability and yield advantages over agricultural residues like corn stover, these crops are currently not available in the large volumes required for pilot scale research.

Corn stover can vary in composition and moisture content due to corn variety, region, weather, soil type, fertilization practices, harvesting and storage practices, time in storage, and so on. A recent NREL study assessed the compositions of corn stovers from many commercial hybrid corn varieties using a rapid compositional analysis method known as near-infrared spectroscopy/projection-to-latent-structures modeling (NIR/PLS) [25]. This study evaluated the compositions of 508 commercial corn stover samples collected from 47 sites in eight Corn Belt states after the 2001, 2002, and 2003 harvests. From this study, the average concentrations (dry wt %) of the major stover components were 32% glucan, 19% xylan, 18% solubles, and 13% lignin (corrected for protein). These composition results are summarized in Table 3 along with the characteristic variation of each component. Figure 4 shows the distribution of total structural carbohydrate content among the samples.

Table 3. Summary of Whole Stover Composition Data
Component Average
(dry wt %)
Min Max Range
Ethanol solubles 3.3 1.7 4.1 2.4
Sucrose 3.6 0 10 10
Extractable inorganics (soil) 2.5 0 4.8 4.8
Other water extractables 8.6 1.4 15.7 14.2
Total solubles 17.9 5.7 30.8 25
Glucan 31.9 26.5 37.6 11
Xylan 18.9 14.8 22.7 7.9
Galactan 1.5 0.8 1.9 1.1
Arabinan 2.8 1.6 3.6 2
Mannan 0.3 0 0.7 0.7
Lignin (corrected for protein) 13.3 11.2 17.8 6.6
Structural inorganics 3.9 0.8 6.6 5.8
Protein 3.7 1.1 5.4 4.3
Acetyl 2.2 0.9 2.9 2
Estimated uronic acids 3.1 2.5 3.7 1.2
Total structurals 81.6 70.4 90.8 20.4
Component closure 99.5 93.8 104.9 11.1
Total Structural Carbohydrates + Sucrose (dry wt %)
52 54 56 58 60 62 64
Frequency
0
10
20
30
40
50 Design
Composition
Figure 4. Structural carbohydrate distribution of the feedstock variability study [25]

13
Table 4 compares the composition used in the 2002 design to the composition used in the present design. The composition used in the 2002 design was based on an average of nine stover samples obtained from two batches [26]. Compared with the data in Table 3, its glucan, xylan, and lignin concentrations were each higher than the more recent study’s averages for those components and near or above the maximum concentration measured in the 508 stover samples. (The earlier corn stover was handled extremely carefully between the field and the lab, while the samples from the more recent study were collected from the fields well after harvest.) The composition chosen for the present design was based on a single sample taken from the overall distribution. As indicated in Figure 4, this composition fits well inside the carbohydrate distribution of the more recent study and therefore provides a more representative design basis. The moisture content value assumed for corn stover was also updated to 20% based on the feedstock logistics specifications table developed by INL and reported in the OBP Multi-Year Program Plan (MYPP) [27].

14
Table 4. Corn Stover Composition from the 2002 Design [2] and the Present Design
Component 2002 Design
(dry wt %)
Present Design
(dry wt %)
Glucan 37.40 35.05
Xylan 21.07 19.53
Lignin 17.99 15.76
Ash 5.23 4.93
Acetatea 2.93 1.81
Protein 3.10 3.10
Extractives 4.68 14.65
Arabinan 2.92 2.38
Galactan 1.94 1.43
Mannan 1.56 0.60
Sucrose - 0.77
Unknown soluble solidsb 1.18 -
Total structural carbohydrate 64.89 58.99
Total structural carbohydrate + sucrose 64.89 59.76
Moisture (bulk wt %) 15.0 20.0
a Represents acetate groups present in the hemicellulose polymer; converted to acetic acid in pretreatment.
b In the 2002 design, unknown soluble solids were calculated by difference to close the mass balance. This is now included in the extractives component.

When converting the analytical composition to components used in the Aspen model, the water and ethanol-soluble fractions from the compositional analysis were combined under “extractives.” The extractives component is assumed to be organic, with an average composition of CH2O, and consists primarily of sugars, sugar alcohols, and organic acids [28]. The presence of extractives in corn stover depends on the time of harvest and in part to how much microbial degradation of the material occurs after harvest; the amount of extractives in a given sample may therefore be indicative of its age. Additionally, where the mass balance did not sum to 100%, the extractives component was used to close it by difference. (In the 2002 design, the “unknown soluble solids” component performed this function.) Sucrose is another extractive component, but it is measured separately in laboratory analysis and has been added as a feedstock component in the present design; it is therefore excluded from the extractives component. The amount of sucrose present in corn stover is highly dependent on harvesting and handling practices. In pretreatment, this sucrose is assumed to be fully hydrolyzed to glucose and fructose. The fructose is further converted to degradation products in pretreatment, but the glucose resists degradation and thus is available for fermentation [29].

The differences in composition between the 2002 design and the present design have a few notable economic implications. Because the glucan (cellulose) content in the feedstock is lower, the present design has a lower ethanol yield per ton of feedstock. On the whole, the total structural carbohydrate composition (glucan + hemicellulose components) is about 5% lower than in the 2002 composition. Conversely, in the present design, a larger portion of the feedstock is non-carbohydrate organic compounds. These ultimately become process residues that are burned to provide heat and electricity. The amount of electricity generated per ton of feedstock processed is therefore higher than in the 2002 design (though less electricity is exported as a co product because the present design has a higher internal electricity demand).

15
2.3 Design Report Conventions

2.3.1 Units

The Aspen model we developed is, by legacy, based on the set of units required by Aspen for specifying custom component properties: kg, kmol, atm, °C for materials, and MMkcal (Gcal) for energies. Values in this report that were pulled directly from the Aspen model therefore tend to be reported in these units. Harris Group preferred to use U.S. standards (lb, Btu, °F, gal, etc.) when communicating with equipment vendors. Therefore, equipment specifications tend to be cited in these U.S. units. We have made an effort to cite both sets of units in this report, to the degree that it does not distract from the discussion.

Note that in the present report, certain quantities (e.g., yields and costs) are computed and reported in terms of “tons.” To avoid ambiguity, tonne will denote a metric tonne (1,000 kg) and ton will denote a short or U.S. ton (2,000 lb). In general, the U.S. ton is the standard for this document. “Ton” also appears in Section 3.9 in the context of refrigeration, but this usage should be clear from the discussion.

2.3.2 Total Solids Loading

The process described here converts a solid feedstock (corn stover) into a liquid product (ethanol). Most material streams in the process therefore have a solid fraction and a liquid fraction. The relative amount of solids in a given stream is called its “solids loading.” Total solids loading is defined as the total weight percent of soluble solids (e.g., sugars and salts) and insoluble solids (e.g., cellulose and lignin) in a given material stream. Where useful, the total solids loading and the insoluble solids loading will be reported together. Note that in our convention, sulfuric acid, acetic acid, and ammonia are not considered soluble solids but ammonium acetate and ammonium sulfate are. Therefore, around some unit operations, e.g., hydrolysate conditioning, total solids loading is not a conserved quantity. 

2.3.3 Ethanol Density

The most important results from this analysis are reported in terms of volume of ethanol produced: $/gal, gal/yr, gal/ton, etc. To avoid errors in these quantities that may arise from using the ethanol density computed by Aspen Plus, an accepted value was used for anhydrous ethanol at 20°C (68°F): 0.789 kg/L [30].

2.3.4 Theoretical Yields and Conversions
The terms “yield” and “conversion” are used throughout this report to describe the extent of various chemical and biochemical reactions. It should be understood that each of these quantities is a percentage of the theoretical. For example, the statement “95% conversion of glucose to ethanol” means that 95% of the glucose in the system was consumed in the following reaction: 

Glucose  2 Ethanol + 2 CO2

which has a theoretical yield of 0.51 g ethanol / g glucose.

16
3 Process Design and Cost Estimation Details

The process design described in this study was based upon demonstrated performance andplanned performance goals from DOE’s core R&D efforts in biochemical conversion. This  section describes the process in detail and discusses the influence of specific R&D goals in the decision-making process.

3.1 Area 100: Feedstock Storage and Handling

3.1.1 Overview

Area 100 handles incoming biomass feedstock. In contrast to the 2002 design, which assumed bale delivery and yard storage of corn stover followed by milling and washing, the present design assumes that corn stover is delivered according to the specifications detailed in the Idaho National Laboratory (INL) design report for the pioneer uniform-format feedstock supply system [24]. In this envisioned design, biomass is stored in a central depot and is preprocessed and homogenized to a degree before delivery, such that the biorefinery receives feedstock with known, uniform-format specifications including particle size distribution, moisture content, and bulk density.

Harris Group designed the receiving and handling system in Area 100 based on this delivery specification, using the INL design report as well as its own experience with the required equipment. The equipment in Area 100 is physically located at the ethanol plant and consists of weighing and unloading stations for incoming biomass supply trucks, short-term queuing storage, and conveyors for feeding bulk feedstock to the pretreatment reactor. A simplified process flow diagram for this area is shown in Figure 5, and more detail is given in PFD-P120-A101 (Appendix E).

Figure 5. Simplified flow diagram of the feedstock receiving system
To pretreatment
Concrete storage dome
Dust collection
Truck tipper Milled corn stover

17
3.1.2 Design Basis

In the uniform-format feedstock supply system design, feedstock would be stored in a satellite depot location with delivery to the biorefinery occurring six days a week by truck or possibly by rail. At the depot, material would be milled to a mean size of 0.16–0.23 in. (with a high content of fines), in order to achieve a mean bulk density of 9–11 lb/ft3 to maximize the biomass load per trailer. The incoming corn stover feedstock is assumed to have 20% moisture when it reaches the biorefinery; this is representative of a mixture of field-dried material having <15% moisture and co-harvested material having >20% moisture. Because the preprocessing operation is designed to lose very little dry matter and does not include any rinsing of biomass, it is assumed that the corn stover composition discussed in Section 2.2 is valid for the delivered material. We also note that the particle size of <0.25 in. is consistent with the material currently used in NREL pretreatment research.

The as-received corn stover feed requirement for the plant is 2,756 U.S. ton/day (104,200 kg/h; 229,700 lb/h) including moisture. In the projected design, refinery receiving operates on the same schedule as the biomass depot: 24 hours a day, six days a week. Each truck trailer holds 10 U.S. tons of biomass. To satisfy production and storage requirements, the plant must receive 12 trucks every hour. Incoming trucks are weighed by electronic scale (M-101) and unloaded using a whole-truck dumper (M-102) capable of a 7–10 minute unloading time. The dumpers empty into dedicated hoppers (M-103), which meter the biomass to a series of conveyors (C-101, C-102, C-103). These carry material from the truck tipper to short-term storage. The minimum receiving rate is 244 ton/h to maintain 114 ton/h of continuous processing. Because trucks are not unloaded continuously, some extra capacity needs to be built into the conveyor that carries material from the truck dumpers to storage (minimum 330–440 ton/h recommended). In order to process 244 ton/h, and assuming a relatively constant flow of trucks, a pair of scales (one inbound and one outbound) and two truck dumpers are required.

On-site storage is kept to a minimum of 72 hours to allow for a weekend buffer. Open piles are not favored due to concerns of fire, rodent infestation, and moisture degradation. Instead, the unloaded feedstock is stored in concrete domes (M-104). Two domes (each with a 36-hour capacity) are required so that one can be loaded while the other empties to the conversion process.

Conveyors (C-106, C-107, C-108) connect the storage domes to the feedstock receiving bins on the pretreatment reactor in Area 200. A dust collection system (M-106) integrated with the conveyors and domes handles airborne particles released during the unloading and conveying processes. No dry matter is assumed lost in Area 100. In contrast to the 2002 design, the feedstock is not washed, which eliminates a source of evaporative water loss in this area. There is some evidence that feedstock washing may still be desired to reduce any incoming inorganics from fertilized feedstocks like corn stover, and this practice may be revisited in the future.

3.1.3 Cost Estimation

The feedstock cost assumed in this report is $58.50/dry ton (2007$). This cost comes from the Multi-Year Program Plan (MYPP) published by DOE’s Office of the Biomass Program [27]. The total of $58.50/ton includes $23.50/ton for a grower payment (MYPP Table B-1) and $35/ton for all collection, processing, storage, and transportation costs between the field and the receiving bin on the pretreatment reactor (MYPP Table B-2). It should be stressed that these costs are 2012 DOE research targets, like the conversion performance targets used in the Aspen model.

18
Harris Group did obtain vendor quotes or other estimates for the truck unloading equipment, storage domes, conveyors, and dust collectors. Although the final equipment list assembled by Harris Group does not completely match the INL design report, the capital and operating costs for Area 100 are assumed to be included in the MYPP feedstock cost and are not included in the total capital investment (TCI) calculation; therefore they do not affect the MESP.

The truck scales were quoted by St. Louis Scale, and the truck dumpers and hoppers were quoted by Jeffrey Rader. The storage domes, each with a 4,400 ton capacity, were quoted by Domtec. The internal reclaim system was quoted by Cambelt. All other connecting conveyors were quoted by Dearborn Midwest Conveyor Co. Sly, Inc. provided a quote for all components in the dust collection system. The belt scales for biomass leaving the storage domes were quoted by Tecweigh.

19
3.2 Area 200: Pretreatment and Conditioning

3.2.1 Overview

The pretreatment process converts most of the hemicellulose carbohydrates in the feedstock to soluble sugars (xylose, mannose, arabinose, and glucose) by hydrolysis reactions. Acetyl groups in the hemicellulose are liberated as acetic acid. The breakdown of biomass in pretreatment facilitates downstream enzymatic hydrolysis by disrupting cell wall structures, driving some lignin into solution, and reducing cellulose crystallinity and chain length. The nature and extent of such changes are highly dependent on the pretreatment chemistry and reaction severity (defined by residence time, temperature, and catalyst loading). Sugar degradation products such as furfural and 5-hydroxymethyl furfural (HMF) can also be formed in pretreatment. These compounds can have adverse effects on the fermenting organisms in sufficiently high concentrations.

In the present design, hydrolysis reactions are catalyzed using dilute sulfuric acid and heat from steam. Pretreatment is carried out in two stages in the present design and the reaction severity is fairly mild compared to what has been modeled in the past. This milder pretreatment favors the production of soluble xylose oligomers. Higher-severity pretreatments tend to produce more monomeric xylose but at the risk of forming significant amounts of degradation products if reaction conditions are not well controlled.

The first stage in pretreatment is a horizontal screw-feed reactor with a short residence time (5–10 minutes). The second stage is a lower temperature/longer residence time “oligomer conversion” step that converts most of the xylose oligomers leaving the first stage to monomeric xylose without generating significant additional degradation products [31]. After the pretreatment reactors, the hydrolysate slurry is flash-cooled, vaporizing a large amount of water along with some of the acetic acid and furfural. The flash vapor is condensed and sent to the wastewater treatment area. The hydrolysate slurry is cooled by dilution water and sent to a conditioning reactor, where ammonia is used to raise its pH from 1 to 5–6. Figure 6 shows a simplified flow diagram of the pretreatment area.

Figure 6. Simplified flow diagram of the pretreatment and conditioning process
Milled corn stover
Acid
Steam
Steam
Dilution water
& NH3
Vertical presteamer
Horizontal reactor
Blowdown tank
Oligomer conversion
Ammonia conditioning
To wastewater
To enzymatic hydrolysis
BFW
Hot water

20
In previous designs, the pretreated biomass was separated into washed solid and liquid fractions, and the liquor and wash water were conditioned by an “overliming” process in which the pH was increased from 1 to ~10 with lime and then readjusted to ~5 with additional sulfuric acid. The lime and sulfuric acid precipitated as gypsum, which was removed in another solid-liquid separation step. The conditioned liquid was then re-slurried with the cellulosic solids before enzymatic hydrolysis. In overliming, a significant amount of sugar in the liquor (as much as 13%) could be lost to side reactions occurring at high pH or pressed out with the wet gypsum. The present design uses ammonia in place of lime to avoid these sugar losses. The high miscibility of ammonia also permits conditioning of the whole hydrolysate slurry and eliminates the solid-liquid separation steps. Fermentation studies have indicated that there is no benefit to over-conditioning at high pH when using ammonia, so the hydrolysate is simply adjusted to enzymatic hydrolysis pH in one step. While ammonia is considerably more expensive than lime, the economic benefits of reduced sugar loss and reduced capital cost make ammonia the more economic alternative [32]. It is also possible that the ammonia could reduce nitrogen requirements in fermentation, but this currently is not modeled.

3.2.2 Design Basis

The pretreatment reactor system includes a feedstock receiving system, followed by a vertical vessel with a long residence time for steam-heating and potential acid impregnation of the biomass, followed by the horizontal pretreatment reactor, which operates at a higher pressure and a short residence time. PFD-P120-A201 (Appendix E) shows the components in greater detail and PFD-P120-A202 shows the oligomer conversion and conditioning equipment. The horizontal reactor configuration was chosen because it permits tighter residence time distribution control than a vertical reactor. This is important in single-step, high-severity pretreatment to minimize “over-cooking” or “under-cooking” portions of the biomass, either of which would lower the overall yield.

Milled corn stover is fed to the receiving bins at the inlet of the pretreatment reactor (M-201). The receiving bins are rectangular with a bottom-drag conveyor that moves the feedstock pile inside the bin toward the doffing rolls (special scraper shafts with radial pins that spread material uniformly onto the discharge belt conveyor). The receiving bins also have a top rake-belt installed just under the bin cover to move incoming material toward the end of the bin, ensuring first-in/first-out material handling. At the discharge of each bin, the transfer conveyor (C-201) lifts material to the distribution screw conveyor (C-202), which supplies slightly (~10%) more feedstock than each pin drum feeder requires. Overfeeding allows the speed of the pin drum feeders to control the flow rate of material into each plug screw feeder. It also ensures that the plug screw feeders maintain a maximum fill. The excess feedstock is conveyed back to the storage bin by a series of screw conveyors (C-203).

Each pin drum feeder (M-202) packs feedstock material into separate plug screw feeders (M-203). The 26-in. plug screw feeder is a rugged, high-compression screw device designed to form a pressure-tight plug of material through axial compression. The compression action in each plug screw feeder may also squeeze out water and some of the water-soluble extractive components. This “pressate” could be handled as a separate, concentrated waste stream but in the present model, it is assumed that the pressate is recombined with the hydrolysate at the outlet of the reactor. Dilute sulfuric acid is injected at the discharge spool of the plug screw feeder. Feedstock drops from the plug screw discharge into a mixing and heating screw (C-204). The heating screw discharges the feedstock into the top of the presteamer (M-204). Hot water is added at this point to control the pretreatment effluent at 30 wt % total solids.

21
The vertical biomass presteamer is designed for a retention time of up to 10 minutes at a temperature of up to 165°C, though in the current model it only operates at 100°C such that no significant hydrolysis reactions occur in the presteamer. With a 2,205 ton/day throughput and 10- minute retention time, a single vertical vessel is adequate. Feedstock flows downward through the vertical reactor with uniform temperature throughout. The reactor is discharged through a dual screw outlet device (C-205) to two plug screw feeders (M-206). The plug screw feeders meter feedstock to the pretreatment reactor and control the pressure and temperature difference between it and the presteamer. Acid for the pretreatment reaction is added at the discharge of each plug screw feeder. The transport conveyors (C-206, C-207) combine feedstock from both plug screw feeders and deliver it to the pretreatment reactor (M-207).

The pretreatment reactor is a single horizontal reaction vessel. The reactor is designed for fairly severe conditions of up to 190°C (374°F) and about 1.1 wt % sulfuric acid. In the current design, the reaction conditions are milder at 158°C (316°F) and 18 mg acid/dry g of biomass. Acid is metered to the reaction chamber at a rate proportional to the mass flow rate of feedstock. High pressure steam is injected into this vessel to maintain temperature. The reactor pressure is held just at the bubble point for the mixture. Heat losses from the reactor are not accounted for in the energy balance calculations. The residence time in the pretreatment reactor is nominally 5 minutes. The reaction conditions are summarized in Table 5.

Table 5. Pretreatment Reactor Conditions
Sulfuric acid loading 18 mg/g dry biomassa
Residence time 5 minutes
Temperature 158°C
Pressure 5.5 atm (81 psia)
Total solids loading 30 wt %
a Additional acid is added downstream of the pretreatment reactor.

The pretreatment reactor is discharged to a flash tank (T-203). The pressure of the flash is controlled to keep the temperature at 130°C (266°F). The slurry from T-203 goes into the secondary oligomer conversion reaction vessel (T-208), where it is held at 130°C for 20–30 minutes. An additional 4.1 mg/g of sulfuric acid is added in the oligomer conversion step, bringing the total acid loading to 22.1 mg/g dry biomass. (Note that in the Aspen model, all of the acid is added to the pretreatment reactor block.)

The oligomer conversion reactor is discharged into another flash tank (T-204) that operates at atmospheric pressure. After this flash, the hydrolysate whole slurry containing 30 wt % total solids and 16.6 wt % insoluble solids is sent to the conditioning tank (T-209). Here, the slurry is diluted with water to slightly greater than 20 wt % total solids to ensure miscibility through enzymatic hydrolysis. Ammonia gas is mixed into the dilution water to raise the hydrolysate pH to 5. The residence time in T-209 is 30 minutes and the dilution cools the slurry to 75°C (167°F).

The flash vapor from T-203 is used to preheat the boiler feed water in H-812 or combined with the 100°C (212°F) flash vapor from T-204, which is condensed in H-201 and H-244. This condensate contains volatile, potentially inhibitory organics created in pretreatment and therefore is routed to wastewater treatment (Area 600).

22
Table 6 summarizes the reactions and percent conversions that take place in pretreatment. Glucan contained in the hemicellulose side-chains is converted to glucose along with a small portion of the cellulose. Minor hemicellulose carbohydrates (arabinan, mannan, galactan) are assumed to have the same reactions and conversions as xylan. The xylan-to-xylose conversion is an assumed total hydrolysis that also includes an enzymatic component that will be discussed later. The sucrose reaction to HMF and glucose reflects 100% hydrolysis of sucrose to fructose and glucose, followed by complete degradation of the fructose to HMF, as mentioned in Section 2.2.
Table 6. Pretreatment Hydrolysis Reactions and Assumed Conversions
Reaction Reactant % Converted to Product
(Glucan)n + n H2O→ n Glucose Glucan 9.9%
(Glucan)n + n H2O → n Glucose Oligomera Glucan 0.3%
(Glucan)n → n HMF + 2n H2O Glucan 0.3%
Sucrose → HMF + Glucose + 2 H2O Sucrose 100%
(Xylan)n + n H2O→ n Xylose Xylan 90.0%
(Xylan)n + m H2O → m Xylose Oligomera Xylan 2.4%
(Xylan)n → n Furfural + 2n H2O Xylan 5.0%
Acetate → Acetic Acid Acetate 100%
(Lignin)n → n Soluble Lignin Lignin 5.0%
a Sugar oligomers are considered soluble but not fermentable.


3.2.3 Cost Estimation

For the pretreatment reactor system, Harris Group obtained a detailed quote from Andritz, Inc., totaling approximately $20MM for the whole system: feedstock receiving bin, additional size reduction steps (if necessary), pre-steaming, pressurized heating, reaction, and flash cooling. A reactor schematic provided by Andritz is shown in Figure 7. This reactor configuration is similar in principle to the pretreatment reactor assumed in the 2002 design. 

The reactor system is constructed of carbon steel with all parts in contact with acid (pretreatment reactor, pressurized transporter, and plug screw feeder) clad in Incoloy 825. This met Andritz’s approval but was primarily chosen to be consistent with the 2002 design and a previous NREL corrosion study on reactor metallurgy [33]. This reactor system is actually overdesigned for the pretreatment process conditions considered here and is capable of operating at a significantly higher severity. In the present design, the pretreatment system contributes about $0.14/gal to the MESP; we chose not to adjust the cost of the reactor to account for the lower residence time, temperature, pressure, or acid loading. This will permit continued use of the same reactor cost in our analyses as researchers change the pretreatment severity in their optimization studies. As long as acid is used in any concentration, we believe it is unlikely that the reactor cost would change significantly because Incoloy (or similarly expensive) cladding would still be required. The reactor cost will be revisited in the future if pretreatment conditions change more significantly.

23
Figure 7. Horizontal pretreatment reactor design scheme (Andritz, Inc.)

Costs for other equipment, such as pumps, agitators, tanks, conveyors, and heat exchangers, were estimated using Harris Group’s internal database. The holding tank for sulfuric acid (T-201) is plastic, and the rest of the equipment is stainless steel—most of it 316SS to provide additional acid resistance at temperatures below 100°C (212°F).

3.2.4 Achieving the Design Case
Table 7 shows demonstrated pilot-scale performance results achieved from 2008–2010 [21, 34–35] as well as the 2012 conversion targets (i.e., those used in the Aspen model) for the pretreatment area. In pretreatment, the 2012 target is 90% conversion of xylan to monomeric xylose with 5% loss to degradation products. An additional 2012 target is to move to a whole slurry conditioning process and thereby eliminate the need for a solid-liquid separation step in the pretreatment area.
Feedstock
Feedstock
Steam
Flush water
Flush water
Steam
Acid
Vent
Hydrolysate to oligomer conversion
Pressate
Pressate
reinjection
Screw feeder
Screw feeder
Vertical presteamer
Horizontal reactor

24
Table 7. Research Status and 2012 Targets in the Pretreatment Area
2008 State of Technology
2009 State of Technology
2010 State of Technology
2012 Targets
Pretreatment
Solids loading (wt %) 30% 30% 30% 30%
Xylan conversion to xylose (%) 75% 84% 85% 90%
Xylan conversion to furfural (%) 11% 6.4% 8% 5%
Conditioning
Ammonia loading (g/L of hydrolysate) 13 10 4.8 4.8
Hydrolysate solid-liquid separation yes yes yes no
Xylose sugar loss (% entering conditioning) 2% 2% 2% 1%
Glucose sugar loss (% entering conditioning) 1% 1% 1% 0%

In NREL’s pretreatment research, significant improvements in the conversion of xylan to xylose by dilute-acid pretreatment were demonstrated at the bench scale in 2007, where conversions of 75% or higher were routinely achieved in bench-scale batch reactors [36]. Efforts to duplicate these results in continuous pilot-scale operation in 2008 proved more challenging. Continuous pretreatment is more difficult than batch pretreatment because process conditions (residence time in particular) cannot be as tightly controlled. Experiments in NREL’s 200 kg/day continuous orizontal pretreatment reactor indicated a xylan-to-xylose conversion limit of ~60% in that reactor configuration, though total conversion to monomeric and oligomeric xylose was around 75%. The mild secondary oligomer conversion step was therefore added to convert the oligomers to monomeric xylose without generating additional degradation products, meeting the 2008 xylose target of 75%.

In 2009, the internals of the horizontal reactor were modified to tighten its residence time distribution [37]. Optimization of the operating conditions between the two stages met 2009 targets with an overall xylan-to-xylose conversion of 79.6% with 6.4% loss to furfural. Remaining oligomers were 9.0%, leaving 5% of the xylan unreacted [38]. Further process optimization in 2010 showed little improvement over these conversions but additional xylose yield was obtained in enzymatic hydrolysis using an advanced cellulase preparation that has xylanase and “xylooligomerase” activities. In washed-solids enzymatic hydrolysis, the advanced enzyme preparation converted an additional 82% of the unreacted xylan to xylose. Overall, an 85.3% yield of monomeric xylose was achieved from all thermochemical and enzymatic processes in 2010 experiments [39].

The targeted enzymatic conversion of xylan and xylose oligomers described above is quite promising [40]. It could eliminate the secondary oligomer conversion step used in our design and, in general, permit lower-severity pretreatments that yield more xylose oligomers and fewer degradation products. Lower-severity pretreatments have relaxed residence time control requirements and may be able to utilize lower-cost vertical reactor configurations. (Vertical pretreatment reactors are typically less expensive than horizontal reactors with the same throughput because they have less complex internals, though reduced severity will probably not eliminate the need for exotic reactor cladding on acid-wetted surfaces.) Additionally, lower pretreatment severity would result in lower energy requirements and reduced chemical costs, including reduced cleanup in wastewater treatment.

25
Including these hemicellulase “accessory” enzymes in our technoeconomic analysis is complicated because little to no cost information exists for these highly specialized, pre commercial enzymes. However, preliminary analysis has shown that if the xylan and xylose oligomer hydrolysis is carried out simultaneously with the cellulose enzymatic hydrolysis, accessory enzymes are probably the more economic option, assuming they can be obtained at a cost per kg of protein similar to that currently assumed for cellulase [41].

Replacing overliming with ammonia conditioning has eliminated significant sugar losses and gypsum disposal cost. Because ammonia can be mixed with the dilution water and applied as an aqueous solution, the whole hydrolysate slurry may be treated at once without a solid-liquid separation step. However, from Table 7, one may note that elimination of hydrolysate solid liquid separation is not assumed until 2012. This is due not to problems with the conditioning procedure but to conversion limitations in whole-slurry enzymatic hydrolysis caused by end product inhibition, particularly with respect to the xylanase activities discussed above. Nevertheless, in the present design, which is intended to reflect 2012 technology, a whole-slurry process through conditioning and enzymatic hydrolysis is assumed.

Further research topics in the pretreatment area include biomass deacetylation through acid pre impregnation, use of co-catalysts (e.g., iron salts), and disc-refining of the pretreated slurry. These are designed to reduce sulfuric acid usage in pretreatment and achieve high xylose yields under less severe pretreatment conditions while maintaining high enzymatic digestibility of cellulose in the pretreated solids, with economic benefits as discussed above. In addition, deacetylation and disc-refining may significantly enhance downstream enzymatic hydrolysis and  potentially decrease enzyme loading requirements. Acid pre-impregnation is not explicitly modeled in our design, but it is envisioned that it could take place in the vertical presteamer, though the cost of the reactor system would have to be increased to include Incoloy cladding on the presteamer as well as all screw feeders and conveyors between the presteamer and the pretreatment reactor. This design effort is ongoing.

26
3.3 Area 300: Enzymatic Hydrolysis and Fermentation

3.3.1 Overview

In this process area, cellulose is converted to glucose using cellulase enzymes. This process is known as enzymatic saccharification or enzymatic hydrolysis. A cellulase enzyme preparation is a mixture of enzymes (catalytic proteins) that work together to break down cellulose fibers into cellobiose and soluble gluco-oligomers and ultimately into glucose monomers. The resulting glucose and other sugars hydrolyzed from hemicellulose during pretreatment are fermented to ethanol. Most fermentation research at NREL has used the recombinant co-fermenting bacterium Zymomonas mobilis because this microorganism and much of its genome are in the public domain [42]. “Co-fermenting” means that the organism can simultaneously ferment glucose and xylose to ethanol. Other co-fermenting ethanologens are also being considered at NREL and elsewhere, e.g., metabolically engineered strains of Saccharomyces cerevisiae [43].

The process assumed in this design is known as separate (or sequential) hydrolysis and fermentation (SHF). Enzymatic hydrolysis is initiated while the slurry is still at an elevated temperature after pretreatment and conditioning. At this temperature, the enzyme activity is higher so conversion is faster and a smaller amount of enzyme is required. Once the conversion of cellulose to glucose is complete, the slurry is cooled to fermentation temperature and inoculated with the fermenting microorganism (the “ethanologen”). This deviates from the 2002 process, which was based on a simultaneous saccharification and co-fermentation (SSCF) process in which the temperature of the slurry was reduced and fermentation was initiated before enzymatic hydrolysis was complete. In SSCF, the enzyme continues to hydrolyze cellulose even after fermentation is initiated. Fermentation creates a sugar sink (because sugar is being consumed by the ethanologen) that helps drive the enzymatic hydrolysis reactions toward glucose.

The 2002 process was also nominally continuous with a total residence time of 3 days. Based on more recent experience with Z. mobilis, a 5-day SHF process with batch fermentation was selected as a more realistic case for the present design. Enzymatic hydrolysis begins in a continuous, high-solids reactor. As the cellulosic solids are saccharified by the enzyme, the viscosity of the mixture drops dramatically, such that it can be pumped to one of several parallel bioreactors. Hydrolysis continues in this vessel until complete, then the slurry is cooled and the ethanologen inoculum is added. The ethanol-containing fermentation broth is emptied to the beer well (storage tank) before being pumped to distillation. Figure 8 shows a simplified flow diagram of the enzymatic hydrolysis and fermentation process. 

27
Beer
To recovery
High-solids hydrolysis (continuous flow)
Batch Hydrolysis/Fermentation
Seed train (Zymomonas mobilis)
Beer well
CW
Enzyme
Hydrolysate
Figure 8. Simplified flow diagram of the enzymatic hydrolysis and fermentation process

3.3.2 Design Basis

The full process flow is shown in PFD-P120-A301 and -A302 (Appendix E). Enzymatic hydrolysis is initiated in a continuous, high-solids reactor (T-310). Neutralized, diluted hydrolysate is cooled with cooling water in H-301 and fed to T-310 at slightly higher than 20 wt % total solids. A 100-hp inline mixer upstream of the continuous hydrolysis reactor (A-308) mixes the enzyme into the slurry. After the cellulase enzyme stream is mixed in, the total solids loading is 20 wt % (10.6 wt % insoluble) and the temperature is 48°C (118°F). The  residence time in this first stage is 24 hours, after which the slurry is batched to one of twelve 950,000-gal vessels (F-300), where enzymatic hydrolysis continues for another 60 hours.

Moving pretreated material at 20% (or higher) total solids loading is challenging because this material is not pumpable until the cellulose has been partially enzymatically hydrolyzed. In the present design, the continuous high-solids hydrolysis reactor is envisioned as an empty tower, with the slurry entering at the top and flowing down with gravity. Horizontal mixers with rotating paddles are another design option for performing the initial enzymatic hydrolysis reaction, and NREL will be testing such a reactor in its new Integrated Biorefinery Research Facility (IBRF) in 2011 [44]. These are expected to be more expensive than the plug-flow tower specified here, but not dramatically so given the relatively short residence time expected in the high-solids vessels and when considered in the total equipment scope of the plant. We believe that the tower design is a suitable placeholder.

The amount of enzyme used (the enzyme loading) is determined by the amount of cellulose present in the hydrolysate and the specific activity of the enzyme. In the present design, the total cellulase loading is 20 mg enzyme protein/g cellulose to achieve a 90% conversion to glucose. “Protein” here refers to the total concentration of protein in the enzyme broth as determined by assay; not all of this protein has cellulase activity. Although sugar yield generally increases with higher enzyme loading, the additional enzyme obviously comes at a cost. Enzyme loading therefore has a significant and complex impact on process economics. Determining the most economical enzyme loading requires optimization of several process parameters including temperature, residence time, and total solids loading [45]. The design conditions developed based on the recommendations of enzyme manufacturers and NREL researchers are summarized
in Table 8.

28
Table 8. Enzymatic Hydrolysis Conditions
Temperature 48°C (118°F)
Initial solids loading 20 wt % total solids (10.6% insoluble/9.4% soluble)
Residence time 3.5 days total (84 h)
Number and size of continuous vessels 8 @ 950 m3 (250,000 gal) each
Number and size of batch vessels 12 @ 3,600 m3 (950,000 gal) each
Cellulase loading 20 mg protein/g cellulose

The batch reactors are agitated and temperature-controlled using a pump-around loop that consists of a centrifugal pump (P-300) and a heat exchanger (H-300). During enzymatic hydrolysis, the temperature is maintained with cooling water. Temperature control during enzymatic hydrolysis is important. Enzyme studies at NREL have indicated an optimum temperature of 48°C for a number of commercial and development enzymes. A -5°C deviation could result in a dramatically reduced rate of reaction; a +5°C deviation could result in the onset of protein denaturation. Either situation would reduce the cellulose conversion yield for the same residence time.

Table 9 lists the reactions and conversions taking place during enzymatic hydrolysis. The saccharified slurry contains 11.7 wt % total soluble sugar (including oligomers), with 6.7% monomeric glucose and 3.7% monomeric xylose. As mentioned in Section 3.2, some of the more advanced enzyme preparations have shown a significant ability to also convert xylan to xylose. This additional conversion is captured in pretreatment so it is not included in Table 9. Note that glucose oligomers are modeled in Aspen as “glucose molecules in oligomeric form”; the actual size distribution of the oligomers is not captured.

Table 9. Enzymatic Hydrolysis Reactions and Assumed Conversions
Reaction Reactant % Converted to
Product
(Glucan)n → n Glucose Oligomer Glucan 4.0%
(Glucan)n + ½n H2O → ½n Cellobiose Glucan 1.2%
(Glucan)n + n H2O → n Glucose Glucan 90.0%
Cellobiose + H2O → 2 Glucose Cellobiose 100%

After 60 hours of additional enzymatic hydrolysis in F-300, the saccharified slurry is cooled by the pump-around loop and larger heat exchanger H-310 (specific to this task and shared between all the fermentors) to 32°C for fermentation. Recombinant Zymomonas mobilis bacterium is used as the ethanologen. This strain of Z. mobilis can simultaneously ferment glucose and xylose to ethanol. The present design assumes that the minor hemicellulosic sugar arabinose is also fermented to ethanol with the same yield as xylose, although this is a research target for 2012 and has not yet been demonstrated at NREL.

The inoculum protocol for Z. mobilis is a direct transfer of cells without a cell concentration step. In order to provide a required 10% inoculum volume back to the production fermentors, 10% of the saccharified slurry is split off to seed production (see PFD-P120-A301, Appendix E). Each seed train consists of five reactors operating in batch mode with a 24-hour batch time and an additional 12-hour turnaround time. The seed fermentors are cooled with chilled water from Area 900 to maintain the temperature at 32°C (90°F). The first vessel (40 gallons) is inoculated with a seed culture from the lab. Its broth is used to inoculate a larger reactor, and so on. After five iterations, the cell mass from the last vessel (200,000 gallons) is sufficient to inoculate the production vessel. Following the 2002 design, it was decided that two trains would be optimal [2]. Using these conditions, the fifth reactor in Train A will complete fermentation at 180 hours. Train B will complete fermentation 12 hours later. Another 24 hours after that, Train A is again complete and the cycle continues. A discussion of seed train cycling can be found in the 2002 report. Table 10 summarizes the seed train design specifications. Additionally, 0.1% (w/v) sorbitol is used in the final seed fermentor to improve cell viability at high sugar concentrations [46, 47]. Sorbitol is not a component in the Aspen model, but it is reflected in the economics by purchasing an amount of sorbitol equivalent to 0.1% (w/v) of the sugar flow to the seed train, at a cost of approximately 0.7 cents/gal ethanol.

29

Table 10. Seed Train Specifications
Inoculum level 10 vol % of production vessel size
Batch time 24 h
Fermentor turnaround time 12 h
Number of trains 2
Number of fermentor stages 5
Maximum fermentor volume (F-305) 200,000 gal (757 m3)
Corn steep liquor (CSL) loading 0.50 wt %
Diammonium phosphate (DAP) loading 0.67 g/L fermentation broth (whole slurry)

Table 11 gives the reactions and conversions used in the seed fermentors to describe the
microorganism growth and sugar metabolism. The fraction of sugar converted to cell mass is rather small. This is typical for Z. mobilis and is economically beneficial as well—most of the sugar entering the seed train is converted to ethanol, which is ultimately added to the production fermentors and recovered. So even though 10% of the saccharified slurry is diverted to produce the seed culture, its ethanol-producing potential is not lost. Other species (E. coli or yeast) could be expected to have cell mass yields about 2 times higher than that of Z. mobilis and thus produce modestly lower amounts of ethanol during seed culture propagation.

Table 11. Seed Train Reactions and Assumed Conversions
Reaction Reactant % Converted to
Product
Glucose → 2 Ethanol + 2 CO2 Glucose 90.0%
Glucose + 0.047 CSLa + 0.018 DAP → 6 Z. mobilis + 2.4 H2O Glucose 4.0%
Glucose + 2 H2O→ 2 Glycerol + O2 Glucose 0.4%
Glucose + 2 CO2→ 2 Succinic Acid + O2 Glucose 0.6%
3 Xylose → 5 Ethanol + 5 CO2 Xylose 80.0%
Xylose + 0.039 CSL + 0.015 DAP → 5 Z. mobilis + 2 H2O Xylose 4.0%
3 Xylose + 5 H2O → 5 Glycerol + 2.5 O2 Xylose 0.3%
Xylose + H2O→ Xylitol + 9.5 O2 Xylose 4.6%
3 Xylose + 5 CO2 → 5 Succinic Acid + 2.5 O2 Xylose 0.9%
a Corn steep liquor (CSL) and diammonium phosphate (DAP) are both nitrogen sources required for Z. mobilis growth. The stoichiometry shown above is only used to balance the compositions assumed for nonstandard components like cell mass.

Two high-capacity transfer pumps (P-302) are used to transfer the seed to a holding tank (T-301) in a timely fashion (approximately 2.5 h). The seed hold tank (T-301) is sized to hold 20% more than the fifth seed reactor (F-305). Another pump (P-301) feeds the seed to the production fermentation train.

30
Besides being fermented to ethanol, sugar may be lost to side products by contaminating microorganisms. A total of 3% of the sugars available for fermentation is assumed lost to contamination, as discussed in the 2002 design report. This is the level of contamination loss tolerated by the corn ethanol industry, so it can be thought of as an expected value consistent with good batch fermentor operation. The contamination loss is modeled by converting a fraction of the sugars to lactic acid upstream of the fermentor. This allows us to simply assign a percent loss to contamination in the model so the conversions in the fermentor do not have to be adjusted. Table 12 shows the contamination reactions only.

Table 12. Co-Fermentation Contamination Loss Reactions
Reaction Reactant % Converted to
Product
Glucose → 2 Lactic Acid Glucose 3.0%
3 Xylose → 5 Lactic Acid Xylose 3.0%
3 Arabinose → 5 Lactic Acid Arabinose 3.0%
Galactose → 2 Lactic Acid Galactose 3.0%
Mannose → 2 Lactic Acid Mannose 3.0%

Fermentation is conducted in a batch system of 950,000-gal vessels (F-300). The fermentation residence time is modeled as 36 hours. Inoculum from the seed train is fed at 10 vol % of the hydrolysate flow along with the nutrients corn steep liquor (CSL, 0.25 wt %) and diammonium phosphate (DAP, 0.33 g/L of whole slurry). The fermentors are cooled using the pump-around loop with H-300 switched from cooling water to chilled water from the coolant loop (Area 900). Agitation requirements in the main production reactors were reduced from those in the 2002 design. The main reactors (F-300) are agitated at 0.03 hp/1,000 gal (6 W/m3). The assumption is that most of the liquefaction and viscosity reduction of the slurry takes place in the continuous high-solids hydrolysis reactor, and vigorous agitation is not required in anaerobic Z. mobilis fermentation.

Table 13 summarizes the conditions in the fermentation vessels and Table 14 lists the reactions and conversions assumed in fermentation. Based on NREL’s knowledge of state-of-the-art co fermenting microorganisms, arabinose is assumed to have the same conversion to ethanol as xylose does. Conversion of galactose and mannose to ethanol is not assumed, in contrast to the 2002 design. Arabinose follows the xylose stoichiometry, with 85% conversion to ethanol. Inhibition effects from furans and acetate are not modeled explicitly in Aspen, having no kinetics available to do so, but they are implicit in the static conversions used in the model because these conversions are based on fermentation experiments carried out in the presence of these inhibitors. NREL does have an active research program in fermentation inhibitor characterization and mitigation [48], but the details of this program are beyond the scope of this process design report.

31
Table 13. Co-Fermentation Conditions
Organism Recombinant Zymomonas mobilis
Temperature 32°C (96°F)
Initial fermentation solids level 19.8% total solids (14.7% soluble, 5.1% insoluble w/w)
Residence time 1.5 days (36 h)
Inoculum level 10 vol %
Corn steep liquor (CSL) level 0.25 wt %
Diammonium phosphate (DAP) level 0.33 g/L fermentation broth (whole slurry)

Table 14. Co-Fermentation Reactions and Assumed Conversions
Reaction Reactant % Converted to Product
Glucose → 2 Ethanol + 2 CO2 Glucose 95.0%
Glucose + 0.047 CSLa + 0.018 DAP → 6 Z. mobilis + 2.4 H2O Glucose 2.0%
Glucose + 2 H2O → 2 Glycerol + O2 Glucose 0.4%
Glucose + 2 CO2 → 2 Succinic Acid + O2 Glucose 0.6%
3 Xylose → 5 Ethanol + 5 CO2 Xylose 85.0%
Xylose + 0.039 CSL + 0.015 DAP → 5 Z. mobilis + 2 H2O Xylose 1.9%
3 Xylose + 5 H2O → 5 Glycerol + 2.5 O2 Xylose 0.3%
Xylose + H2O → Xylitol + 0.5 O2 Xylose 4.6%
3 Xylose + 5 CO2 → 5 Succinic Acid + 2.5 O2 Xylose 0.9%
a Corn steep liquor (CSL) and diammonium phosphate (DAP) are both nitrogen sources required for Z. mobilis growth. The stoichiometry shown above is only used to balance the compositions assumed for Z. mobilis cell mass. Nutrient requirements have not been optimized and a minimal, low-cost nutrient formulation has yet to be defined.

The fermentation broth or “beer” has an ethanol concentration of 5.4 wt % and is collected in the beer well (T-306). A small amount of additional ethanol is entrained in the CO2 vent stream and will be recovered to the beer well via the vent scrubber. The beer well is designed for a residence time of 4 hours to provide surge capacity between fermentation and distillation.

3.3.3 Cost Estimation

In general, the material of construction for all equipment in this section is 304SS, which is the most cost-effective material for fermentation service. Carbon steel has been proposed as an alternative and does have a precedent in the corn ethanol industry with some technology providers. However, stainless steel is more common, and Harris Group felt that carbon steel fermentors would have to be designed thicker for corrosion allowance, which would mostly negate the capital savings from using the cheaper material. Carbon steel also tends to pit and can harbor biofilms, creating a contamination source.

The continuous enzymatic hydrolysis reactor (T-310) is envisioned in this design as an empty tower that is loaded from the top. Harris Group obtained a quote from Caldwell for eight such vessels to be run in parallel. These were flat-bottomed plug-flow reactors with a 10:1 height:diameter ratio. The larger vessels were quoted by Mueller: the million-gallon batch fermentors (F-300), the seed hold tank (T-301), and the beer well (T-306). Mueller also quoted the fourth and fifth seed fermentors (F-304, F-305), including internal cooling coils. The smaller seed fermentors (F-301, F-302, F-303) were quoted by A&B Process Systems as skidded units with cooling jackets and agitators. Harris Group developed costs for all of the pumps in this area using their internal equipment database. Costs for the larger agitators, i.e., those on the fermentors (A-300), the seed fermentors (A-304, A-305), and other large tanks (A-301, A-306), were based on vendor (Lotus) quotes obtained by Harris Group. Large agitators tend to be topmounted because they are more energy-efficient than side-entry agitators.

32
Harris Group obtained quotes from Alfa Laval for the plate and frame heat exchangers in this area (H-300, H-310). The incoming hydrolysate cooler is a shell-and-tube heat exchanger from Fox Engineering.

3.3.4 Achieving the Design Case
For the enzymatic hydrolysis and fermentation area, Table 15 shows the demonstrated results used in the State of Technology (SOT) cases from 2008 to 2010 and the ultimate 2012 targets (i.e., those used in the Aspen model). 

Table 15. Research Status and 2012 Targets in Enzymatic Hydrolysis and Fermentation
2008 State of Technology
2009 State of Technology
2010 State of Technology
2012 Targets
Total solids loading (wt %) 20% 20% 17.5% 20%
Enzymatic hydrolysis substrate Washed
solids
Washed
solids
Washed
solids
Whole
slurry
Combined hydrolysis and fermentation
time (days) 7 5 5 5
Corn steep liquor loading (wt %) 1% 1% 1% 0.25%
Overall cellulose to ethanol conversion
(through hydrolysis and fermentation,%)a 85.5% 84% 87% 85.5%
Xylose to ethanol fermentation
conversion (%) 80% 82% 79% 85%
Arabinose to ethanol fermentation
conversion (%) 0% 51% 68% 85%
a Assumes 95% glucose-to-ethanol conversion.

Enzymatic hydrolysis and fermentation experiments are typically “integrated” with pretreatment, meaning that a single large batch of pretreated material is used to perform many hydrolysis and fermentation experiments. Integrated performance results for the process configuration and operating conditions assumed in the 2002 design (i.e., 20% total solids loading with overliming) [2] were first produced in 2005. In 2008, integrated experimental results advanced significantly toward the 2012 targets following the replacement of overliming with ammonium hydroxide conditioning, which demonstrated a slightly improved cellulose-to-ethanol yield and significantly better xylose-to-ethanol yield due to decreased sugar losses and improved hydrolysate fermentability [32].

Enzymatic Hydrolysis
In all of the SOT experiments shown in Table 15, the pretreated hydrolysate underwent solidliquid separation and the liquor was conditioned with ammonium hydroxide as described previously. In these so-called washed-solids experiments, enzymatic hydrolysis was performed only on the pressed and washed pretreated solids (i.e., in the absence of pretreatment liquor). The conditioned liquor was added back to the hydrolysate slurry just before fermentation. The 2012 targets for enzymatic hydrolysis, however, assume a whole-slurry process, in which the whole pretreated slurry is neutralized, hydrolyzed, and fermented without a complicated and costly solid-liquid separation step. Based on bench-scale testing at NREL, Larox (now Outotec) helped to estimate the purchased capital cost of a hydrolysate pressure filter system at the present design flow as being on the order of $30MM minimally. The solid-liquid separator cost used in the 2002 design was only about $5MM. We suspect that the older cost estimate was extremely optimistic. In general, we have found a considerable discrepancy in the cost of solid-liquid separation technology being quoted now compared to what was quoted in the 1990s and 2000s, though we have not investigated why this might be so.

33
In 2009, NREL began studying whole-slurry enzymatic hydrolysis in earnest because advanced enzyme preparations became available that could perform satisfactorily on this material. One advanced preparation was tested at the pilot scale and performed very well, achieving 91% cellulose-to-glucose conversion in initial process-relevant whole-slurry enzymatic hydrolysis experiments on a 2008 batch of pretreated corn stover (PCS) in which a 75% xylan-to-xylose conversion was achieved in pretreatment (see Table 7). Previously, cellulose-to-glucose conversions of 90% were not uncommon in washed-solids hydrolysis experiments, but this enzyme was the first tested at NREL to demonstrate such a high conversion in a whole-slurry experiment.

As described in Section 3.2, the direction in NREL pretreatment research has been toward lower severity processes that rely on secondary thermochemical or enzymatic hydrolysis to convert xylose oligomers to monomers. The reduced severity also affects cellulose digestibility. In newer batches of PCS that have higher (≥80%) xylose yield, the glucose yield from cellulose is lower for the same total solids loading. Loss of conversion may be counteracted to a degree by reducing the solids loading or by employing pretreatment-related process steps such as deacetylation and/or disc-refining, as discussed in Section 3.2.4. Whole-slurry hydrolysis results using the advanced enzyme preparation are summarized in Table 16.

Table 16. Summary of Integrated Whole-Slurry Enzymatic Hydrolysis Performance Using an Advanced Enzyme Preparation
SOT Year
PCS Batch Total Solids Loading (wt %)
Glucose Yield from Cellulose
2009 2008: 75% xylose 20% 91%
2009 2009: 80% xylose 20% 83%
2010 2010: 80% xylose 20% 84%
2010 2010: 80% xylose 17.5% 86%
2010 2010: 80% xylose 15% 90%

Cellulose-to-glucose conversion in these experiments is approaching the 2012 targets (90% conversion at 20 wt % total solids), but it is not there yet. Achieving these targets will require use of one of the rapidly-improving enzyme preparations being developed by NREL’s industrial collaborators or through DOE’s ongoing enzyme solicitation focused on the development of advanced enzyme systems [49]. In addition to cellulase activity, these advanced enzyme preparations will likely have hemicellulase activity, enabling less severe pretreatment. Accessory enzymes (e.g., ferulic acid esterase) may also be present in advanced cocktails to more efficiently hydrolyze the bonds within and linkages between cellulose, hemicellulose, and lignin. NREL will continue to monitor the performance of these evolving enzyme preparations as well as the cost of solid-liquid separation technologies in order to choose the most cost-effective process option for demonstration in 2012.

34
Fermentation
NREL continues to perform integrated fermentation experiments using the recombinant, co-fermenting Z. mobilis strain 8b. As of 2010, the ethanol tolerance limit of this microorganism has become the major barrier in NREL fermentation research. In co-fermentation, this strain readily consumes all of the available glucose, and we assume 95% is converted to ethanol. This microorganism will further consume the xylose in the system, producing ethanol until it reaches ts ethanol tolerance limit of approximately 60 g ethanol/L. (In practice, the presence of typical fermentation inhibitors from biomass hydrolysate drives the limit to <60 g/L.)

As discussed above, sugar yields from pretreatment and enzymatic hydrolysis have been steadily increasing. This has led to lower percent xylose utilizations in fermentation experiments, especially those performed at higher total solids loadings where the xylose is more concentrated. Characteristic ethanol yields from xylose in the 2009 and 2010 SOT cases are shown in Table 17. Even though the amount of available sugar changes in each case, the final ethanol concentration is more or less constant (within the accuracy of the measurement) and is indicative of the microorganism’s practical ethanol tolerance limit. At 20% total solids in 2009, the microorganism was able to convert 82% of available xylose before reaching its limit. In 2010, the same limit was reached after converting only 63% of available xylose. In other words, the results summarized in Table 17 suggest that Z. mobilis strain 8b was operating very close to its ethanol tolerance limit in 2009 and was most likely being inhibited by ethanol in 2010 when the sugar concentrations increased.

Table 17. Ethanol Yields from Xylose
2009 SOT 2010 SOT
% Total Solids in Fermentation
Xylose Conversion
Final Ethanol Conc. (g/L)
Xylose Conversion
Final Ethanol Conc. (g/L)
15% - - 78% 49
17.5% - - 79% 53
20% 82% 52 63% 53
25% - - 20% 50

Ethanologen strain research is currently being performed outside of NREL through ongoing DOE solicitation projects [50]. The companies participating in these projects are tasked with improving the ethanol tolerance of co-fermenting microorganisms like Z. mobilis to alleviate the problem of reduced ethanol yield at high sugar concentrations. Despite the highly sensitive nature of strains (ease of propagation, value of intellectual property, etc.), NREL expects to receive some of these strains for testing in 2011 and we hope to be able to demonstrate better ethanol tolerance from one or more of these strains under integrated processing conditions.

The fermentation strain solicitation awardees were also tasked with demonstrating improved conversion of the minor hemicellulosic sugars (arabinose, galactose, and mannose) to ethanol. Arabinose is the third most abundant sugar available in corn stover following glucose and xylose, making up about 5% of the total available sugar. Achieving an 85% arabinose-to-ethanol yield provides an additional 3 gallons of ethanol per ton of dry corn stover and decreases the MESP by about $0.08/gal compared to the MESP with zero conversion of arabinose. Galactose accounts for another 2.5% of the available sugar, and mannose content in corn stover is typically negligible. As of 2008, it was clear that the solicitation awardees were not likely to make significant progress on galactose or mannose conversion but that conversion of arabinose to ethanol was possible through incorporation of known arabinose metabolic pathways. In 2010, one of the awardees reported to DOE that they had demonstrated arabinose conversions of 68% on pure arabinose and 90% when glucose was dosed along with arabinose. The specifics of these experiments are protected information and cannot be shared here. NREL has also begun a program to genetically engineer the arabinose fermentation pathway into the Z. mobilis 8b strain to reduce the risk that the proprietary ethanologens being developed through the DOE strain solicitation are unable to meet the 2012 cost targets [51].

35
Low-Cost Media

As seen in Table 15, corn steep liquor (CSL) is assumed as a nutrient source for ethanol fermentation. While NREL does not actually use CSL in routine laboratory or pilot plant experiments, its use is assumed in the technoeconomic model as a placeholder for a low-cost source of nitrogen and trace minerals, and reducing the quantity of this material used in fermentation is a 2012 target. CSL, a by-product of the corn wet milling process, is high in protein, vitamins, and minerals and is usually mixed with the corn fiber by-product and sold as luten feed [52]. On its own, CSL is used as a nutrient source in many fermentation industries including wet-mill corn ethanol, pharmaceuticals, and industrial enzyme production. Because CSL is a wet mill by-product, and the corn starch business is relatively static, there is in effect a fixed amount of CSL available in the United States. We have performed some projections elsewhere and have determined that it is unlikely that CSL could scale to support cellulosic ethanol production at commercial volumes of billions of gallons per year [51]. Finding another low-cost and scalable nutrient source is a subject of future NREL research and technoeconomic analysis.

36
3.4 Area 400: Cellulase Enzyme Production

3.4.1 Overview

This process area produces cellulase enzyme that is used in Area 300 to hydrolyze cellulose into glucose. Cellulase refers to a mixture of enzymes (catalytic proteins) that includes: (1) endoglucanases, which attack randomly within the cellulose fiber, reducing polymer chain length rapidly; (2) exoglucanases, which attack the ends of highly crystalline cellulose fibers; and (3) β- glucosidase, which hydrolyzes the small cellulose fragments (cellobiose, a glucose dimer) to glucose. Cellulase is produced industrially using (among other microorganisms) Trichoderma reesei, a filamentous fungus that secretes high levels of cellulase enzymes when grown aerobically in the presence of cellulose or other cellulase inducers.

The 1999 design report [1] introduced Area 400 to produce cellulase on-site with ethanol, using a slipstream of the conditioned hydrolysate slurry from pretreatment. The 2002 design report [2] omitted Area 400 in favor of a purchased-enzyme model in which the enzyme was assigned a certain fixed cost contribution per gallon of ethanol. Area 400 was reinstated for this design report with new reactor design assumptions and several other improvements over the 1999 cellulase enzyme production model. We note that by including an on-site enzyme production section, NREL and DOE are not making a judgment about whether or not the cellulosic ethanol industry should align to this mode of enzyme distribution. Rather, the model on-site enzyme section is intended to improve transparency in determining the true cost of cellulase enzymes for large-scale cellulosic ethanol production.

The present design considers submerged aerobic cultivation (“aerobic fermentation”) of a T. reesei-like fungus on a feedstock of glucose and fresh water. Producing cellulase enzymes with glucose is not straightforward, because the absence of cellulose does not encourage the microorganism to secrete cellulase enzymes. Here, we have assumed a media preparation step where a small fraction of glucose is converted to sophorose, a powerful inducer of cellulase, using a small amount of the cellulase enzyme itself. When grown on this substrate, T. reesei has been shown to productively secrete cellulase [53]. Using glucose as the substrate is not necessarily more expensive than using hydrolysate slurry from pretreatment because the expected enzyme titer is significantly higher with glucose, reducing the capital and utility costs compared with using hydrolysate. Figure 9 is a simplified flow diagram of the enzyme production section.

Figure 9. Simplified flow diagram of the enzyme production process
Glucose + water
Sophorose conversion enzyme
To hydrolysis
Media prep
Aerobic culture (fed-batch)
Holding tank
Glucose/sophorose Air
Seed train (Trichoderma reesei)

37
3.4.2 Design Basis

The on-site enzyme process was designed without input from enzyme companies or other protein production experts, although several individuals knowledgeable about this topic did participate in the peer review of this report. Based on the claims in U.S. Patent 4,762,788 (Example 5) [54] and a few reasonable assumptions, we have developed a rudimentary process that is adequate for our needs. The key assumptions used in the current design are summarized in Table 18. Note that the mass yield of enzyme from glucose is actually a computed number that is dependent on assumptions regarding protein composition and microorganism-specific productivity, which will be described below.

Table 18. Area 400 Guiding Design Basis Assumptions
Parameter Assumption
Protein loading to enzymatic hydrolysis 20 mg protein/g cellulose
Reactor size 300,000 L @ 80% final working volume
Enzyme titer at harvest 50 g/L
Mass yield of enzyme from glucose 0.24 kg enzyme/kg glucose
Enzyme production cycle time 120 h online, 48 h offline, 168 h total

The desired cellulase loading to enzymatic hydrolysis is 20 mg of enzyme protein per g of cellulose. “Protein” here refers to the total amount of high molecular weight protein in the enzyme broth as determined by assay; not all of this protein is active cellulase. The total protein demand was thus calculated to be 490 kg/h (1,080 lb/h). An additional 10% is produced to account for the slipstream provided to the media preparation tank to make the glucose/sophorose mixture. The size of the cellulase production vessels was chosen to be 300 m3 (80,000 gal) with a height-to-diameter ratio (H/D) of 2. Fermentation is assumed to be a fed-batch process starting at 50% working volume and ending at 80%. Over one week, each bioreactor will see a 24-hour cell growth period, a 96-hour protein production period, and a 48-hour offline period for draining, cleaning, and refilling. With a one-week total cycle time and the production parameters listed in Table 18, one bioreactor is capable of producing 12,000 kg of protein in a week, or 71.4 kg/h (157 lb/h). The equivalent enzyme volumetric productivity is 0.30 g protein/L-h. Nine reactors were therefore required to deliver the 490 kg/h of protein needed for enzymatic hydrolysis.

The reactors are loaded initially with the glucose/sophorose carbon source and nutrients including corn steep liquor (CSL), ammonia, and SO2. After the initial cell growth period, additional substrate is added to maintain protein production. The bioreactors are sparged with compressed and cooled air and corn oil is added as an antifoam. The reactors are temperature controlled by chilled water flowing through internal coils. 

To determine the aeration and agitation requirements for the production bioreactors, the oxygen transfer rate was set equal to the oxygen uptake rate (OTR=OUR), with the OUR computed stoichiometrically from the protein production rate. In the modeled bioreactors, the reaction stoichiometry balances the reactions of substrate, oxygen, ammonia, and SO2 to cell mass and enzyme (plus CO2 and water) using an elemental composition for commercial cellulase provided by Novozymes [55]. The composition of cell mass was taken as the average of a generic cell mass composition [56] and the enzyme composition, with the assumption that cell mass includes some unreleased protein.

38
Cellulase protein: CH1.59N0.24O0.42S0.01

T. reesei cell mass: CH1.645O0.445N0.205S0.005

In the production bioreactors, it is assumed that 90% of the carbon source is converted via the protein reaction and 10% is converted via the cell mass reaction. In the seed reactors, 85% of the carbon is converted via the cell mass reaction and 5% via the protein reaction, with 10% unreacted. This represents an overall molar selectivity of glucose to 31% protein, 4% cell mass, and 65% CO2, yielding 0.24 kg enzyme protein/kg glucose. The total oxygen demand for one bioreactor producing 12,000 kg protein in 120 hours online is 8.4 kmol/h. At its maximum (i.e., at the initial working volume of 50%), the OUR is 56 mmol/L-h.

The OTR is the product of the volumetric mass transfer coefficient kla (h-1) and the log mean oxygen concentration gradient (the difference between the saturated dissolved oxygen concentration and the desired dissolved oxygen concentration) at the top and bottom of the bioreactor operating volume:
OTR ൌ ݇௟ܽ
ሺ כ ௕ܥെ ஽ܥሻ െ ሺܥ௧  כെ ஽ܥሻ
ln ൬ ௕ܥ ܥ௧  כ כെ  ܥെ ஽ ஽ܥ൰

where Cb* and Ct* are the saturated dissolved oxygen concentrations (mmol/L) at the bottom and top of the vessel, respectively, and CD is the desired dissolved oxygen concentration, which is assumed to be 30% of saturation at 1 atm absolute pressure (0.063 mmol/L). The top and bottom concentrations of saturated dissolved oxygen were calculated by Henry's Law:

௅ܥܪ  ൌߨ

where π is the partial pressure of oxygen (atm), H is Henry’s coefficient (atm/(mmol/L)), and CL is the liquid concentration of the gas (mmol/L). Henry’s coefficient for oxygen in water was set equal to 1 atm/(mmol/L) for all calculations. (Henry’s coefficient for oxygen in pure water is approximately 1.3 atm/(mmol/L) at 25°C, but solubility may be affected by the non-water components in the broth; a coefficient of 1 is a reasonable initial estimate.) The pressure at the top of the vessel was taken to be 1 atm and the pressure at the bottom was determined by the static head of liquid in the vessel. The volumetric mass transfer coefficient was then computed using the following correlation [57]:

݇௟ܽ ൫hିଵ൯ ൌ 8.42 ൬ܸ ܲ ௅൰଴.ଷଷ ܸீ ଴.ହ଺

where P is the impeller power consumption and VL is the working volume. The correlation assumes that P/VL is expressed in hp/1,000 L. VG is the superficial gas velocity (cm/s) in the head space. This correlation is intended for non-Newtonian fungal cultivation systems with a maximum volume of 30 m3. Our bioreactors exceed the maximum intended volume for this correlation by several orders of magnitude but we believe that this equation yields results that are reasonable enough in the absence of more sophisticated reactor design involving computational fluid dynamics and so on.

39
Because we have assumed a fed-batch fermentation, the working volume varies over time, along with the OTR and aeration rate in vvm (standard volume of air per volume of liquid per minute), which are volumetric quantities. In absolute terms, the average aeration rate for a VG of 200 cm/min was 0.83 standard m3/s (including two days of offline time). The average impeller power P was determined to be 260 kW (350 hp), with a maximum of 600 kW (800 hp). The final specifications for the cellulase production bioreactors are shown in Table 19.

Table 19. Specifications of the Enzyme Production Bioreactors
Total volume 300 m3 / 80,000 gal
Maximum working volume 80%
H/D ratio 2
Height 11.5 m
Diameter 5.75 m
Operating pressure 1 atm
Operating temperature 28°C (82°F)
Material 316SS
Agitator 800 hp

Four trains of three seed fermentors provide inoculum to the production bioreactors. Each vessel in the seed trains is run batchwise on the same substrate as the production vessels. Air is also sparged through each of the seed vessels, which are cooled with chilled water. The seed bioreactors are each sized at 10% of the next bioreactor volume, i.e., 0.3 m3, 3 m3, and 30 m3. The aeration demand is assumed to be 10% of the production aeration rate. Four trains were chosen because each production fermentor has a total cycle time of 7 days, while each seed fermentor should have a cycle time of 2 days (including cleaning and sterilization) to get through the cell growth phase only.

Like the oxygen uptake rate, the glucose demand is also computed stoichiometrically from the required protein production rate. Ammonia and SO2 are fed to the reactors stoichiometrically and CSL, trace nutrients, and antifoam (corn oil) are added to the substrate based on flow rate. The required nutrient concentrations are taken from Schell et al. [58] and are restated in Table 20.

Table 20. Cellulase Production Nutrient Requirements
Component Amount
Ammonia Stoichiometric (approx. 7 g/L)
SO2 Stoichiometric (approx. 0.6 g/L)
CSL 1% w/w
Corn oil 0.1% v/v
Ammonium sulfate 1.4 g/L
Potassium phosphate 2.0 g/L
Magnesium sulfate 0.3 g/L
Calcium chloride 0.4 g/L
Tween 80 0.2 g/L

Glucose, the carbon source for cell mass and protein, is the most significant enzyme production expense in this model. Electricity is also a significant contributor due to the power requirements of air injection, agitation, and refrigeration. The electricity demand in the enzyme production area is summarized in Table 21.


40
Table 21. Cellulase Production Electricity Requirements
Air compressor 1,408 kW
Agitators 2,326 kW
Chiller system (Area 400 contribution) 1,587 kW
Total electricity (includes pumps, etc.) 5,340 kW
Total electricity demand per kg protein 9 kWh/kg

3.4.3 Cost Estimation

Most equipment in this area is stainless steel. The air compressor and some of the nutrient delivery equipment items are specified as carbon steel. Harris Group obtained quotes for the production bioreactors (F-400) from Mueller, with internal cooling coils included. The production agitators and motors were quoted by Lotus. The smaller seed fermentors were quoted by A&B Process Systems as complete skid-mounted units with cooling jackets and agitators. The air compressor is a packaged unit from Dresser Roots, capable of delivering 8,000 SCFM of air at 3 atm. Harris Group developed costs for the pumps in this area using their internal database.

Not included in the enzyme production model are any costs for concentration, stabilization, or transportation of the enzyme to the plant. At the very least, one expects to have to pay licensing fees for the cellulase production microorganism, but these costs are not included because we lack information on what they might be (though an educated guess might be 5 cents or less per gallon of ethanol).

3.4.4 Enzyme Cost Discussion

The 2002 design model and subsequent analyses using that model assumed that cellulase enzymes had a fixed contribution to the MESP that was independent of the ethanol yield. This value was taken from the Multi-Year Program Plan (MYPP) of DOE’s Office of the Biomass Program [27], which in earlier editions stated that using technology available in 2009, the enzyme cost contribution should be $0.35/gal (2007$) and should decrease to $0.12/gal ethanol by 2012. These values were computed by NREL based on projections made by enzyme companies in 2005, following a DOE-funded research campaign that helped to significantly reduce cellulase enzyme production costs [59]. Enzyme costs in this range were considered realistic if production costs associated with transportation and formulation costs were eliminated, i.e., if the enzymes were produced on-site or near-site and were not formulated for stability during extended storage [60, 61].

Since the 2005 projections, DOE negotiated additional awards with several enzyme manufacturers [49] to further develop improved cellulase preparations and drive down production costs to the levels specified in the MYPP. In the process, DOE and NREL both received feedback from the enzyme industry that even $0.35/gal might be too optimistic for currently-available enzymes. Along those lines, in February 2010 the major enzyme manufacturers Genencor and Novozymes announced new commercial-grade cellulase enzyme preparations capable of higher performance at lower loadings. Both cited an enzyme cost contribution of approximately $0.50/gal ethanol [62, 63]. 

Based on the economics of the on-site enzyme section described above, the predicted cost of enzymes to the ethanol plant is $0.34/gal of ethanol. This is broken down as shown in Figure 10.

41
The carbon source (glucose) makes up 57% of the cost of the enzyme, i.e., $0.19/gal of the $0.34/gal is just for glucose. We can back out the unit cost of the enzyme from $0.34/gal by multiplying by the ethanol production rate and dividing by the enzyme flow rate, which works out to $4.24/kg protein.

Figure 10. Enzyme production cost breakdown
Capital 21%
Glucose 57%
Other Nutrients 5%
Electricity 13%
Fixed Costs 4%
$0.34/gal ethanol
$4.24/kg protein
DW1102A

The previous DOE target for enzyme cost was specified as $0.12/gal ethanol, or about one third of what is reported here. One way to achieve such a low cost contribution would be to reduce the enzyme loading. In Figure 11, we see that the enzyme contribution to MESP is roughly linear with the enzyme loading (mg of enzyme per g of cellulose entering enzymatic hydrolysis). At the loading specified in the present design (20 mg/g), the enzyme contribution is $0.34/gal. The enzyme contribution approaches $0.12/gal at about 8 mg/g loading. Therefore, the original enzyme cost targets could potentially be achieved by a reduction in enzyme loading, but such a loading would be significantly lower than what we currently use to approach the 90% cellulose conversion yield target.

42
Figure 11. Enzyme contribution to MESP as a function of loading
$-
$0.10
$0.20
$0.30
$0.40
$0.50
$0.60
$0.70
0 10 20 30 40 50
Enzyme Contribution $/gal
Enzyme Loading mg/g cellulose

The lower limit of enzyme loading is not well understood. In theory, enzyme molecules are not consumed during the hydrolysis reaction but, over time, they may become inactivated by denaturation or irreversible binding to solid particles, especially when lignin is present. Bench and pilot-scale experiments at NREL are therefore typically overloaded (i.e., an excess of enzyme is used) to ensure complete hydrolysis, because we may only have the resources to run a limited number of experiments. However, we have observed that advanced enzymes demonstrate diminishing increases in conversion at loadings as low as 20 mg/g. Ultimately, the lower limit of enzyme loading will be determined by industry and enzyme manufacturers, and will likely decrease as pretreatment technologies and enzyme preparations continue to improve. For the resent design, however, NREL was not comfortable modeling an enzyme loading less than 20 mg/g.

The enzyme cost contribution modeled here is lower than one would expect for an enzyme preparation purchased from a separate, non-adjacent production facility. Transportation of the enzyme to the ethanol plant could alone add $0.09–$0.18/kg of product, even if formulation costs could be avoided. Furthermore, by lumping the enzyme production equipment in with the ethanol plant, some key items are inherently shared, e.g., the land and buildings, cooling tower, and utilities infrastructure. Overhead and fixed costs, especially labor and management, would also be higher for a standalone facility. Eliminating the shared aspects between the enzyme unit and the ethanol plant could easily add another 5 cents per gallon of ethanol to the enzyme contribution. Additionally, an external enzyme production facility would probably demand a higher rate of return than the 10% IRR assumed for the ethanol plant because it is a higher-risk and lower-volume business. Including all these extra costs would bring the total enzyme cost contribution in line with the $0.50/gal level cited in the press.


43
Although the on-site enzyme cost contribution derived in our analysis is lower than what might be expected in a purchased-enzyme scenario, it does not necessarily make a strong argument for on-site production. The cellulase production unit described here, consisting of nine fermentors and four seed trains, is hardly a “plug-and-play” solution, and an ethanol producer could be forgiven for not wanting to assume the mantle of logistical and operational challenges associated with such a system. However, the cost benefits of co-location are real, and the economics of cellulase production are arguably so tightly coupled to those of the fuel product itself that an on site cellulase facility might ultimately make economic sense in the future cellulosic ethanol industry. In the near term, however, it is more likely that ethanol plants will purchase enzyme from an external supplier who has an organization dedicated to improving enzyme performance and reducing costs.

44
3.5 Area 500: Product, Solids, and Water Recovery

3.5.1 Overview

Area 500 separates the fermentation broth from Area 300 into water, anhydrous ethanol, and combustible solids. Distillation and molecular sieve adsorption are used to recover ethanol from the raw fermentation beer and produce 99.5% ethanol. Distillation is accomplished in two columns. The first, called the beer column, removes the dissolved CO2 and most of the water. The second column is called the rectification column and concentrates the ethanol to a near azeotropic composition. See Figure 12 for a process overview of this area.

ATM.
LP STEAM
CW
LP STEAM
CW
Fermentation Vents
Beer
Lignin to combustor
Stillage to WWT
Lignin Separator
Beer Column
Water to recycle
Regenerate
Ethanol product
Return to beer well
Clean water
Rectification
Column Molecular Sieve
Adsorption
Vent Scrubber
Figure 12. Simplified flow diagram of the separation process


The ethanol product leaves the rectification column at ~92.5% ethanol and is further dehydrated to 99.5% by vapor-phase molecular sieve adsorption. During regeneration of the adsorption columns, a low-purity (70 wt %) ethanol stream is generated and is recycled back to the rectification column for recovery. The beer column overhead stream is fed to a water scrubber along with the fermentation vents (containing mostly CO2 but also some ethanol), thereby recovering nearly all of the ethanol. The scrubber effluent is fed back to the beer well. 

The beer column bottoms (stillage) stream contains the unconverted insoluble and dissolved solids. The insoluble solids are dewatered by a pressure filter and sent to the combustor in Area 800. The pressed stillage water cannot be recycled directly back to the process because it contains high levels of organic salts such as ammonium acetate and ammonium sulfate, fermentation nutrients not consumed by the organism, and soluble inorganic compounds from the biomass. Instead, the pressed stillage water is directed to wastewater treatment (Area 600) for cleanup.

45
3.5.2 Design Basis

Beer from the fermentation area (5.4 wt % ethanol) is fed to the beer column after passing through an economizing heat exchanger with the bottoms stream (PFD-P120-A501, Appendix E). The beer column (D-501) operates in a mode that removes the CO2 and as little ethanol as possible to the overhead while removing about 90% of the water to the bottoms. The ethanol is removed as a vapor side-draw from the column and fed directly to the rectification column (D-502). Both columns are modeled with rigorous vapor-liquid equilibrium calculations in Aspen using the RADFRAC model. This is an improvement over the 2002 Aspen model, where the rectification column was modeled as a fixed separation block. This results in a more accurate determination of reboiler and condenser duties for the columns. We note that our Aspen model was not used by the distillation vendor (Megtec) in designing these columns—they arrived at a similar design using their own models.

In the Aspen model, the beer column (D-501) contains 32 stages operating at 48% efficiency, with the feed entering on the fourth tray from the top. The molar reflux ratio required is 3:1. The overhead is vented to the scrubber and contains 85% CO2, 11% ethanol, and close to 4% water. All of the CO2 and only 0.3% of the ethanol entering the beer column is vented here. Most of the ethanol that is vented (99%) will be recovered in the vent scrubber and recycled. In addition, about 0.8% of the ethanol fed to the beer column is lost in the bottoms stream and is considered a permanent loss. More than 99% of the ethanol in the feed is removed as a vapor side-draw from the column at Tray 8 at 40 wt %. To minimize the ethanol loss in the bottoms, the beer column reboiler duty is kept relatively high, so there is a trade-off between ethanol loss and energy usage. Megtec designed the beer column with 32 fixed-valve trays. These have been found to tolerate solids well and have a reasonably good efficiency. The tray spacing is 24 in. and the column diameter is 14 ft. Heat is supplied to a forced-circulation reboiler (H-501) by low pressure (9.5 atm [125 psig]) steam. The forced-circulation reboiler was considered necessary to accommodate the solids present in the beer column bottoms. The beer column is operated at 2 atm (15 psig) overhead pressure to keep the reboiler temperature low in order to minimize fouling.

The vapor side-draw from D-501 is fed directly to the rectification column, D-502. This column uses 45 stages with an efficiency of 76%. The D-501 vapor is fed on Tray 33 (counting from the top). The recycle from the molecular sieve, which is higher in ethanol (72 wt % versus 40 wt %), is fed on Tray 14. The required molar reflux ratio is 3.5:1 to obtain a vapor overhead mixture of 92.5% w/w ethanol and a bottoms composition of 0.05% w/w ethanol. Only 0.1% of the ethanol from fermentation is lost in the bottoms. The rectification column bottoms stream is recycled to the pretreatment reactor as dilution water; ethanol in this stream is not considered a loss. The 7.5% water in the rectification column overhead represents only 0.7% of the water originally entering distillation. Megtec designed the rectification column with 45 valve trays. Above Tray 15, the column is 13 ft in diameter; below Tray 15 it is 4.5 ft in diameter. (Structural supports for this tower are included in its installation cost.) Heat is supplied to the column in a thermosiphon reboiler (H-502) by low-pressure steam. For the present design, an air-cooled condenser was specified to condense the reflux. This was done to reduce evaporative losses from the cooling tower and will be discussed more in Section 5.2. 

The ethanol-containing vent from the beer column overhead, along with the vents from the seed and production fermentors in Area 300, is sent to a water scrubber (T-512). The scrubber column recovers 99% of the vented ethanol. The scrubber effluent contains 1.8 wt % ethanol and is returned to the beer well. The scrubber is designed for absorption of >99% of the ethanol in the vents and no more than 40 tons per year of VOC (volatile organic compound) emissions for air pollution considerations. Higher water flow or lower water temperature could reduce VOC emissions from the vent scrubber, at a potentially significant increase in operating cost and water consumption.

46
The overhead vapor from D-502 is fed to a molecular sieve adsorption unit (M-503), which is a system of columns packed with beds of adsorbent. Water is selectively adsorbed in the beds as the vapor flows through. The design specifics of this unit are not detailed here, but the general arrangement is given in PFD-P120-A503 (Appendix E). Saturated vapor from the rectification column is superheated and fed to one of two adsorption columns. The adsorption column removes 95% of the water and a small amount of ethanol. The 99.5% pure ethanol vapor is cooled by heat exchange with the regeneration condensate and finally condensed with cooling water and pumped to storage. While one bed is adsorbing water, the other is regenerating. The bed is regenerated by passing a small slipstream of pure ethanol vapor back through the water saturated bed while a vacuum is applied. The ethanol strips the water off the adsorbent, and the mixture is condensed and returned to the rectification column (D-502).

Finally, the beer column (D-501) bottoms stream is cooled to 47°C (117°F) in the feed/bottoms economizer; this is a suitable temperature for liquid-solid separation. The cooled material is separated in a pressure filter (S-505, PFD-P120-A505). The pressure filter is operated without a wash, and the cake is dried with air to 35% moisture. The drying air is sent to the combustor, and the pressed stillage water is sent to wastewater treatment in Area 600. This is a significant change from the 2002 process, in which the stillage was evaporated to a combustible syrup, with the evaporator condensate being recycled to the process. The effects of this change on the wastewater treatment area will be discussed in Section 3.6.

A clean-in-place system (part of Area 900) services the equipment in this area that is prone to fouling (e.g., the beer column reboiler) by flushing with a hot caustic solution and circulating the solution until heat transfer surfaces are clean. Manual acid cleaning must be performed occasionally to remove mineral scale.

3.5.3 Cost Estimation

The construction material for equipment in the distillation area is generally 316SS. The beer column and rectification column were quoted by Megtec. The two columns were quoted as a package along with all pumps, heat exchangers (except the rectification column condenser), and reflux drums. The air-cooled rectification column condenser was quoted by GEA Rainey. The molecular sieve adsorption unit was quoted by Delta-T and the vent scrubber system was quoted by Envitech. The lignin separator was quoted by Larox as two FFP 2512 60/60 filter-press units. Harris Group used information and experience from other projects to estimate costs for the rest of the equipment, including solids handling equipment, pumps, and auxiliary tanks.

47
3.6 Area 600: Wastewater Treatment (WWT)

3.6.1 Overview

The ethanol process generates a number of wastewater streams that must be treated before recycle to the process or release to the environment. This is accomplished in the wastewater treatment system in Area 600. The treated water is assumed clean and fully reusable by the process, which reduces both the fresh makeup water requirement and discharge to the environment.

Figure 13 is a simplified flow diagram of the WWT area. Condensed pretreatment flash vapor, boiler blowdown, cooling tower blowdown, and the pressed stillage water streams are mixed together. The combined wastewater stream is processed by anaerobic digestion and aerobic digestion to digest organic matter in the stream. Anaerobic digestion produces a biogas stream that is rich in methane so it is fed to the combustor. Aerobic digestion produces a relatively clean water stream that can be reused in the process as well as a sludge that is primarily composed of cell mass. The sludge is also burned in the combustor.

Beer stillage
Cooling tower blowdown
Pretreatment flash
Boiler blowdown Biogas CH4/CO2
Air Vent to atmosphere
Digester sludge
to combustor
Treated water
Aerobic Digestion
Anaerobic
Digestion
Clarifier
Dewatering
RO
Waste brine
Evaporator
Figure 13. Simplified flow diagram of the wastewater treatment process

In previous designs, the stillage from the beer column was evaporated in Area 500 to yield a syrup that could be routed to the combustor, minimizing the loading to WWT in that model. In the present design, this process flow was ruled out because of the switch to ammonia conditioning in Area 200. In the 2002 design, sulfate ions introduced in dilute-acid pretreatment precipitated as gypsum after overliming and were removed from the process. With the switch to ammonia conditioning, the resultant ammonium sulfate and ammonium acetate salts remain in the process and end up in the stillage. When we modeled evaporation of the stillage to syrup, the salt concentrations in the syrup were so high that boiler vendors were not comfortable quoting a combustor system to handle it, due to concerns of burner fouling. We chose, therefore, to eliminate the stillage evaporators and route the stillage to wastewater treatment instead. 

While we were confident that anaerobic and aerobic digestion could satisfactorily treat the organic material flowing to WWT in our design, some technology vendors expressed concern with the concentrations of ammonia and sulfate and indicated that these could require special upstream cleanup steps, at additional cost and complexity. In 2010–2011, NREL therefore contracted with Harris Group and Brown and Caldwell (BC) to design a treatment system using actual material generated in the pilot plant. Their testing determined that upstream removal of sulfur was not required for our process but that nitrification would be required in conjunction with aerobic digestion to handle the ammonia.

48
The wastewater treatment technology described here deviates significantly from current corn ethanol plants, which strive toward zero-liquid-discharge designs [64]. Such plants may have aerobic digesters or even simple reverse-osmosis systems on internal recycle streams. The deviation in wastewater treatment technology here reflects the challenges inherent in cleaning u inorganics (fertilizer, etc.) that are found on the non-food portion of a food crop and corrosive chemicals added in the front end to overcome lignocellulosic biomass recalcitrance. 

3.6.2 Design Basis

The wastewater treatment system was designed by Harris Group and Brown and Caldwell unde the 2010 subcontract mentioned above. The design includes anaerobic digestion, aerobic digestion with nitrification, sludge dewatering, and reverse osmosis. Additional details can be found in the subcontract report [65]. The relevant design parameters of the wastewater system are summarized in Table 22. Some of these quantities were adjusted from what was determined by laboratory analysis to avoid artificially overdesigning the system for the rich fermentation media components and high suspended solids in the sample.

Table 22. Wastewater Treatment System Design Basis
Hydraulic load 2.15 MMgal/d
Wastewater inlet temperature 50°C
Inlet pH 5.2
Total COD 87 g/L
Soluble COD 85 g/L
Total solids 68 g/L
Total suspended solids 1.5 g/L
Total alkalinity 2,750 mg/L as CaCO3
Ammonia-N 1,060 mg/L
Total Kjeldahl N 1,200 mg/L
Sulfate 4,400 mg/L
Silica 1,600 mg/L
Potassium 500 mg/L
Phosphate 805 mg/L

Upsets (including unusual suspended solids, fouling, etc.) and other intermittent loads (e.g., from process spills) were not considered in the design. Rain and snow run-off, equipment washing, and other non-process wastewater are assumed to flow to a municipal wastewater treatment system. Insoluble organic compounds like cellulose, xylan, and protein are assumed inert in anaerobic digestion, although these are largely removed upstream in the stillage lignin separator (Area 500). BC indicated that these solid components could be handled in WWT for roughly the same capital cost, but additional operating costs due to nitrification requirements of the protein fraction were prohibitive.

The process flow is detailed in PFD-A120-A601 and PFD-A120-A602 (Appendix E). The pressed stillage water, condensed pretreatment flash vapor, boiler blowdown, and cooling tower blowdown are mixed together and pumped through a heat exchanger (H-602) and cooled to 35°C. The cooled stream then flows directly to the anaerobic digester (T-606).

49
The total chemical oxygen demand (COD) entering anaerobic digestion in the design case is approximately 26,500 kg/h (58,300 lb/h) (equivalent to 64 g/L). In anaerobic digestion, 91% of each organic component is destroyed; 86% is converted to biogas (methane and carbon dioxide) and 5% is converted to cell mass. Methane is produced from the utilized organic matter at 228 g/kg COD removed. Carbon dioxide is also produced at a nearly equimolar rate to methane, such that the biogas from the digester is 51% CH4/49% CO2 on a dry molar basis. Cell mass is produced at a yield of 45 g cell mass per kg COD digested. Sulfate is converted to hydrogen sulfide (H2S) and leaves the system in the biogas. Since the COD-to-sulfate ratio in the design basis is ~20, the methane-producing organisms will out-compete the sulfate-reducing organisms, so upstream removal of sulfate is not necessary.

During standard operation, the biogas will flow to the combustor, providing about 65 MMkcal/h (260 MMBtu/h) or 36% of the total fuel supplied to the combustor. The H2S in the biogas will be treated downstream of the combustor with flue gas desulfurization (Area 800). An emergency biogas flare is designed into the process to burn the biogas in case of a process upset in the combustor.

The liquid from the anaerobic digester is pumped to aerobic activated-sludge lagoons with floating aerators (T-608). In the lagoons, 96% of the remaining soluble organic matter is removed, with 74% producing water and carbon dioxide and 22% forming cell mass. With a 91% reduction of the COD in anaerobic digestion followed by a 96% reduction of the remaining COD in aerobic digestion, the total COD reduction is 99.6%. Ammonium ions from the stillage pass through to aerobic digestion where they are converted to nitrate by nitrifying bacteria. Because the nitrification process lowers the pH (by forming nitric acid), caustic must be added to the lagoons for neutralization.

The fully digested material is pumped to a membrane bioreactor (R-609) for clarification. The membrane unit removes additional COD along with colloidal particles (especially silica). Coarse- and ultra-filtration upstream of the membrane unit separate the aerobic biomass sludge. Most of the sludge is recycled to the lagoons to maintain a high cell mass loading. The remaining portion is removed to a holding tank, where it is mixed with sludge from anaerobic digestion.

The sludge in the holding tank is dewatered periodically using a centrifuge (S-611). The centrifuge solid is primarily cell mass and is conveyed to the combustor for disposal (C-614). The water leaving the centrifuge is recycled to the aerobic lagoons for additional treatment.

The treated water has a COD of about 0.5 g/L and is routed to a reverse osmosis (RO) membrane system for salt removal. Approximately 80,000 L/hr (350 gpm) of water is rejected from RO as a 7% brine containing primarily sodium nitrate along with all remaining ions and organics. The RO water effluent is assumed to be pure and is mixed with process makeup water and recycled to the process. The brine from RO is further concentrated in a mechanical-vapor-recompression evaporator (M-640) to 50% solids and the condensate is also recycled to the process. We do not further process the brine in our model at this time, and it is assumed to be waste. In reality, one may choose to further crystallize the brine for solid disposal. Some biomass burners may be designed to handle the salt (turning sodium nitrate into N2, NOx, and soda ash). It may also be possible to use flue gas to spray-dry this material.

50
3.6.3 Cost Estimation

Harris Group and Brown and Caldwell estimated cost for the wastewater system, drawing on support from technology vendors such as ADI and Biothane. While the BC estimate included a complete project cost work-up, we have only used the installed equipment costs in our technoeconomic model because we account for our own indirect and project costs at the plant level. To the extent that the cost data obtained by BC were publishable, details can be found in the subcontract report [65]. Harris Group also generated costs for the wastewater cooler (H-602) and sludge screw conveyor (C-614).

3.6.4 Wastewater Challenges

The switch from overliming to ammonia conditioning in Area 200 has forced a major change in our WWT design. In overliming, the sulfate from sulfuric acid pretreatment was removed after conditioning in the form of “gypsum” (calcium sulfate). Previous work showed that this waste product was about 70% gypsum; the rest was unknown organics that could possibly be classified as hazardous waste requiring remediation (e.g., phenolics) [66]. The disposal cost of this material was therefore not well defined in the 2002 model, and ultimately the sugar losses associated with overliming were unacceptable, prompting the switch to ammonia conditioning.

Because the stillage containing ammonium and sulfate salts could no longer be concentrated into a combustible syrup, as noted earlier, the chosen alternative was to route the stillage to wastewater treatment. The ammonia is removed from the system as sodium nitrate (which requires caustic) and the sulfate is removed as gypsum from the combustor flue gas (which requires lime). At this point, readers may question the wisdom of replacing lime in pretreatment with the combined requirement of ammonia in pretreatment, caustic in WWT, and lime in FGD; this is a valid and open question. However, NREL feels that going back to overliming is not the obvious solution, given the cost of hydrolysate solid-liquid separation, uncertainty around the cost of gypsum disposal, and staggering sugar losses associated with overliming. We will investigate how these options affect process economics and sustainability in a future study. The primary research path, as discussed in Sections 3.2 and 3.3, is to reduce the amount of chemicals added in pretreatment and thereby move to so-called no-conditioning processes that may be applicable given the advanced enzymes and fermentation organisms currently in development. This should reduce or eliminate the need for removal of inorganic material from wastewater and bring the plant more in line with current corn ethanol technology. 

51
3.7 Area 700: Product and Feed Chemical Storage

3.7.1 Overview

This portion of the plant provides bulk storage for process chemicals and the ethanol product. The chemicals stored in this area include ammonia, corn steep liquor (CSL), sulfuric acid, and gasoline (used as a denaturant for the ethanol product). Water for fire suppression is also stored here.

3.7.2 Design Basis

Table 23 shows the major storage requirements for the present design. PFDs for the storage area can be found in PFD-P120-A701 and PFD-P120-A702 (Appendix E).

Table 23. Storage Requirements
Material Tank No. Size
Ethanol product T-701 Sufficient to contain 7 days of production: 2 carbon steel tanks @
750,000 gal each
Gasoline denaturant T-710 7 days of blendstock: 1 carbon steel tank @ 65,000 gal
Sulfuric acid (93%) T-703 5 days of storage: 1 carbon steel tank @ 12,600 gal
Ammonia T-706 5 days of storage: 2 SA-516-70 tanks @ 28,000 gal. Ammonia is
stored anhydrous at 250 psig.
Fire water T-704 4 hours of fire suppression @ 2,500 gpm: 1 glass-lined carbon steel
tank @ 600,000 gal
Corn steep liquor Diammonium phosphate (DAP) T-720 5 days of storage: 1 glass-lined carbon steel tank @ 70,000 gal

T-760 7 days of storage: 1 SS304 tank @ 12,800 gal

DAP is assumed to be packaged in super-sacks and is unloaded via solid feeder (C-755), requiring an unloading blower (P-755) and DAP vent baghouse (S-755). From the storage bin, DAP is fed into a day tank (T-760) where it is mixed with water with a 5-hp agitator. The DAP solution is pumped (P-760) to fermentation. The ethanol product pump (P-701), sulfuric acid pump (P-703), ammonia pump (P-706), CSL pump (P-720), and gasoline pump (P-710) are sized for quick loading and unloading of trucks. The fire water pump (P-704) is sized for 2,500 gpm.

3.7.3 Cost Estimation

Harris Group developed costs for most of the equipment in this section using their internal cost database. Quotes for some of the more specialized-material tanks were obtained from Mueller or Trinity Tank (via Chemithon). Quotes for agitators for the DAP and CSL tanks were obtained from Lotus, Inc.


52
3.8 Area 800: Combustor, Boiler, and Turbogenerator

3.8.1 Overview

The purpose of the combustor, boiler, and turbogenerator subsystem is to burn various organic by-product streams to produce steam and electricity. Combustible by-products include all of the lignin and the unconverted cellulose and hemicellulose from the feedstock, biogas from anaerobic digestion, and biomass sludge from WWT. Burning these by-product streams to generate steam and electricity allows the plant to be self-sufficient in energy (“thermal-neutral”), reduces solid waste disposal costs, and generates additional revenue through sale of excess electricity.

The fuel streams are fed to a combustor capable of handling the wet solids. A fan moves air into the combustion chamber. Treated water enters the heat exchanger circuit in the combustor and is boiled and superheated to high-pressure steam. A multistage turbine and generator are used to generate electricity. Steam is extracted from the turbine at two different conditions for use in the process. In the final stage of the turbine, the remaining steam is taken down to a vacuum and condensed with cooling water for maximum energy conversion. The condensate is returned to the boiler feed water system along with condensate from the various heat exchangers in the process. The steam turbine turns a generator that produces AC electricity for all users in the plant. The balance of electricity is assumed to be sold back to the grid, providing a co-product credit.

3.8.2 Design Basis

The moisture of the combined solid feed to the combustor is 44%; a small amount of additional moisture is entrained in the biogas. Given the fuel disposition, Babcock & Wilcox recommended a TowerPak Stirling Power Boiler system. This system features a live-bottom grated fuel bin to ensure drying and complete combustion of the wet solid fuel. The system was quoted to produced 525,000 lb/h (239,000 kg/h) of steam at 850°F (454°C) and 900 psig. Boiler efficiency, defined as the percentage of the feed heating value that is converted to steam heat, is ~80%.

Flue gas from the combustor preheats the entering combustion air then enters a spray dryer for flue gas desulfurization (FGD). Due to the switch to ammonia conditioning, the sulfur content in the combustor feed is significantly higher than it was in the 2002 design. All of the sulfur entering the combustor is converted to sulfur dioxide, and its concentration in the flue is >1,800 ppmw. This level of SO2 requires FGD. Lime (calcium hydroxide) is sprayed into the flue gas as a 20 wt % slurry at 20% stoichiometric excess. FGD converts 92% of the SO2 into calcium sulfate, which falls out the bottom of the spray dryer. The water in the slurry is vaporized and exits with the flue gas to the baghouse. The baghouse removes particulate ash, which is landfilled along with the calcium sulfate. The scrubbed gas is exhausted through a stack. 

Pretreatment research is currently targeting a lower acid use, so we will revisit the issue of SO2 emissions in the future. Additionally, 1% of the generated sulfur dioxide is converted to sulfuric acid. The presence of this acid requires that the flue gas temperature be kept above the dew point to avoid corrosion.

Other pollutant generation rates were not changed from the 2002 design [67] and are computed based on the heating value of the combustion feed stream. Carbon monoxide is assumed to be generated at a rate of 0.31 kg/MWh (0.2 lb/MMBtu). Nitrogen oxide, or NOx, is generated at 0.31 kg/MWh (0.2 lb/MMBtu). NOx formation is a complicated mechanism and depends on the feed, combustion temperatures, excess air rate, combustor design, and the presence of flue gas cleanup devices like FGD. The fate of the ammoniated salts in the combustor feed is not well understood, but it is likely that some of the ammonia is converted to nitrous oxide (N2O) while also acting to reduce NOx formation [68]. (Ammonia injection is indeed one way to reduce NOx emissions.)

53
On the steam side, the boiler feed water (BFW) system includes a softener (M-820) for the makeup and condensate water, a deaerator (T-826) to remove air and other non-condensables, surge tanks, and pumps. Makeup water and condensate are treated and deaerated in these units then preheated with steam to 177°C (351°F). The boiler feedwater pumps (P-826) raise the BFW pressure to 900 psig (62 atm), requiring 540 kW (720 hp) of power. An amine injection system is specified to remove oxygen, which can pit the boiler surfaces. Other boiler chemicals include ammonia, added to control the pH and reduce the corrosive nature of the hot condensate, and phosphate, added to control the formation of scale in the steam drum. Boiler blowdown is 3% of steam production. The blowdown stream is flashed to atmospheric pressure; the vapor is vented to the air and the liquid is routed to wastewater treatment.

The turbogenerator (M-811) uses a multistage turbine with two extraction ports and a final condenser. Of the superheated steam leaving the boiler, 12% is extracted from the turbine at 175 psig (13 atm) and 268°C (514°F) for feeding to the pretreatment reactor and the BFW economizer. An additional 35% is extracted at 125 psig (9.5 atm) and 164°C (327°F) and is used in distillation and in the deaerator. The rest of the steam is condensed at -13 psig (0.1 atm). The condensate is pumped back to the boiler. The turbine shaft turns a generator to produce electricity. The generator efficiency is assumed to be 85%. For this design, a total of 41 MW of power is generated from the system. The process uses 28 MW, leaving about 13 MW to be sold to the grid.

3.8.3 Cost Estimation

Harris Group investigated the combined system of combustor, boiler, and turbogenerator. They contacted several vendors to obtain cost and operating information to identify a system suitable for the available fuel streams and steam requirements. The combustor/boiler quote ultimately came from Babcock & Wilcox and included the BFW preheater, FGD spray dryer, and baghouse. For the baghouse, bag replacement appears as a periodic charge in the cash flow worksheet.

The turbogenerator is essentially an off-the-shelf technology, and Harris Group obtained a quote for a 42.2 MW Siemens generator suitable for this project. Harris Group also obtained quotes from Proctor Sales for support equipment including the deaerator, chemical injection system, tanks, and pumps.

54
3.9 Area 900: Utilities

3.9.1 Overview

Area 900 is used to track the utilities required by the ethanol production facility (except for steam, which is provided by Area 800). Area 900 tracks cooling water, chilled water, plant and instrument air, process water, and the clean-in-place (CIP) system. Area 900 also tracks the electricity usage throughout the plant.

The process water manifold in Area 900 mixes fresh water with treated wastewater (assumed suitable for all plant users) and provides this water at a constant pressure to the facility. Water is provided to the cellulase production unit, boiler and cooling tower makeup, the CIP system, and the vent scrubber. Fresh water is also mixed with some internally-recycled water for dilution before pretreatment and enzymatic hydrolysis. The plant and instrument air systems provide compressed air for general use (pneumatic tools and clean-up) and instrument operation. Larger users of compressed air, namely the stillage filter press and cellulase system, have their own compressors specified. The CIP system provides hot cleaning and sterilization chemicals to hydrolysis and fermentation, the enzyme production section, and the distillation system. 

3.9.2 Design Basis

The cooling water system is designed for a 28°C supply temperature with a 9°C temperature rise in coolers throughout the facility. This is an assumed average rise; the actual cooling water rises across each exchanger are not explicitly modeled in Aspen. The primary cooling water users in this process are listed in Table 24. The percentage of cooling duty contributed by each user is shown in Figure 14.

Table 24. Cooling Water Users
M-811 Condenses the steam turbine exhaust at a vacuum.
M-908 The chilled-water loop requires cooling water to condense the refrigerant. The cooling water duty to M-908 is set equal to the total load on the chilled-water loop.
H-301 Cools the pretreated slurry to enzymatic hydrolysis temperature (48°C).
H-509 Cools the ethanol product leaving the molecular sieve before it enters storage.
F-300 Before fermentation is initiated, the slurry must be cooled to fermentation temperature.  It is assumed that cooling water would be used for the initial drop from 48°C to 35°C and that chilled water would afterward be substituted to sustain this temperature.
H-503 Provides cooling and condensation during regeneration of the molecular sieve.
M-401 Uses cooling water to cool the compressed air used in enzyme production.
H-504 Condenses the beer column reflux.
H-244 Condenses residual pretreatment flash vapor before it enters WWT. Most of the vapor is condensed by heat exchange with the incoming dilution water and boiler feed water.

55
Figure 14. Cooling duty distribution between major users
Condensing Turbine 52%
Chiller condenser 14%
Hydrolysis cooler 11%
Hydrolyzate flash condenser 8%
Pre-fermentation cooler 6%
EtOH product cooler 5%
Molsieve regeneration cooler 3%
Enzyme production compressor 1%
Beer column condenser 0%
DW1102A
Total Duty = 97 MMkcal/hr (386 MMBtu/hr)


By far the biggest user of cooling water is the condensing turbine. In contrast to the 2002 design, the cooling water duty required by the ethanol separation section is relatively small because an air-cooled condenser was specified for the rectification column. Aspen computes the cooling tower evaporation rate based on a temperature drop from 37°C to 28°C. It was assumed that windage would be 0.005% of the total flow to the tower. The tower blowdown was assumed to be 0.15% of the flow leaving the tower basin. 

Chilled water is provided by two 2,350-ton Trane centrifugal chillers. Per the chiller spec sheet, the compressor electricity demand for the chiller was estimated at 0.56 kW/ton of refrigeration. The cooling water demand for the chiller system was assumed to be equal to the heat removed in the chilled-water loop. The chilled-water loop provides cooling to the fermentors in Area 300 and Area 400.

Fresh water is assumed to enter the facility at 13°C and is used to cool the wastewater entering Area 600 to digestion temperature before entering the process water tank. The fresh water is mixed with the treated wastewater effluent in the process water tank (T-914) and then split several ways. Clean water must be provided to biomass dilution in the front end, to the cellulase production unit, to the vent scrubber, and to the boiler and cooling tower water makeup. The process water tank is designed for an 8-hour residence time. The process water pump (P-914) pumps water from the tank into the facility and is designed to handle 1.5x the process water flow requirement. In the present design, less water is recycled internally in the process than in the 2002 design. The only water stream directly recycled to the front end of the process is the rectification column bottoms.

56
The plant and instrument air systems provide compressed air for pneumatic tools and clean-up and instrument operation. The plant air compressor is sized for 400 SCFM at 125 psig. An instrument air dryer and surge tank were designed to provide clean dry air at a consistent pressure to the instrument air system. The surge tank was sized at 3,800 gal.

About 68% of the electricity generated by the boiler in Area 800 is used throughout the plant to power pumps, agitators, compressors, etc. The surplus is sold to the grid for credit. The distribution of total plant power utilization among all areas is shown in Figure 15. Note that the cost of the power required by Area 100 is already assumed to be included in the feedstock cost but must be subtracted from the plant’s electricity export. This is reflected in the economics by an operating cost credit equal to this amount of electricity.

Figure 15. Distribution of plant electricity utilization by process area
to A100 Feedstock Handling 2%
to A200 Pretreatment 14%
to A300 Hydrolysis & Fermentation 6%
to A400 Enzyme Production 13%
to A500 Recovery 5%
to A600 Wastewater 18%
to A700 Storage 0%
to A800 Boiler/Turbogen 3%
to A900 Utilities 8%
Excess electricity to grid 31%
DW1102A
Total Power Generated = 41 MW

3.9.3 Cost Estimation

The cooling tower was based on a cost estimate from Marley SPX for a fiberglass cooling tower capable of handling 44,000 gpm. Harris Group estimated costs for the cooling water circulation and makeup pumps using their internal database. The material of construction for the cooling water loop is carbon steel. The cost for the chiller came from a recent Trane quote for a similarly-sized system. Harris Group also used their internal database to estimate costs for the remaining equipment: the process water tank and pump; the plant/instrument air compressor, dryer, and surge tank; and the CIP system.

57
4 Process Economics

The ultimate purpose for developing such a detailed process design, simulation model, and cost estimate is to determine the economics of ethanol production. This information is used either as an absolute cost to assess ethanol’s potential in the marketplace or as a relative cost that can be used to guide research by examining the change in production cost associated with a process modification or other core research activity.

The total capital investment (TCI) is first computed from the total equipment cost. Next, variable and fixed operating costs are determined. With these costs, we use a discounted cash flow analysis to determine the minimum ethanol selling price (MESP) required to obtain a zero net present value (NPV) with a finite internal rate of return (IRR). This section describes the assumptions made in completing the discounted cash flow analysis.

Our analysis does not take into account any policy factors such as subsidies, mandates, or carbon credits because these would be purely speculative. The purpose of this analysis is to demonstrate whether or not cellulosic ethanol can be cost-competitive on its own merits and, if it cannot, to give policymakers a sense of the magnitude of incentive required to make it so. 

4.1 About Cost-Year Indices

The cost-year of 2007 was chosen for this analysis to align with DOE’s 2012 cellulosic ethanol  performance cost goals [27]. It is expected that these performance goals will remain in 2007 dollars (2007$) through 2017 to permit comparison of future feedstocks, conversion technologies, and cellulosic biofuels. However, the present equipment costs were obtained in 2009$ or 2010$ and cost-years for chemicals range from 1999 to 2010. The following is a brief discussion of the methods used for determining MESP in another year’s dollar value.

Each piece of equipment has a purchased cost that reflects a quote made in a certain year. Capital costs provided by Harris Group in 2009$ or 2010$ were adjusted using the Plant Cost Index from Chemical Engineering Magazine [69] to a common basis year of 2007. The final cost index for a given year is generally not made available until the spring of the following year. Therefore, for the small number of equipment items that were quoted in 2010$, we used the Plant Cost Index value from August of 2010. Similarly, for chemical costs we used the Industrial Inorganic Chemical Index from SRI Consulting [70]. Employee salaries were obtained in 2009$ and were scaled using the labor indices provided by the United States Department of Labor Bureau of Labor Statistics [71]. The general formula for year-dollar back-casting is:

2007 Cost = (Base Cost) (2007 Cost Index/Base Year Index)

The cost indices for capital and chemicals are not duplicated here; however, the reader is probably aware of the significant run-up in the price of raw materials such as steel and petroleum in the second half of the 2000s, beginning in 2003–2004. This inflation had dramatic effects on the prices of equipment and chemicals used in our design. Following a market correction, the Plant Cost Index crested in 2008, with the 2009 index actually being lower than the 2007 index. The Industrial Inorganic Chemical Index also crested in 2008 but the correction in 2009 was much smaller. In the year 2007 in particular, chemical prices varied wildly month-to-month and location-to-location, depending on the available supply. It should be noted, therefore, that the chemical costs used in this analysis are static back-projections based on these cost indices. While these costs are reported in 2007$, they do not necessarily reflect the actual market price of that chemical in 2007.

58
The electricity export price was taken to be the average wholesale price as determined by the North American Electric Reliability Corporation for a given year. The wholesale price applies to electricity that is credited back to the grid. These data are provided on the Energy Information Administration’s website [72]. For 2007, the wholesale electricity price was 5.71675 cents/kWh.

4.2 Total Capital Investment (TCI)

Section 3 of this report describes the details of the conceptual process design and how the purchased cost of the equipment was determined. The next step is to determine the installed cost of that equipment. The installation cost can be determined by performing a detailed study of everything required to install the necessary equipment and make it operational (e.g., foundation, piping, wiring). This type of detail is not warranted at this level of analysis, and a factored approach in which multipliers are applied to the purchased equipment cost is considered satisfactory. Many engineering texts such as Garrett [73] or Peters and Timmerhaus [74] detail such factored methodologies for common chemical processes. Indeed, there are as many methodologies for computing the total installed cost of capital equipment as there are textbooks on plant economics. The matter of which method is “correct” is of course open for debate; however, at this level of detail, each methodology is generally considered as good as the next.

The overarching cost methodology we have followed comes from the first biochemical design report prepared for NREL by Chem Systems in 1994 [75]. They provided installation factors for individual pieces of equipment, taken from Walas [76]. While simpler methods suggest a single multiplier be applied to the total purchased equipment cost, those methods tend to cite multipliers applicable for very large projects comprising mostly carbon steel equipment. For the relatively small plant described here, with mixed carbon and stainless steel equipment, the individual installation factor method makes more sense.

From the 1994 Chem Systems report, some of the installation factors were modified in the 1999 and 2002 design reports based on the experience of the engineers involved. Because the costs for the present design were all new, we chose to revert all installation factors back to the values specified by Walas. We found, however, that the Walas factors were in turn taken from the methodology of Cran [77], who deliberately excluded instrumentation costs from his installation factors so that these could be estimated separately. Although Cran details how to compute instrument costs, we decided to assume these would be 30% of the purchased equipment cost, consistent with the estimate in Peters and Timmerhaus [74], which we imposed by adding 0.3 to the Cran factors.

The list of installation factors for the various pieces of equipment is shown in Table 25. See Appendix A for a complete listing of the equipment, along with its purchased and installed costs. In contrast to the 2002 design, which had an equipment cost for every single item, Harris Group obtained many package quotes, in which a given unit operation and all of its support equipment were quoted under one price. The installation factor for such packages can be relatively low because most of the engineering is already included in the price. Additionally, equipment designed as a pre-fabricated skid generally has a lower construction cost. Also, components that are more highly machined and have higher-quality metallurgy tend to be more expensive per unit mass and therefore have a lower installation factor as a function of purchase price than a less sophisticated component does. A good example of all three of these considerations is the pretreatment reactor system.

59
Table 25. Installation Factors
Equipment Multipliera
Agitators, carbon steel 1.6
Agitators, stainless steel 1.5
Boiler 1.8
Compressors, motor driven 1.6
Cooling tower 1.5
Distillation columns, stainless steel 2.4
Heat exchangers, shell & tube, stainless steel 2.2
Heat exchangers, plate & frame, stainless steel 1.8
Heat exchangers, air-cooled 2.8
Inline mixers 1.0
Skidded equipment 1.8
Solids handling equipment (incl. filters) 1.7
Pressure vessels, carbon steel 3.1
Pressure vessels, stainless steel 2.0
Pretreatment reactor system 1.5
Pumps, stainless steel 2.3
Pumps, carbon steel 3.1
Tanks, field-erected, carbon steel 1.7
Tanks, field-erected, stainless steel 1.5
Tanks, storage, plastic 3.0
Tanks, storage, carbon steel 2.6
Tanks, storage, stainless steel 1.8
Turbogenerator 1.8

a Installed cost = (purchased equipment cost) x (multiplier).

The purchased cost for a given component reflects a baseline equipment size. As changes are made to the process, the equipment size required may be different than what was originally designed. Instead of re-costing in detail, an exponential scaling expression was used: 
New Cost =  (Base Cost)(New Size/Base Size)n

where n is a characteristic scaling exponent (typically in the range of 0.6 to 0.7) based upon some characteristic of the equipment related to production capacity, such as flow or heat duty. Such scaled costs are easier to calculate and generally give nearly the same result as resizing the equipment for each scenario. The scaling exponent can be inferred from vendor quotes if multiple quotes are given for different sizes, computed with costing software, or obtained from a standard reference [73–74, 76]. In our case, we returned to the exponents proposed in the 1994 Chem Systems report, which are shown in Table 26. Note that because the costs for most equipment items were newly estimated at their size in the present design, the exponents do not greatly affect the base MESP. They only factor into the calculation when changes are made in the process.

60
Table 26. Scaling Exponents
Equipment Exponent
Agitators 0.5
Compressors, motor driven 0.6
Distillation columns 0.6
Heat exchangers 0.7
Inline mixers 0.5
Package quotes / Skidded equipment 0.6
Pressure vessels 0.7
Pumps 0.8
Tanks, atmospheric 0.7
Solids handling equipment 0.8

Once the total equipment cost has been determined in the year of interest, we must add several other direct and indirect costs to determine the total capital investment (TCI). Site development and warehouse costs are based on the inside-battery-limits (ISBL) equipment costs (Areas 200, 300, 400, and 500) and are considered part of the total direct cost (TDC). Project contingency, field expenses, home-office engineering and construction activities, and other costs related to construction are computed relative to the TDC and give the fixed capital investment (FCI) when summed. The sum of FCI and the working capital for the project is the TCI. Table 27 summarizes these categories and additional factors. Harris Group reviewed the items and factors and determined that they were consistent with other projects the company has completed. Harris Group thought the “home office and construction” charge used in 2002 was possibly a bit high at 25%, so this was reduced to 20%. The project contingency was also changed from 3% to 10% of the TDC. Table 28 summarizes the total installed equipment cost and illustrates the application of factors in Table 27 to obtain the total capital investment (TCI).

61
Table 27. Additional Costs for Determining Total Capital Investment (TCI)
Item Description Amount
Additional direct costs
Warehouse On-site storage of equipment and supplies. 4.0% of the installed cost of ISBL equipment (A200,300,400,500)
Site development Includes fencing, curbing, parking lot, roads, well drainage, rail system, soil borings, and general paving. This factor allows for minimum site development assuming a clear site with no unusual problems such as right-of-way, difficult land clearing, or unusual environmental problems.
Additional piping To connect ISBL equipment to storage and utilities outside the battery limits. 4.5% of ISBL
Indirect costs
Prorateable costs This includes fringe benefits, burdens, and insurance of the construction contractor. 10% of total direct cost (TDC)
Field expenses Consumables, small tool and equipment rental, field services, temporary construction facilities, and field construction supervision. 10% of TDC
Home office and construction Engineering plus incidentals, purchasing, and construction. 20% of TDC
Project contingency Extra cash on hand for unforeseen issues during construction. 10% of TDC
Other costs Start-up and commissioning costs. Land, rights-of-way, permits, surveys, and fees. Piling, soil compaction/dewatering, unusual foundations. Sales, use, and other taxes. Freight, insurance in transit, and import duties on equipment, piping, steel, instrumentation, etc. Overtime pay during construction. Field insurance. Project team. Transportation equipment, bulk shipping containers, plant vehicles, etc. 10% of TDC

62
Table 28. Project Cost Worksheet Including Total Direct Costs and Total Capital Investment
Process Area Purchased Cost Installed Cost
Area 100: Feedstock handlinga $ 14,200,000 $ 24,200,000
Area 200: Pretreatment $ 19,900,000 $ 29,900,000
Area 200: Conditioning $ 1,500,000 $ 3,000,000
Area 300: Enzymatic hydrolysis and fermentation $ 18,500,000 $ 31,200,000
Area 400: Enzyme production $ 10,700,000 $ 18,300,000
Area 500: Recovery $ 11,100,000 $ 22,300,000
Area 600: Wastewater $ 49,300,000 $ 49,400,000
Area 700: Storage $ 2,800,000 $ 5,000,000
Area 800: Boiler $ 36,500,000 $ 66,000,000
Area 900: Utilities $ 4,000,000 $ 6,900,000
Totals (excl. Area 100) $ 154,500,000 $ 232,100,000
Warehouse 4.0% of ISBL $ 4,200,000
Site development 9.0% of ISBL $ 9,400,000
Additional piping 4.5% of ISBL $ 4,700,000
Total Direct Costs (TDC) $ 250,400,000
Prorateable expenses 10.0% of TDC $ 25,000,000
Field expenses 10.0% of TDC $ 25,000,000
Home office & construction fee 20.0% of TDC $ 50,100,000
Project contingency 10.0% of TDC $ 25,000,000
Other costs (start-up, permits, etc.) 10.0% of TDC $ 25,000,000
Total Indirect Costs $ 150,200,000
Fixed Capital Investment (FCI) $ 400,600,000
Land $ 1,800,000
Working capital 5.0% of FCI $ 20,000,000
Total Capital Investment (TCI) $ 422,500,000
Lang Factor (FCI/purchased equip cost)b 3.1
TCI per annual gallon $6.92/gal
2007 dollars
DW1102A
a Feedstock handling not included in this calculation.
b Area 600 not included in Lang Factor.

4.3 Variable Operating Costs

Variable operating costs, which include raw materials, waste handling charges, and by-product credits, are incurred only when the process is operating. Quantities of raw materials used and wastes produced were determined using the Aspen material balance. Table 29 documents the costs and sources of chemicals used in the process, and Table 30 summarizes the variable costs on a per-year and per-gallon-of-ethanol basis.


63
Table 29. Chemical Costs and Sources
Component Cost (2007$) Source
Feedstock (corn stover) $0.0224/lb MYPP, $58.50/dry ton @ 20% moisture [27]
Sulfuric acid, 93% $0.0399/lb Basic Chemical of Omaha via Harris Group
Ammonia $0.1993/lb Terra Industries via Harris Group
Corn steep liquor $0.0252/lb Corn Products via Harris Group
Diammonium phosphate $0.4385/lb Ronas Chemicals via Harris Group
Sorbitol $0.5005/lb Coast Southwest via Harris Group
Glucose $0.2579/lb USDA ERS [78]
SO2 $0.1378/lb SRI Chemical Economics Handbook (CEH)
Enzyme nutrients $0.3727/lb SRI CEH (See Table 20)
Caustic $0.0678/lb Brown and Caldwell WWT design [65]
Lime $0.0904/lb Harris Group
Boiler chemicals $2.2661/lb 2002 Design Report [2]
Cooling tower chemicals $1.3580/lb 2002 Design Report [2]
Fresh water $0.0001/lb Peters & Timmerhaus [74]
Table 30. Variable Operating Costs
Process
Area
Stream Description Usage
(kg/h)
Usage
(lb/h)
Cost
($/ton)
$/hour MM$/yr
(2007$)
Cent/Gal
Ethanol
(2007$)
Raw materials
N/A Feedstock (wet) 104,167 229,688 46.80 5,374.69 45.20 74.07
A200 Sulfuric acid, 93% 1,981 4,367 81.39 177.73 1.49 2.45
Ammonia 1,051 2,317 406.96 471.48 3.97 6.50
A300 Corn steep liquor 1,158 2,554 51.55 65.84 0.55 0.91
Diammonium phosphate 142 313 895.32 140.33 1.18 1.94
Sorbitol 44 98 1,021.93 49.96 0.42 0.69
A400 Glucose 2,418 5,332 526.52 1,403.60 11.80 19.34
Corn steep liquor 164 363 51.55 9.35 0.08 0.13
Ammonia 115 254 406.96 51.59 0.43 0.71
Host nutrients 67 149 745.30 55.34 0.47 0.76
Sulfur dioxide 16 36 275.70 4.99 0.04 0.07
A600 Caustic 2,252 4,966 135.65 336.83 2.83 4.64
A800 Boiler chems <1 1 4,532.17 1.23 0.01 0.02
FGD lime 895 1,973 180.87 178.42 1.50 2.46
A900 Cooling tower chems 2 5 2,716.10 7.14 0.06 0.10
Makeup water 147,140 324,443 0.23 38.11 0.32 0.53
Subtotal 8,328.49 70.36 115.30
Waste disposal
A800 Disposal of ash 5,725 12,623 28.86 182.15 1.53 2.51
Subtotal 182.15 1.53 2.51
By-products and credits
Grid electricity 12,797 kW $0.0572/kWh 731.57 6.15 10.08
Area 100 electricity 859 kW $0.0572/kWh 49.13 0.41 0.68
Subtotal 780.71 6.57 10.76
Total variable operating costs 7,779.08 65.33 107.76



64
4.4 Fixed Operating Costs

Fixed operating costs are generally incurred in full whether or not the plant is producing at full capacity. These costs include labor and various overhead items. Many of the assumptions on fixed operating costs follow the 2002 design report [2] and/or Peters and Timmerhaus [74]. 

Table 31 shows the recommended number of employees and associated salaries. The number of employees was estimated by considering the likely degree of automation for each area and adding a reasonable number of management and support employees. The total number of employees has been reduced from 77 in the 2002 design to 60. The major reason for the reduced labor requirement is the redesign of the feed handling area. In the present design, feedstock is received year-round according to uniform-format specifications and is unloaded with truck tippers, eliminating the need for yard employees and operators to perform milling and washing. Eight operators and two laboratory technicians were added to support the on-site enzyme section, but overall fewer employees were required. Excluding these 10 employees, 50 employees for the ethanol facility is also consistent with a 2008 LECG consulting report prepared for the Renewable Fuels Association [79]. Salaries were estimated by using commercially available salary estimators such as Salary.com as well as open positions posted on internet job sites. Because the model feedstock is corn stover, salaries were estimated for rural regions of the U.S. Midwest (Iowa, Missouri, etc.). These estimates may vary depending on location.

Table 31. Fixed Operating Costs
Position 2007
Salary
# Required
2007 Cost MM$/yr (2007$)
Cent/Gal Ethanol (2007$)
Labor and supervision
Plant manager 141,569 1 141,569
Plant engineer 67,414 2 134,828
Maintenance supervisor 54,894 1 54,894
Maintenance technician 38,522 12 462,266
Lab manager 53,931 1 53,931
Lab technician 38,522 2 77,044
Lab tech-enzyme 38,771 2 77,044
Shift supervisor 46,227 4 184,906
Shift operators 38,522 20 770,443
Shift oper-enzyme 38,771 8 308,177
Yard employees 26,966 4 107,862
Clerks and secretaries 34,670 3 104,010
Total salaries 2,500,000 2.48 4.06
Labor burden (90%) 2,200,000 2.23 3.65
Other overhead
Maintenance 3.0% of ISBL 3,200,000 3.14 5.15
Property insurance 0.7% of FCI 2,700,000 2.80 4.60
Total fixed operating costs 10.66 17.46

A 90% labor burden is applied to the salary total and covers items such as safety, general engineering, general plant maintenance, payroll overhead (including benefits), plant security, janitorial and similar services, phone, light, heat, and plant communications. The 90% estimate is the median of the general overhead range suggested in the 2008 PEP Yearbook produced by SRI Consulting [80].

65
Annual maintenance materials were estimated as 3% of the installed ISBL capital cost and property insurance and local property tax were estimated as 0.7% of the fixed capital investment, based on the 1994 Chem Systems report [75].

4.5 Discounted Cash Flow Analysis and the Minimum Selling Price of Ethanol

Once the total capital investment, variable operating costs, and fixed operating costs have been determined, a discounted cash flow rate of return (DCFROR) analysis can be used to determine the minimum selling price per gallon of ethanol produced. The discounted cash flow analysis is calculated by iterating the selling cost of ethanol until the net present value of the project is zero. This analysis requires that the discount rate, depreciation method, income tax rates, plant life, and construction start-up duration be specified. Because this plant is equity-financed, some assumptions about the loan terms are also required.

We stress that the financial assumptions detailed in this section are of course subject to uncertainty and are not intended to represent the final word in project management. For research and policy purposes, one must at some point decouple the cost of making ethanol from the cost of making money. These financial parameters serve merely as a reference point from which to examine other economic sensitivities.

Discount Rate

For this analysis, the discount rate (which is also the internal rate of return [IRR] in this analysis) was set to 10% and the plant lifetime was set to 30 years. The discount rate was also used in previous design reports and was based on the recommendation in Short et al. [81] on how to perform economic evaluations of renewable energy technologies for DOE. His view was that, “In the absence of statistical data on discount rates used by industrial, transportation and commercial investors for investments with risks similar to those of conservation and renewable energy investments, it is recommended that an after tax discount rate of 10%…be used.”

Equity Financing

For this analysis, it was assumed that the plant would be 40% equity financed. The terms of the loan were taken to be 8% interest for 10 years. The principal is taken out in stages over the 3-year construction period. Interest on the loan is paid during this period, but principal is not paid back. (This is another nth-plant assumption, which says that this cash flow comes from the parent company until the plant starts up.) This is all in contrast to the 2002 design, which assumed a 100% equity purchase. Figure 16 illustrates the sensitivity of minimum ethanol selling price to the percentage of equity financing and the after-tax discount rate (the IRR).

66
Figure 16. Sensitivity of MESP to IRR and % equity (8% interest on a 10-year loan)
$2.00
$2.20
$2.40
$2.60
$2.80
$3.00
$3.20
$3.40
$3.60
0% 20% 40% 60% 80% 100%
Minimum Ethanol Selling Price ($/gal)
Equity %
10% IRR
15% IRR
20% IRR
DW1102A


Depreciation

To determine the capital depreciation amount for the calculation of federal taxes to be paid we used the IRS Modified Accelerated Cost Recovery System (MACRS). Within the MACRS system is the General Depreciation System (GDS), which allows both the 200% and 150% declining balance (DB) methods of depreciation. This offers the shortest recovery period and the largest tax deductions. According to IRS publication 946 [82], a cellulosic ethanol plant would fall under Asset Class 49.5, “Waste Reduction and Resource Recovery Plants.” This class uses a 7-year recovery period, not including the steam plant equipment, which has a 20-year recovery period (Asset Class 49.13). IRS publication 946 contains a special provision for cellulosic biofuels plants that allows them to write off 50% of the capital investment in the first year. This was not implemented in our cost model because it does not ultimately affect the MESP. (Although the provision affects the cash flow in the first few years of the analysis, it does not change the year in which the plant goes into the black and must start paying taxes.)

Taxes

The federal corporate tax rate used in our analysis is 35%. Income tax is averaged over the plant life and that average is calculated on a per-gallon basis. The amount of income tax to be paid by a potential ethanol producer varies annually due to changes in the volume of product produced and the allowable depreciation deduction. In fact, no income tax is paid in the first eight years of operation because the depreciation and loan interest deductions are greater than the net income. State taxes are not considered, primarily because the location of the plant has not been determined and tax rates vary from state to state (from 0% to 12%).

Construction Time

The construction time is important to the cash flow analysis because no income is earned during construction, but huge sums of money are being expended. Perry and Green [83] indicate that small projects (less than $10 million investment) can be constructed in fewer than 18 months and that larger projects can take up to 42 months. An overview of petroleum refining economics indicates that large refineries (on the order of $1.5 billion investment) can be constructed in 24 months [84]. Certainly this ethanol process is much smaller than a petroleum refinery, so using a construction time of 24 months fits within these references, although an important difference between this type of facility and a refinery is the large number of field-erected vessels. These are constructed on-site and have a longer construction time than if the tanks were delivered finished. Table 32 summarizes the schedule for construction and the cash flow during that time. Twelve months are added before construction for planning and engineering.

67
Table 32. Construction Activities and Cash Flow
Project Start Month
Project End Month
Activity Description
% of Project Cost
0 12 Project plan and schedule established; conceptual and basic design engineering, permitting completed. Major equipment bid packages issued, engineering started on selected sub-packages, P&IDs complete, preliminary plant and equipment arrangements complete. 8%
12 24 All detailed engineering including foundations, structure, piping, electrical, site, etc. complete; all equipment and instrument components purchased and delivered; all site grading, drainage, sewers, rail, fire pond, foundation, and major structural installation complete; 80% of all major process equipment set (all except longest-lead items), all field fabricated tanks built, and the majority of piping and electrical materials procured. 60%
24 36 Complete process equipment setting, piping, and instrumentation installation complete; all electrical wiring complete; all building finishing and plumbing complete; all landscaping complete; precommissioning complete; and commissioning, start-up, and initial performance test complete. 32%
TOTAL 100%
Note: The above assumes no utility or process equipment orders placed prior to month seven. Expenditures based on typical 60 MMgal/yr grain-to-ethanol facility.

Start-Up Time

Perry and Green [83] indicate that for a moderately complex plant, start-up should be about 25% of the construction time, or 6 months in this case. Delta-T’s experience (described in the 2002 design report) with start-up indicated that a large grain-to-ethanol plant could be started up in less than 6 months. Considering that this design is for the nth operating plant, we assumed a start up time of 3 months. The start-up period is not completely wasted, however. We expect that an average of 50% production could be achieved during that period while incurring 75% of variable expenses and 100% of fixed expenses.

Working Capital

Peters and Timmerhaus [74] define working capital as money available to cover (1) raw materials and supplies in inventory, (2) finished product in storage, (3) accounts receivable, (4) cash on hand for monthly payments such as wages and maintenance supplies, (5) accounts payable, and (6) taxes payable. They indicate that working capital is usually 10%–20% of the fixed capital investment. This flow of money is required over the life of the plant, beginning in the start-up phase to make product that generates revenue to use in purchasing more materials and supplies. For this project, 10% would be about $40 million. On-site ethanol storage capacity is 7 days; assuming that the product can be made, shipped, and payment received in 30 days is conservative. One month’s raw materials, labor, maintenance, taxes, and overhead is $6.9 million. Therefore, a lower number seems reasonable. Garrett [73] suggests that using a fraction of the yearly operating cost, typically 10%–35%, is more relevant. When these percentages are used to calculate working capital, this results in a working capital range of $8 million–$28 million. We chose to use $20 million, or 5% of the fixed capital investment.

68
Table 33 summarizes the parameters used in the discounted cash flow analysis. Using these parameters, plus the cost information in Table 28, Table 30, and Table 31, the resulting minimum ethanol selling price of pure ethanol is $2.15/gal (2007$). Table 34 summarizes the yields and conversion costs for the present design. According to the methodology of Cran [77], the expected accuracy of the TCI analysis is +/- 25%. If we apply this uncertainty to the TCI, the impact on the cost of ethanol is +/-$0.24/gal. The complete discounted cash flow summary worksheet is shown in Appendix B. The MESP can be further broken down into the cost of each process area. Figure 17 illustrates the contribution to the overall cost by process area and capital, operations, and fixed costs. (The bar for feedstock + handling reflects the single feedstock cost of $58.50/dry U.S. ton delivered to pretreatment and has not been decomposed.) Table 33. Discounted Cash Flow Analysis Parameters
Plant life 30 years
Discount rate 10%
General plant depreciation 200% declining balance (DB)
General plant recovery period 7 years
Steam plant depreciation 150% DB
Steam plant recovery period 20 years
Federal tax rate 35%
Financing 40% equity
Loan terms 10-year loan at 8% APR
Construction period 3 years
First 12 months’ expenditures 8%
Next 12 months’ expenditures 60%
Last 12 months’ expenditures 32%
Working capital 5% of fixed capital investment
Start-up time 3 months
Revenues during start-up 50%
Variable costs incurred during start-up 75%
Fixed costs incurred during start-up 100%

69
Table 34. Summary of Yields, Rates, and Conversion Costs
Feedstock rate 2,205 dry U.S. ton/day
On-line time 8,410 h/yr
Ethanol yield 79.0 gal/dry U.S. ton feedstock
(76% theoretical based on feedstock carbohydrates)
Ethanol production rate 61.0 MMgal/yr
Total equipment cost $232MM
Total capital investment (TCI) $423MM
TCI per annual gallon $6.92/gal
Minimum Ethanol Selling Price $2.15/gal
Feedstock contribution $0.74/gal
Enzyme contribution $0.34/gal
Non-enzyme conversion contribution $1.07/gal

-$0.40 -$0.20 $0.00 $0.20 $0.40 $0.60 $0.80
Feedstock + Handling: 74.1¢
Pretreatment / Conditioning: 28.8¢
Enzymatic Hydrolysis and Fermentation: 20.2¢
Cellulase Enzyme: 33.8¢
Distillation and Solids Recovery: 12.1¢
Wastewater Treatment: 33.5¢
Storage: 2.3¢
Boiler/Turbogenerator: (Net) 4.3¢
Utilities: 6.3¢
Capital Recovery Charge Raw Materials & Waste Process Electricity
Grid Electricity Total Plant Electricity Fixed Costs
DW1102A
Figure 17. Cost contribution details from each process area (per gallon EtOH)

At the time of the 2002 design report, it was thought that the costs predicted then were probably too high for a company to start constructing a cellulosic ethanol plant based on undemonstrated technology. Today we are seeing several such biorefineries being planned or built at the pilot and commercial scale. The technoeconomic results reported here fall within the range claimed by these companies with respect to ethanol yield and TCI/gallon. The principal barrier to commercialization today is the current lack of access to capital for large, first-of-a-kind projects.

70
5 Analysis and Discussion

5.1 Carbon and Energy Balance

Overall material and energy balances were performed on the Aspen model. Table 35 shows the flow of carbon inputs and outputs. Closure on the carbon balance was 100.4%; small errors are due to the imperfect stoichiometry used to generate microbial cell mass in fermentation and wastewater treatment. As shown in the table, >96% of all carbon in the process enters in the biomass feed, with small amounts of additional carbon coming from glucose (for enzyme production) and fermentation nutrients like corn steep liquor. 

Of the carbon inputs to the process, 29% of carbon atoms leave as ethanol. Major exit points for the balance of carbon (accounting for 66%) are the combustor stack and scrubber vent. We expect the amount of carbon exiting in the combustion exhaust to be rather large because most by-products (lignin, etc.) of this process are burned to form CO2. The majority of the carbon exiting the scrubber vent is also in the form of CO2 from fermentation.

Table 35. Ethanol Plant Overall Carbon Balance
Stream Carbon Flow
(kmol/h)
% of Carbon
Flow
Carbon inlets
Stover feedstock 3,117 96.6%
Glucose 81 2.5%
Other 28 0.9%
Total 3,226 100.0%
Carbon outlets
Combustion exhaust 1,670 51.8%
Ethanol product 941 29.2%
Scrubber vent 471 14.6%
Ash 10 0.3%
WWT brine 4 0.1%
Aerobic lagoons 88 2.7%
Enzyme production vents 54 1.7%
Total 3,238 100.4%

Only the carbohydrate components of the biomass can be converted to ethanol by fermentation. Of the carbon in the feed stream, 1,857 kmol/h (59.6%) is carbohydrates (glucan, xylan, arabinan, mannan, galactan, and sucrose); converting all of this carbon to ethanol represents the theoretical yield. According to Table 35, 1,412 kmol/h of the feed stream carbon is actually converted by the ethanol pathway (ethanol in the product plus CO2 in the scrubber vent), so the actual yield is 76% of the theoretical yield. The same yield in the 2002 design was 80% of theoretical. Ours is slightly lower because we have not assumed conversion of the minor sugars galactose and mannose.

An energy balance was performed to compare the energy products from the process (ethanol and electricity) to the potential energy in the biomass feed. The potential energy for material streams used in this analysis has three contributions: 
1. A combustion energy, defined as the lower heating value (LHV) of the stream at a reference temperature of 25°C.

71
2. A sensible heat effect to account for deviations of a stream’s temperature from the reference temperature of 25°C. (This is computed by Aspen.)
3. A latent heat effect to account for major volatile components (e.g., water, ethanol, furfural) that are in a phase other than the reference phase.

The LHV is the energy released when a material is burned to form its combustion products, with water in the vapor phase. This is considered to be a more “true” heating value for transportation fuels, where the combustion water is generally not condensed to recover heat. On an LHV basis, any liquid water present in a material stream therefore reduces its combustion potential because heat must be expended to vaporize that water. Note that the sign convention in this basis follows the usual convention for heat of combustion: streams that can be burned (e.g., glucose or ethanol) have a negative potential energy. Streams that cannot be burned (e.g., water or sulfuric acid) have a positive potential energy.

A comparison of the major energy streams produced by the process to the combustion energy of the biomass feed is made in Table 36; a small discrepancy in the model’s energy balance closure is due to reasons cited above. The combined energy available from the ethanol product and the exported electricity is 48% of the energy content of the biomass feed. The energy losses from the cooling tower and combustion exhaust are fairly large. Ambient heat losses are also significant; these include the wastewater lagoons and the air-cooled condenser on the rectification column. Compared to the 2002 design, less energy is lost from the cooling tower and combustion exhaust but more is lost through these ambient mechanisms. Note that “electricity reserve” refers to the total power demand to a small number of intermittent users in the plant (e.g., conveyor belts). This reserved electricity is not available for export and must be accounted for separately.

Table 36. Ethanol Plant Overall Energy Balance
Stream Energy Flow (MMkcal/h)
Major energy inputs
Stover feedstock -316
Glucose -8
Sulfuric acid 1
Ammonia -4
Other chemicals 0
Well water 87
Total -239
Major energy outputs
Ethanol -139
Cooling tower evaporation -20
Combustion exhaust + ash -12
Ambient heat losses -63
Electricity export -11
Electricity reserve -4
WWT brine 8
Total -240

As with the carbon balance, the energy content of non-carbohydrate compounds cannot be converted to ethanol. The total energy content of the carbohydrate components in the feed is -192 MMkcal/h. In other words, only 61% of the feedstock’s combustion energy can be used to make ethanol. Given the energy content recovered as ethanol from Table 36, the percent of carbohydrate energy in the feed recovered as ethanol is about 72%, similar to the amount of carbohydrate carbon recovered as ethanol. A diagram of the overall mass, carbon, and energy balance is presented in Figure 18.
72

73
Figure 18. Mass, carbon, and energy balance diagram for the overall process
Pre
treatment
Chemicals
Biomass
Enzymatic
hydrolysis
Chemicals
Glucose
Enzyme
Production
Wastewater
treatment
Boiler/
Turbogenerator
-147 Recovery
Process and
Cooling water
Stack+Ash
Ethanol
Well water
Cooling twr
WWT Evap
Elec out
losses
Fermentation
Chemicals
Chemicals
Vent
Air
Chemicals
Air
Air
Air
Elec Rsrv
Brine
losses
losses
1,299 kg/hr
22 kmol C/hr
-2 Gcal/hr
3,031 kg/hr
0 kmol C/hr
-3 Gcal/hr
104,167 kg/hr
3,117 kmol C/hr
-316 Gcal/hr
12,105 kg/hr
2,845 kg/hr
81 kmol C/hr
-8 Gcal/hr
377 kg/hr
6 kmol C/hr
-1 Gcal/hr
32,853 kg/hr
223,602 kg/hr
4,504 kg/hr
0 kmol C/hr
2 Gcal/hr
895 kg/hr
0 kmol C/hr
0 Gcal/hr
284,495 kg/hr
147,140 kg/hr
0 kmol C/hr
87 Gcal/hr
817,045 kg/hr
3,226 kmol C/hr
-239 Gcal/hr
21,398 kg/hr
471 kmol C/hr
0 Gcal/hr
Vent
21,808 kg/hr
941 kmol C/hr
-139 Gcal/hr
-24 Gcal/hr
33,387 kg/hr
54 kmol C/hr
0 Gcal/hr
221,417 kg/hr
88 kmol C/hr
-1 Gcal/hr
9,929 kg/hr
4 kmol C/hr
8 Gcal/hr
-26 Gcal/hr
-11 Gcal/hr
-12 Gcal/hr
-4 Gcal/hr
371,750 kg/hr
1,680 kmol C/hr
-12 Gcal/hr
137,362 kg/hr
0 kmol C/hr
-20 Gcal/hr
817,052 kg/hr
3,238 kmol C/hr
-240 Gcal/hr
-111
17
4
80
86
7
-97
-66
216
-51
-3
-4 -39
-1
-3
-1
-6
101 Thin stillage
Lignin cake
Recycle water
Biogas
Recycle water
Dilution water
Dilution water
Dilution water
Cooling water
Material Heat Work Energy flows (Gcal/hr) shown on selected intermediate streams.
Positive energy flow has a negative sign.
Evaporation


74
5.2 Water Balance

Consumptive water usage in the biochemical conversion process is generally considered to be high compared with a thermochemical conversion process or even a petroleum-based fuel process, when viewed in terms of gallons of water used per gallon of fuel produced (gal/gal). Based on detailed water balances from the Aspen simulation, the consumptive water usage in the 2002 design was 6.3 gallons of water used per gallon of ethanol [2]. Using the older model as a guide, Harris Group adjusted some assumptions around the cooling tower for a modest reduction in water usage, but as the model was updated for the present report, these adjustments were ultimately canceled out by more accurate accounting of cooling water streams and inclusion of the on-site enzyme production area. Without additional process modifications, the new design’s consumptive water usage would therefore have been greater than in the 2002 design. In light of this, we gave more attention to water reduction and optimization.

As discussed in Section 3, the switch from lime to ammonia conditioning after pretreatment created a problem with ammonium sulfate and other inorganics accumulating in the evaporated stillage syrup. Boiler vendors were not comfortable quoting equipment to handle this stream, so we chose instead to handle the stillage in the wastewater treatment section. Doing so gave us the opportunity to remove the syrup evaporators, which in the 2002 design accounted for about one half of the cooling tower losses and one-third of the total water losses. (Although the evaporators returned clean water to the process in the 2002 design, they were a net water loser—the amount of water returned to the process was less than the amount of water lost from the cooling tower as a result of condensing the recycled water.) Furthermore, the evaporated stillage syrup, which was sent to the combustor in the 2002 design, contained about 50% water. This water came out of the ethanol conversion process but was then lost via the combustor stack. By routing the stillage to wastewater treatment, all of the water contained in the stillage becomes theoretically recyclable to the process. The stillage evaporators in the 2002 design also acted as the condenser for the rectification column. Simply removing the evaporators and using cooling water in the rectifier condenser would therefore not have resulted in a significant reduction in consumptive water usage. Instead, Harris Group proposed placing an air-cooled condenser on the rectification column. The capital cost was about the same—$487K for the air-cooled condenser versus $440K for the cooling-water condenser initially specified by Megtec. The air-cooled unit uses about 300 hp (225 kW) of electricity, but this extra demand is insignificant to the overall plant, which generates more than 40 MW of electricity.

Taken together, elimination of the stillage evaporators combined with addition of the air-cooled rectifier condenser and improved heat integration in the front end of the process led to a reduction in the consumptive water usage from 6.3 gal/gal in 2002 to 5.4 gal/gal in the present design report. The overall water balance is shown in Table 37—the “makeup water” line item indicates the consumptive water usage.

Additional water enters the process via the feedstock and raw chemicals, both as free water and as “potential” water, i.e., the combustion product of lignin and unconverted sugars. Water is also consumed in hydrolysis reactions, and these are accounted for as well. We note that describing water usage with the units of gallons of water per gallon of ethanol can be somewhat misleading, because this quantity obviously depends on ethanol yield, and the yield in the present design is about 12% lower than in the 2002 design (79.0 gal/ton versus 89.7 gal/ton). Based on the actual makeup water flow, the present design has reduced the 2002 water usage by about 20% (150,000 kg/h versus 187,000 kg/h) for a plant that has the same feedstock flow rate and produces its own enzyme.

75
Table 37. Ethanol Plant Water Balance
Inputs kg/h gal/gal Outputs kg/h gal/gal
Moisture in feedstock 20,833 0.76 Water in ethanol product 109 0.00
Water in glucose (Area 400) 427 0.02 Cooling tower evaporation 137,363 5.00
Water in raw chemicals 3,056 0.03 Stripped in enzyme aeration 774 0.03
Generated in enzyme prod. 1,291 0.02 Scrubber vent 522 0.02
Generated in fermentation 121 0.00 Destroyed in pretreatment 2,473 0.09
Generated in WWT 2,680 0.10 Destroyed in enzym. hydrolysis 2,631 0.10
Generated in combustor 23,869 0.87 WWT evaporation 4,350 0.16
Enzyme prod. air intake 638 0.02 WWT brine 4,967 0.18
Lignin cake dryer intake 237 0.01 Combustor stack 54,451 1.98
WWT lagoon aeration intake 4,379 0.16 Boiler blowdown vent 2,580 0.09
Combustor air intake 5,572 0.20
Makeup (consumptive) water 147,140 5.35
Sum of inputs 210,243 7.65 Sum of outputs 210,220 7.65

The ethanol conversion process itself is not a significant loser of water. Utilities are responsible for practically all water loss, with 90% of the net water loss due to cooling tower evaporation. Table 38 expresses the individual cooling water users (see Figure 14) in terms of their water loss responsibility in gal/gal.

Table 38. Individual Contributors to Cooling Water Evaporation
Cooling Water User MMkcal/h % of
duty
gal/gal
Condensing turbine 50.7 52.1% 2.60
Chiller condenser 13.4 13.8% 0.69
Pre-hydrolysis cooler 10.6 10.9% 0.54
Hydrolysate flash 7.3 7.5% 0.37
Pre-fermentation cooler 5.9 6.1% 0.30
Ethanol product cooler 5.2 5.3% 0.27
Molsieve regeneration cooler 2.6 2.6% 0.13
Enzyme air compressor 1.2 1.2% 0.06
Beer column condenser 0.5 0.5% 0.02
Total 97.4 100% 5.00

The largest cooling water user is the condensing turbine (M-811), which is responsible for 2.6 gal/gal of water loss. A condenser on the turbine allows the steam to discharge from M-811 at a vacuum (about 0.1 atm) for maximum conversion of compressive energy to electricity. With the condensing turbine in place, the process generates enough electricity to supply all users in the plant plus a significant surplus, which is assumed to be sold to the grid. It would be difficult to eliminate the condensing turbine in the present design because without it, the plant would only be able to burn enough of the lignin and biogas to meet the steam demand. This would result in a significant excess of fuel that would have to be landfilled or disposed of somehow, or incinerated at no value. The plant would also no longer make enough electricity to support all of its users and would have to purchase the balance from the grid. Note that grid electricity also has a water usage associated with it, which in a full life cycle assessment would have to be attributed to the ethanol plant. Given the turbogenerator electricity output, the consumptive water use associated with the condensing turbine can be expressed as 0.46 gal/kWh, which is roughly equivalent to the consumptive water use in coal-fired electricity plants [85]. 
 
76
The water-condensed chiller assumed here could potentially be replaced with an air-condensed system; however, these units do not have a very large capacity, so many parallel units would be required at a significant capital expense. The hydrolysate flash condenser and the pre-hydrolysis cooler could also potentially be replaced, but by inspection neither of them would break even with their water savings given the low cost of water used in the model.

The three low-temperature coolers in Table 38 (ethanol product cooler, pre-fermentation cooler, and molecular sieve regeneration cooler) account for another ~0.7 gal/gal of water loss, but these are not candidates for air-cooled heat exchangers because their outlet temperature is too low (32°–35°C). The other users below these in Table 38 either do not represent a significant cooling water duty or are likely to come skidded with cooling water hookups.

5.3 The Cost of Sugar

Sugars are an intermediate product in the formation of ethanol. Hemicellulose is hydrolyzed to form xylose, arabinose, galactose, and mannose in the pretreatment area. Cellulase enzyme hydrolyzes the cellulose into glucose. NREL has received feedback from the biofuels industry (mainly from non-ethanol producers) that knowing the production cost of sugar from  ignocellulosic biomass is important to them as it can help them compare feedstocks and pretreatment processes, at least to the extent that these things can be considered modular to their process. To that end, NREL maintains a process model for intermediate sugar production that reports a minimum sugar selling price (MSSP, $/lb) [86, 87]. It should be stressed that the sugar stream produced in this analysis is strictly “imaginary.” The purpose of this analysis is merely to separate the cost of producing sugars from the downstream costs of producing ethanol or other products.

In the sugar cost analysis, enzymatic hydrolysis is assumed to be carried out in a sterile way and nearly to completion so that a transferable sugar stream is produced. The sugar model basically follows the ethanol model through enzymatic hydrolysis. A lignin press with counter-current washing is added after hydrolysis to separate lignin and unreacted insoluble solids from the dilute mixed sugar stream. The combustion section is retained, and an electricity co-product credit is assumed for these solids. A wastewater cost is kept to account for treatment of the pretreatment flash vapor; however, given that the beer column stillage (the principle wastewater feed in the ethanol model) is not applicable in the sugar model, an on-site wastewater facility is no longer justified. Instead, an operating cost of $0.09/kg COD is applied for disposal of the wastewater material to off-site treatment. Fermentation, distillation, stillage treatment, and ethanol storage are completely removed from the sugar model. As in the ethanol process design, enzymatic hydrolysis is assumed to achieve 90% cellulose-to-glucose conversion. 

Mass balances and capital and operating costs were determined for the sugar process using the same DCFROR methodology described for the ethanol process in Section 4, and the minimum dilute sugar selling price was calculated to be 11.6 cents/lb (2007$); detailed economics for this case are shown in Figure 19. Table 39 shows the sugar stream composition. It is important to note that this value is not directly comparable to a traditional commodity sugar derived from corn or sugarcane, as the cellulosic sugar material contains a mixture of C6 and C5 sugars at a relatively dilute concentration (set by solids loading limitations in enzymatic hydrolysis) as well as other contaminants such as furfurals, inorganic salts, residual lignin, etc.

77
Table 39. Mixed Sugar Stream Composition
Component Transfer Concentration (g/L)
Upgraded Concentration (g/L)
Glucose 75.9 289.8
Xylose 42.1 160.8
Arabinose 5.1 19.6
Mannose 1.3 4.8
Galactose 3.0 11.5
Total sugars 127.4 486.6
Extractive organics 31.2 119.1
Solubilized lignin 1.7 6.4
HMF 0.9 3.6
Furfural 0.9 0.1
Ammonium sulfate 5.5 21.0
Ammonium acetate 4.1 15.8
Insoluble solids 0.3 1.1

Table 39 also presents a composition for an “upgraded” sugar stream. Given the dilute nature of the raw sugar stream at 127 g/L total sugars, the associated selling price of 11.6 cents/lb should be viewed more as a “transfer price” where the raw cellulosic sugar material is sold over the fence to a conversion process that can use dilute sugar. In order to present a sugar price that more closely resembles traditional commodity sugars, we also evaluated the cost of concentrating the material on-site. A triple-effect evaporator system was added to the model, with heat input specified to achieve 50% water in the syrup (less than 50% sugar given the additional components present). The heat for concentrating the sugar syrup was assumed to come from supplemental natural gas rather than from the residual lignin. The 2007 price for natural gas for industrial use was taken from the U.S. Energy Information Administration, at $7.68 per thousand cubic feet [88]. After considering the added cost of the evaporator and condenser equipment as well as the cost of natural gas, the minimum sugar selling price was calculated to be 14.3 cents/lb (2007$), associated with 487 g/L total sugars. This concentrated sugar still has non-sugar compounds that may require cleanup, at additional cost.


78
Figure 19. Economic summary for dilute sugar production
Minimum Sugar Selling Price $0.1158 /lb, Dilute sugars
Sugar Production (MMlb / Year) 910.4
Sugar Yield (lb / Dry U.S. Ton Feedstock) 1179
Feedstock Cost $/Dry U.S. Ton $58.5 (Includes handling)
Internal Rate of Return (After-Tax) 10%
Equity Percent of Total Investment 40%
Capital Costs
Pretreatment & Conditioning $33,000,000 Feedstock + Handling 4.963
Enzymatic Hydrolysis $19,600,000 Sulfuric Acid 0.164
On-Site Enzyme Production $18,300,000 Ammonia 0.483
Solids Recovery $7,300,000 Glucose (Enzyme Production) 1.296
Wastewater Treatment $0 Other Raw Materials 0.107
Storage $1,900,000 Waste Disposal 0.222
Boiler/Turbogenerator $66,000,000 Electricity -0.676
Utilities $6,900,000 Natural Gas (sugar concentration) 0.000
Total Installed Equipment Cost $152,900,000 Fixed Costs 0.979
Capital Depreciation 0.978
Added Costs $127,000,000 Average Income Tax 0.559
(% of TPI) 45% Average Return on Investment 2.505
Total Project Investment $279,900,000 Manufacturing Costs ($/yr)
Feedstock + Handling $45,200,000
Installed Equipment Cost/Annual lb $0.17 Sulfuric Acid $1,500,000
Total Project Investment/Annual lb $0.31 Ammonia $4,400,000
Glucose (Enzyme Production) $11,800,000
Loan Rate 8.0% Other Raw Matl. Costs $1,000,000
Term (years) 10 Waste Disposal $2,000,000
Capital Charge Factor 0.131 Electricity -$6,100,000
Natural Gas (sugar concentration) $0
Fixed Costs $8,900,000
Sugar Concentration (g/L) 127 Capital Depreciation $8,900,000
Energy Efficiency (LHV sugar/LHV feed) 50.8% Average Income Tax $5,100,000
Average Return on Investment $22,800,000
Excess Electricity (KWH/lb) 0.12
Plant Electricity Use (KWH/lb) 0.26
Plant Water Use (gal/lb) 0.4
Specific Operating Conditions
Enzyme Loading (mg/g cellulose) 20
Saccharification Time (days) 3.5
Manufacturing Costs (cents/lb sugar)
Sugar Production Process Engineering Analysis
Corn Stover Design Report Case: DW1102A
Dilute Acid Prehydrolysis with Enzymatic Saccharification
All Values in 2007$


79
5.4 Cost Sensitivity Analysis
Here we present a limited sensitivity analysis using the technoeconomic model presented in this report. More exhaustive sensitivity analyses are planned for future publication, including sensitivity to feedstock variability and an overarching Monte Carlo sensitivity analysis including conversion and economic assumptions.

A single-point sensitivity was performed on the Aspen model using the variables and limits shown in Table 40. The baseline for all variables was the 2012 performance target used in the design case described previously. Reasonable minima and maxima for each variable were chosen with a group of NREL researchers. Each variable was changed to its maximum and minimum value while all others were held constant. The sensitivities of MESP and ethanol yield to these parameters are displayed as tornado charts in Figure 20. These indicate that conversion parameters have the largest (and only) impacts on ethanol yield. Conversion parameters also factor heavily into MESP, along with parameters that affect capital and operating costs. The uncertainty in capital costs resulting from the factored approach we used (+/-25%) has the largest impact to MESP but is on the order of other key parameters. We note that this is an imperfect comparison because the TCI bar represents a true uncertainty while the other bars are more accurately called a risk, in the sense that they represent a range of results that we might expect to see in the pilot-scale demonstration runs. The magnitude of these bars is of course a function of the range we chose in Table 40. Conversion parameters have their own uncertainty due to the laboratory measurements involved. We plan to quantify the sensitivity of MESP to these uncertainties in a future paper.

Table 40. Assumptions Varied in the Sensitivity Analysis
Assumption Name Min Baseline Max
Pretreatment PT % solids 25% 30% 40%
PT acid loading (mg/g) 10 22.1 35
PT temperature °C 150 158 170
PT xylan to xylose 80% 90% 92%
PT xylan to furfural 3% 5% 8%
PT glucan to glucose 6% 9.9% 12%
Enz hydrolysis EH % solids 17.5% 20% 25%
EH cellulose to glucose 75% 90% 95%
EH enzyme loading mg/g 10 20 30
EH time (d) 2 3.5 5
Fermentation FERM contamination losses 0% 3% 6%
FERM xylose to ethanol 75% 85% 90%
FERM arabinose to ethanol 0% 85% 85%
FERM time (d) 1 1.5 3
Capital Total capital investment -25% - +25%


80
Figure 20. Single-point sensitivity tornado charts for (a) MESP and (b) ethanol yield
$(0.30) $(0.20) $(0.10) $- $0.10 $0.20 $0.30
PT xylan to furfural 3:5:8%
PT temperature 150:158:170C
PT % solids 40:30:25%
PT glucan to glucose 12:10:6%
FERM time 1:1.5:3 d
EH time 2:3.5:5 d
FERM arabinose to ethanol 85:85:0%
PT xylan to xylose 92:90:80%
FERM xylose to ethanol 90:85:75%
FERM contamination losses 0:3:6%
EH % solids 25:20:17.5%
PT acid loading 10:22:35 mg/g
EH cellulose to glucose 95:90:75%
EH enzyme loading 10:20:30 mg/g
TCI +/-25%
ΔMESP ($/gal)
Base case $2.15
(a)
-8.0 -6.0 -4.0 -2.0 0.0 2.0 4.0
EH time 2:3.5:5 d
FERM time 1:1.5:3 d
PT % solids 40:30:25%
PT xylan to furfural 3:5:8%
EH enzyme loading 10:20:30 mg/g
PT temperature 150:158:170C
PT acid loading 10:22:35 mg/g
EH % solids 25:20:17.5%
PT glucan to glucose 12:10:6%
FERM arabinose to ethanol 85:85:0%
PT xylan to xylose 92:90:80%
FERM xylose to ethanol 90:85:75%
FERM contamination losses 0:3:6%
EH cellulose to glucose 95:90:75%
ΔYield (gal/ton)
Base case 79.0 (b)


81
5.5 State of Technology Back-Casting

The annual State of Technology (SOT) assessment is an essential activity for biochemical conversion research at NREL. The state of technology process is complementary to the design report. Without reconfiguring the unit operations in the Aspen model, the projected conversions from the design report are replaced by present conversions that have been experimentally verified at the bench and/or pilot scale on process-relevant material. By comparing the SOT year-over-year, research advances can be quantified in terms of economic improvements in the overall process.

We understand that “State of Technology” is arguably a misnomer because no commercial cellulosic ethanol plants exist today. The aim of an SOT case for a given year is not to report a current commercial production cost for cellulosic ethanol, but to reflect NREL’s best estimate of ethanol production costs in a hypothetical nth plant using the current best slate of demonstrated technical capabilities. The SOT uses conversion performances that have been demonstrated experimentally, with a preference for data obtained in NREL’s ~1 ton/day pilot facility. Not all conversion parameters can be practically measured in the pilot plant, so the SOT cases contain both laboratory-scale data and pilot-scale data. There is of course some risk in assuming that bench-scale performance data is applicable at large scale.

Since its inception, the SOT analysis has been based on the technoeconomic model from the 2002 design report [2]. Feedstock costs and year-dollars were updated, and some minor process modifications were made, but the basic Aspen model stayed the same. Using the new Aspen model described in this report, we performed a back-casting of the 2007–2010 SOTs using their conversion results. Table 41 shows these back-cast cases and their related MESP values. Much of the research that went into demonstrating these cases was discussed in Sections 3.2 and 3.3. Also shown in Table 41 are the 2011 interim conversion targets.

82
Table 41. Back-Casted State of Technology Cases and Future Targets
2007
SOT
2008
SOT
2009
SOT
2010
SOT
2011 2012
Minimum Ethanol Selling Price ($/gal) $3.53 $3.46 $3.08 $2.67 $2.62 $2.15
Feedstock contribution $1.01 $0.94 $0.85 $0.72 $0.76 $0.74
Enzyme contribution $0.39 $0.38 $0.36 $0.36 $0.43 $0.34
Non-enzyme conversion contribution $2.14 $2.14 $1.87 $1.59 $1.43 $1.07
TCI/annual gallon $11.33 $11.32 $10.60 $10.15 $9.40 $6.92
Yield (gallon/dry ton) 69 70 76 75 78 79
Technical targets
Feedstock
Feedstock cost ($/dry ton) $69.60 $65.30 $62.05 $53.70 $59.60 $58.50
Pretreatment
Xylan to xylose (including enzymatic) 75% 75% 84% 85% 88% 90%
Xylan to degradation products 13% 11% 6% 8% 5% 5%
Hydrolysate solid-liquid separation Yes Yes Yes Yes Yes No
Xylose sugar loss 2% 2% 2% 2% 1% 1%
Glucose sugar loss 1% 1% 1% 1% 1% 0%
Enzymatic hydrolysis & fermentation
Enzyme loading (mg/g) 20 20 20 20 25 20
Combined sacch & ferm time (d) 7 7 7 5 5 5
Corn steep liquor loading (wt %) 1% 1% 1% 1% 0.6% 0.25%
Overall cellulose to ethanol 86% 86% 84% 86% 86% 86%
Xylose to ethanol 76% 80% 82% 79% 85% 85%
Arabinose to ethanol 0% 0% 51% 68% 80% 85%
Operating parameters
Pretreatment solids loading (wt %) 30% 30% 30% 30% 30% 30%
Pretreatment temperature (°C) 190 190 158 158 158 158
Acid loading (mg/g dry biomass) 38.0 30.0 24.5 22.1 22.1 22.1
Secondary oligomer hold step No Yes Yes Yes Yes Yes
Ammonia loading (g per L of liquor) 12.9 12.9 9.8 4.8 4.8 4.8
Conditioning mode Liquor Liquor Liquor Liquor Liquor Whole
slurry
Saccharification mode Washed
solids
Washed
solids
Washed
solids
Washed
solids
Whole
slurry
Whole
slurry
Enz. hydrolysis solids loading (wt %) 20% 20% 20% 17.5% 20% 20%
Reference Aspen model (DW-) 1102F 1102E 1102D 1102C 1102B 1102A
The enzyme costs in Table 41 were computed by the on-site enzyme model described in Section 3.4. The loadings were set for each case, and the model computed the amount of enzyme needed and its cost. No research advances were assumed in the enzyme production section, so in effect the unit cost of enzyme protein ($/kg) remained constant across all cases. The enzyme loading itself is flat at 20 mg enzyme protein/g cellulose from 2007–2010 and then increases to 25 mg/g in 2011. This reflects a change in process integration from washed-solids to whole-slurry enzymatic hydrolysis. The rationale for this change was that it will allow us to eliminate all solid-liquid separation steps in the process once a suitable whole-slurry hydrolysate conditioning process is found. To date, whole-slurry experiments have indicated that a higher enzyme loading is required to reach acceptable conversion yields of cellulose to glucose. Reducing this enzyme loading back to 20 mg/g is a research target for 2012.

83
6 Concluding Remarks

6.1 Summary

NREL analysts and process engineers made a significant effort in 2009–2010 to update the 2002 design report of Aden et al. [2] that described the biochemical conversion of lignocellulosic biomass (corn stover) to ethanol. The purpose of these design reports is to investigate the process design and economics of converting lignocellulosic biomass to ethanol at scale and at a profit. The end result of the analysis is an absolute selling price for ethanol that is based on reasonable process engineering and plant design assumptions. This information is used to predict the cost competitiveness and market penetration potential of cellulosic ethanol in comparison with petroleum-derived fuels and corn ethanol. The design report also helps NREL and DOE to direct their research by using it to examine the sensitivity of the selling price to process alternatives, equipment and operating cost reductions, and advances in conversion research. Proposed research and its anticipated results can be translated into a new design with new economics that can be compared with the benchmark case.

In updating the design report, NREL and Harris Group revisited all major assumptions of the 2002 and earlier design reports, questioning their validity and making adjustments or improvements where needed. This included taking advantage of new technologies and engineering practices. All equipment costs and major raw material costs were updated with new quotes obtained in 2009$ and 2010$.

Some of the notable conversion process changes from the 2002 design were the following:
* The corn stover feedstock composition used in the design was updated to reflect a composition with a carbohydrate profile closer to the mean observed in NREL studies.
* A highly detailed pretreatment reactor configuration was provided by Andritz, Inc. The specifications of the reactor were mutually agreed upon between Andritz, Harris Group, and NREL researchers.
* Ammonia conditioning of the pretreated biomass replaced the previous practice of overliming followed by gypsum precipitation. The ammonia process allows the hydrolysate to be conditioned as a whole slurry, eliminating a solid-liquid separation step. 
* The enzymatic hydrolysis and fermentation section was previously modeled as a continuous train but is now modeled as a batch system. Upstream of the batch reactors, a continuous high-solids enzymatic hydrolysis reactor was added.
* An on-site enzyme production section replaced the previous purchased-enzyme cost model. Cellulase enzyme is produced using a T. reesei analog on glucose substrate. The purpose of the enzyme production section was to improve transparency on the true cost of enzymes for cellulosic ethanol and not to make a judgment call as to whether enzymes should be made on-site or purchased from a distributor.
* The wastewater treatment section was completely redesigned in high detail to accurately model treatment of the elevated nitrogen and sulfur levels that resulted from the switch from overliming to ammonia conditioning.

84
The end result of the technoeconomic analysis was a predicted minimum ethanol selling price (MESP) of $2.15/gal (2007$). This reflects a $0.74/gal contribution from feedstock, a $0.34/gal contribution from enzymes, and a $1.07/gal contribution from the remainder of the conversion process.

6.2 Variance from the 2002 Design
In the original 2002 design report, which projected 2012 technology, the modeled 2012 MESP was $1.07/gal ethanol in 2000$ ($1.29/gal if directly converted to 2007$). Since then, the projected 2012 model has evolved to include inflation in capital and chemical costs, new feedstock costs from INL, elimination of feedstock handling and yard workers, and some key process changes, including the oligomer conversion step in pretreatment and the switch to mmonia conditioning. The most recently updated MESP target for 2012 was $1.49/gal ethanol in 2007$ [27]. The model used to compute this price was based on the 2008 State of Technology model [21], which in turn was based on the 2002 design model. Table 42 compares this previous model to the present design, with the costs broken down by process area (note that the totals may be appear to be off by a cent due to rounding).

Table 42. Comparison of the Previous Target Case and the Present Design (2007$/gal)
Model Comparison by Area 2012 Model Based
on 2008 SOT
New 2012 Model
(This Work)
Difference
Feedstock $0.57 $0.74 $0.17
Feed handling (included in
feedstock cost in current model) $0.01 $0.00 -$0.01
Pretreatment/conditioning $0.26 $0.29 $0.03
Saccharification and fermentation $0.12 $0.20 $0.08
Cellulase $0.12 $0.34 $0.22
Distillation and solids recovery $0.16 $0.12 -$0.04
Wastewater treatment $0.03 $0.34 $0.31
Storage $0.02 $0.02 $0.01
Boiler/turbogenerator (includes
electricity co-product credit) $0.16 $0.04 -$0.12
Utilities $0.06 $0.06 $0.01
TOTAL (MESP) $1.49 $2.15 $0.66

Because the MESP is expressed in $/gal, it depends of course on the overall ethanol yield, which in the present design is about 12% lower than in the older model. Overall, there was a $0.66/gal (44%) increase over the previous target of $1.49/gal. When broken down by process area, we see in Table 42 that the more notable changes in cost came from the enzyme section (due to a changein the way enzyme costs were determined, i.e., by on-site production instead of an assumed price per gallon of ethanol) and from the wastewater area (material that was previously burned is now being routed to wastewater). The individual contributors to the cost delta are expressed in a different way in Table 43. At $0.22 per gallon, the new enzyme cost model is the largest contributor to the MESP difference between the two models. Another $0.08 can be attributed to the lower yield from the new feedstock composition, and $0.10 to an increase in the feedstock cost. A total of $0.21 can be attributed to net increases in the capital equipment costs, chemical costs, and labor rates.

85
Table 43. Individual Contributors to the Change in MESP
Contributor Amount
(2007$/gal)
Explanation
Feedstock cost $0.10 From $50.90 to $58.50 (new grower payment assumption)
Feedstock composition $0.08 Lower yield from more representative feedstock composition
Cellulase $0.22 On-site production model predicted $0.34/gal versus the
previous $0.12/gal purchased model
Electricity credit -$0.07 Larger fraction of biomass is converted to electricity with the
updated composition
Capital $0.30 Net increase in the capital equipment required
Financial assumptions -$0.06 100% equity versus 40% equity with 8% interest
Chemicals $0.06 New chemical costs
Fixed costs $0.03 New labor costs
$0.66

6.3 Future Work

The overarching near-term goal for DOE’s Office of the Biomass Program is to demonstrate the cost-competitiveness of cellulosic ethanol with petroleum fuels by 2012. NREL and DOE have agreed on a slate of conversion parameters that are likely achievable by 2012. These development targets lead to an nth-plant MESP of $2.15/gal by 2012, as modeled by the process design described in this report. One of NREL’s main tasks is to perform integrated pilot-scale testing that demonstrates these conversion targets in 2012. The pilot-scale tests will make use of NREL’s biochemical process integration expertise and other core conversion research occurring at smaller scales.

Pretreatment research will continue to focus on increasing xylan-to-xylose conversion, both by optimizing the conditions between the first step of pretreatment and the secondary oligomer conversion step and by supplementing enzymatic hydrolysis with accessory xylanase enzymes. Enzymatic hydrolysis research will have a significant focus on integrated experiments and on optimizing conditions using the newest pretreated material with the highest xylose conversion. Another focus in the pretreatment and enzymatic hydrolysis areas will be to reduce chemical usage and severity in pretreatment while maintaining good enzyme digestibility of the pretreated biomass. These experiments must be performed in an integrated way with fermentation. Also, some of the results described in this design report use an advanced research enzyme preparation. It is likely we will continue to experiment with more advanced preparations in 2011 and beyond.

In fermentation research, some of the advanced strains being developed by the awardees of DOE’s ethanologen strain solicitation are slated to be tested in NREL’s pilot plant. There is also a significant internal effort to genetically engineer the NREL Z. mobilis strain with a metabolic pathway to convert arabinose to ethanol. This is a risk mitigation strategy should the solicitation strains prove difficult to integrate into NREL’s pilot-scale ethanol process.

Process integration research will continue to focus on cost reduction through process design. Obtaining a pretreatment, conditioning, and enzymatic hydrolysis process that can be carried out as a whole slurry, without a solid-liquid separation step, is key to future cost reductions and will be studied aggressively. Other areas where process integration research plays a role is in reducing costs of fermentation media and mitigating the problems in back-end cleanup and wastewater treatment discussed in this report. These areas of the process will receive much more scrutiny between now and 2012.

86
In technoeconomic analysis research, we have plans to perform an extensive Monte Carlo cost sensitivity analysis using the new design report process described here. The analysis will examine the sensitivity to economic parameters such as raw material and equipment costs, to the expected compositional variability of corn stover, and to the specific process parameters defined in Aspen, such as fermentation conversions. There is also an interest in updating the Aspen model to handle alternate feedstocks: switchgrass, sorghum, wheat straw, sugarcane bagasse, etc. Each feedstock may require key process changes to overcome biomass recalcitrance or a thermal deficit. Once we have determined the similarities and difference between feedstocks, the goal is to produce a single, flexible model that can handle them all.

In addition to alternate feedstocks, this work is applicable to further technoeconomic analysis of advanced biofuels. The cellulosic ethanol process described here is only one of many pathways by which a transportation fuel can be produced from biomass. In the future, advanced conversion technologies that produce infrastructure-compatible or “drop-in” fuels (primarily gasoline, diesel, and/or jet-range hydrocarbons) will have an increasing importance in NREL’s and DOE’s research portfolio. Figure 21 shows some example pathways that yield such fuels from sugar; most of these technologies are already being researched by startup companies and academic institutions using clean sugar from corn or sugar cane. NREL plans to leverage its expertise in sugar generation from lignocellulosic material to help move these technologies away from food based sugars and toward sustainable biomass.

Figure 21. Sugar-based pathways for conventional and advanced biofuels

In a technoeconomic model of an advanced conversion process using cellulosic sugar, the front end of the Aspen model described in this report would largely stay the same through pretreatment and enzymatic hydrolysis, up to the production of a sugar intermediate. The sugar conversion and product recovery sections would be replaced with new sections that describe the technologies in Figure 21. Our process models for sugar production and the specialized wastewater and utilities sections should therefore be considered modular to these future studies.

87
References
NREL milestone reports cited below cannot be accessed outside of NREL and DOE. Readers may contact the authors of the specific reference to determine if this information has been made public since publication of this design report.
1. Wooley, R.; Ruth, M.; Sheehan, J.; Ibsen, K. Lignocellulosic Biomass to Ethanol Process Design and Economics Utilizing Co-Current Dilute Acid Prehydrolysis and Enzymatic Hydrolysis: Current and Future Scenarios. Report No. NREL/TP-580-26157. Golden, CO: National Renewable Energy Laboratory, July 1999. http://www.nrel.gov/docs/fy99osti/26157.pdf.
2. Aden, A.; Ruth, M.; Ibsen, K.; Jechura, J.; Neeves, K.; Sheehan, J.; Wallace, B.; Montague, L.; Slayton, A.; Lukas, J. Lignocellulosic Biomass to Ethanol Process Design and Economics Utilizing Co-Current Dilute Acid Prehydrolysis and Enzymatic Hydrolysis for Corn Stover. Report No. NREL/TP-510-32438. Golden, CO: National Renewable Energy Laboratory, June 2002. http://www.nrel.gov/docs/fy02osti/32438.pdf. 
3. “Aspen Plus.” Burlington, MA: Aspen Technology. http://www.aspentech.com/products/aspen-plus.cfm.
4. Tao, L.; Aden, A. “The Economics of Current and Future Biofuels.” In Vitro Cell Dev. Biol.; Vol. 45, 2009; pp. 199-217.
5. F.O. Lichts. Ethanol Production Costs: A Worldwide Survey. Turnbridge Wells, Kent, UK: Agra Informa, 2007.
6. Kwiatkowski, J.R.; McAloon, A.J.; Taylor, F. “Modeling the Process and Costs of Fuel Ethanol Production by the Corn Dry-Grind Process.” Ind. Crops Prod.; Vol. 233, 2006; pp. 288-296.
7. Rodrigues, A.P. Participação dos fornecedores de cana na cadeia do açúcar e álcool. Congresso Internacional de Tecnologias na Cadeia Produtiva, Concana Uberaba, MG, março de, 2007 (in Portuguese).
8. Seabra, J.E.A. Technical-Economic Evaluation of Options for Whole Use of Sugar Cane Biomass in Brazil. Ph.D. Thesis. Campinas Faculdade de Engenharia Mecânica Universidade Estadual de Campinas, 2007 (in Portuguese).
9. Graboski, M.S.; McCormick, R.L. “Combustion of Fat and Vegetable Oil Derived Fuels in Diesel Engines.” Prog. Energy Combust. Sci.; Vol. 24, 1998; pp. 125–164.
10. Haas, M.J.; McAloon, A.J.; Yee, W.C.; Foglia, A.T. “A Process Model to Estimate Biodiesel Production Cost.” Biores. Technol.; Vol. 97, 2006; pp. 671–678.
11. Laser, M.; Larson, E.; Dale, B.; Wang, M.; Greene, N.; Lynd, L.R. “Comparative Analysis of Efficiency, Environmental Impact, and Process Economics for Mature Biomass Refining Scenarios.” Biofuels, Bioproducts, & Biorefining; Vol. 3, 2009; pp. 247-270.

88
12. Kazi, F.K.; Fortman, J.A.; Anex, R.P.; Hsu, D.D.; Aden, A.; Dutta, A.; Kothandaraman, G. “Techno-Economic Comparison of Process Technologies for Biochemical Ethanol Production from Corn Stover.” Fuel; Vol. 89, 2010; pp. S20-S28. 
13. Klein-Marcuschamer, D.; Oleskowicz-Popiel, P.; Simmons, B.A.; Blanch, H.W. “Technoeconomic Analysis of Biofuels: A Wiki-Based Platform for Lignocellulosic Biorefineries.” Biomass and Bioenergy; Vol. 34, 2010; pp. 1914-1921.
14. Klein-Marcuschamer, D.; Oleskowicz-Popiel, P.; Simmons, B.A.; Blanch, H.W. “JBEI Corn Stover to Ethanol Model.” U.S. Department of Energy Joint BioEnergy Institute Wiki, http://econ.jbei.org/wiki/index.php/Corn_Stover_to_Ethanol_Model.
15. Huang, H.J.; Ramaswamy, S.; Al-Dajani, W.; Tschirner, U.; Cairncross, R.A. “Effect of Biomass Species and Plant Size on Cellulosic Ethanol: A Comparative Process and Economic Analysis.” Biomass and Bioenergy; Vol. 33, 2009; pp. 234-246.
16. Sendich, E.N.; Laser, M.; Kim, S.; Alizadeh, H.; Laureano-Perez, L.; Dale, B.; Lynd, L. “Recent Process Improvements for the Ammonia Fiber Expansion (AFEX) Process and Resulting Reductions in Minimum Ethanol Selling Price.” Bioresource Technology; Vol. 99, 2008; pp. 8429-8435.
17. Gnansounou, E.; Dauriat, A. “Techno-Economic Analysis of Lignocellulosic Ethanol: A Review.” Bioresource Technology; Vol. 101, 2010; pp. 4980-4991.
18. Bals, B.; Wedding, C.; Balan, V.; Sendich, E.; Dale, B. “Evaluating the Impact of Ammonia Fiber Expansion (AFEX) Pretreatment Conditions on the Cost of Ethanol Production.” Bioresource Technology; Vol. 102, 2011; pp. 1277-1283.
19. Piccolo, C.; Bezzo, F. “A Techno-Economic Comparison Between Two Technologies for Bioethanol Production from Lignocellulose.” Biomass and Bioenergy; Vol. 33, 2009; pp. 478-491.
20. National Academy of Sciences. Liquid Transportation Fuels from Coal and Biomass: Technological Status, Costs, and Environmental Impacts. Washington, DC: The National Academies Press, 2009. http://www.nap.edu/catalog/12620.html.
21. Humbird, D.; Aden, A. Biochemical Production of Ethanol from Corn Stover: 2008 State of Technology Model. Report No. NREL/TP-510-46214. Golden, CO: National Renewable Energy Laboratory, July 2009. http://www.nrel.gov/docs/fy09osti/46214.pdf.
22. Wooley, R; Putsche, V. Development of an ASPEN PLUS Physical Property Database for Biofuels Components. Report No. NREL/MP-425-20685. Golden, CO: National Rnewable Energy Laboratory, April 1996. http://biodev.nrel.gov/pdfs/3955.pdf.

89
23. Wooley, R.; Ibsen, K.; Putsche, V. Development of an ASPEN PLUS Physical Property Database for Biofuels Components. NREL Technical Memo, Document #4141. Golden, CO: National Renewable Energy Laboratory, 1999. http://biodev.nrel.gov/bcfcdoc/4141.pdf.
24. Hess, J.R.; Kenney, K.L.; Ovard, L.P.; Searcy, E.M.; Wright, C.T. Uniform-Format Solid Feedstock Supply System: A Commodity-Scale Design to Produce an Infrastructure Compatible Bulk Solid from Lignocellulosic Biomass, Section 3: Pioneer Uniform Feedstock Supply System. Report No. INL/EXT-08-14752. Idaho Falls, ID: Idaho National Laboratory, 2009. http://www.inl.gov/bioenergy/uniform-feedstock.
25. Templeton, D.W.; Sluiter, A.D.; Hayward, T.K.; Hames, B.R.; Thomas, S.R. “Assessing Corn Stover Composition and Sources of Variability via NIRS.” Cellulose; Vol. 16, 2009; pp. 621-639.
26. Corn stover analysis, sample 33A14 from Kramer Farm, Wray Pioneer Lot. Huffman Report #123409. Wray, CO: Kramer Farm.
27. Office of the Biomass Program, Energy Efficiency and Renewable Energy, U.S. Department of Energy. Multi-Year Program Plan. Washington, DC: U.S. Department of Energy, April 2011. http://www1.eere.energy.gov/biomass/pdfs/mypp_april_2011.pdf.
28. Chen, S.F.; Mowery, R.A.; Scarlata, C.J.; Chambliss, C.K. “Compositional Analysis of Water-Soluble Materials in Corn Stover.” J. Agric. Food Chem.; Vol. 55, 2007; pp. 5912- 5918.
29. Bower, S.; Wickramasinghe, R.; Nagle, N.J.; Schell, D.J. “Modeling Sucrose Hydrolysis in Dilute Sulfuric Acid Solutions at Pretreatment Conditions for Lignocellulosic Biomass.” Biores. Technol.; Vol. 99, 2008; pp. 7354-7362.
30. Ethanol (data page). Wikipedia, http://en.wikipedia.org/wiki/Ethanol_%28data_page%29.
31. Nagle, N.; Weiss, N.; Kuhn, E.; Tucker, M.; Sievers, D.; Elander, R. Validate > 75% Xylan Yield and <8% Degradation from Whole Corn Stover using a High Solids Continuous Pretreatment Reactor. D Milestone Report, Document #10341. Golden, CO: National Renewable Energy Laboratory, 2008. http://biodev.nrel.gov/bcfcdoc/10341.pdf.
32. Jennings, E.; Mohagheghi, A.; Schell, D.; Dowe, N. Technical and Economic Performance of an Ammonium Hydroxide-Based Conditioning Technology. E Milestone Report, Document #10379. Golden, CO: National Renewable Energy Laboratory, November 2008. http://biodev.nrel.gov/bcfcdoc/10379.pdf. 
33. Jechura, J. Correlation of Metal Corrosion Data. NREL Technical Memo, Document #5194. Golden, CO: National Renewable Energy Laboratory, March 2001. http://biodev.nrel.gov/bcfcdoc/5194.pdf.

90
34. Humbird, D. FY 2009 State of Technology Update—Biochem. D Milestone, Document #10590. Golden, CO: National Renewable Energy Laboratory, October 2009. http://biodev.nrel.gov/bcfcdoc/10590.pdf.
35. Humbird, D. FY 2010 Biochemical Platform State of Technology Update. D Milestone, Document #10752. Golden, CO: National Renewable Energy Laboratory, September 2010. http://biodev.nrel.gov/bcfcdoc/10752.pdf.
36. Weiss, N.; Nagle, N.; Elander, R.; Tucker, M. Achieve 75% Xylose Yield in Laboratory Scale High Solids Pretreatment Reactor on Corn Stem Internode. D Milestone Report, Document #9926. Golden, CO: National Renewable Energy Laboratory, 2007. http://biodev.nrel.gov/bcfcdoc/9926.pdf.
37. Sievers, D.; Kuhn, E.; Nagle, N.; Tucker, M.; Weiss, N. Implement Equipment Modifications to the Existing Horizontal Pretreatment Reactor System to Allow for Operation with a Tighter Residence Time Distribution. D Milestone Report, Document #10404. Golden, CO: National Renewable Energy Laboratory, December 2008. http://biodev.nrel.gov/bcfcdoc/10404.pdf.
38. Nagle, N.; Kuhn, E.; Sievers, D.; Tucker, M.; Weiss, N.; Elander, R. Parametric Study using the Continuous Horizontal Pretreatment Reactor using Corn Stover to Determine Operating Conditions that Achieve 80% Yield of Monomeric Xylose. D Milestone Report, Document #10575 Golden, CO: National Renewable Energy Laboratory, September 2009. http://biodev.nrel.gov/bcfcdoc/10575.pdf.
39. Nagle, N.; Kuhn, E.; Elander, R. Parametric Study Using the Modified Continuous Horizontal Pretreatment Reactor Using Corn Stover to Determine Operating Conditions that Can Achieve Yields of ≥ 85% of Monomeric Xylose. NREL D Milestone Report, Document #10764 Golden, CO: National Renewable Energy Laboratory, September 2010. http://biodev.nrel.gov/bcfcdoc/10764.pdf.
40. Selig, M; Decker, S. Enzymatic Conversion of Oligosaccharides from Various Pretreatment Hydrolysates. Joule Milestone Report, Document #10114. Golden, CO: National Renewable Energy Laboratory, March 2008. http://biodev.nrel.gov/bcfcdoc/10114.pdf.
41. Humbird, D.; Elander, R. Develop Process Engineering Scenarios for Potential Leading Pretreatment/Enzymatic Hydrolysis Configurations. E Milestone Report, Document #10582. Golden, CO: National Renewable Energy Laboratory, September 2009. http://biodev.nrel.gov/bcfcdoc/10582.pdf.
42. Zhang, M.; Eddy, C.; Deanda, K.; Finkelstein, M.; Picataggio, S. “Metabolic Engineering of a Pentose Metabolism Pathway in Zymomonas mobilis.” Science; Vol. 267, 1995; pp. 240-243.
43. Miroslav, S; Ho, N. “Production of ethanol from cellulosic biomass hydrolysates using genetically engineered saccharomyces yeast capable of cofermenting glucose and xylose,” Applied Biochemistry and Biotechnology; Vol. 144, 2004; pp. 403-416.

91
44. “Integrated Biorefinery Research Facility.” National Renewable Energy Laboratory website, http://www.nrel.gov/biomass/integrated_biorefinery_research_facility.html.
45. Humbird, D.; Mohagheghi, A.; Dowe, N.; Schell, D. “Economic Impact of Total Solids Loading on Enzymatic Hydrolysis of Dilute-Acid Pretreated Corn Stover.” Biotechnology Progress; Vol. 26, 2010; pp.1245-1251.
46. Loos, H.; Kramer, R.; Sahm, H.; Sprenger, G. “Sorbitol Promotes Growth of Zymomonas mobilis in Environments with High Concentrations of Sugar: Evidence for a Physiological Function of Glucose-Fructose Oxidoreductase in Osmoprotection.” J. Bact.; Vol. 179, 1994; pp. 7688-7693.
47. Dowe, N.; Humbird, D.; Schell, D. Status Report on Overall Corn Stover to Ethanol Yield Improvement Effort. Joule Milestone, Document #10457. Golden, CO: National Renewable Energy Laboratory, March 2009. http://biodev.nrel.gov/bcfcdoc/10457.pdf.
48. Franden, M.A.; Zhang, M. Characterize Hydrolyzate Toxicity Across a Variety of Hydrolyzates Obtained from the Horizontal Pretreatment Reactor and Other Selected Process Relevant Hydrolyzates Using both Biological and Chemical Analysis. D Milestone, Document #10585. Golden, CO: National Renewable Energy Laboratory, September 2009. http://biodev.nrel.gov/bcfcdoc/10585.pdf.
49. “Enzyme Systems Solicitation.” Financial Opportunities: Past Solicitations. Washington, DC: U.S. Department of Energy, Energy Efficiency and Renewable Energy website, 2008. http://www1.eere.energy.gov/biomass/past_solicitations.html#Enzymes.
50. “Ethanologen Projects—Development of Fermentative Microorganisms.” Financial Opportunities: Past Solicitations. Washington, DC: U.S. Department of Energy, Energy Efficiency and Renewable Energy website, 2007. http://www1.eere.energy.gov/biomass/past_solicitations.html#Ethanologen_Projects.
51. Schell, D.; Humbird, D.; Wolfrum, E.; Zhang, M. Research Plan for Demonstrating the 2012 Cost Target. E Milestone, Document #10458. Golden, CO: National Renewable Energy Laboratory, March 2009. http://biodev.nrel.gov/bcfcdoc/10458.pdf. 
52. “Ethanol Co-Products.” Ethanol Information website, http://ethanol information.com/ethanol-coproducts.php.
53. Meerman, H.J.; Kelley, A.S.; Ward, M. “Advances in Protein Expression in Filamentous Fungi,” Chapter 7. Baneyx, F., ed. Protein Expression Technologies: Current Status and Future Trends. Norfolk, UK: Horizon Bioscience, 2004; p 345.
54. Warzywoda, M., et al., U.S. Patent No. 4,762,788, 28 November 1984.
55. Emme, B., Novozymes, Inc., personal communication with David Humbird, 2009.
56. Atkinson, B.; Mavituna, F. Biochemical Engineering and Biotechnology Handbook. New York: The Nature Press, 1983.

92
57. Wang, D.; Cooney, C.; Demain, A.; Dunnill, P.; Humphrey, A.; Lilly, M. Fermentation and Enzyme Technology. New York: John Wiley & Sons, 1979.
58. Schell, D.; Riley, C.; Bergeron, P.; Walter, P. Technical and Economic Analysis of an Enzymatic Hydrolysis Based Ethanol Plant – Draft. SERI Technical Report TP-232- 4295. Golden, CO: Solar Energy Research Institute, 1991. http://biodev.nrel.gov/bcfcdoc/3892.pdf.
59. Jechura, J. Sugar Platform Post Enzyme Subcontract Case. Technical Memo, Document #9382 Golden, CO: National Renewable Energy Laboratory, October 2005. http://biodev.nrel.gov/bcfcdoc/9382.pdf.
60. Merino, S.T.; Cherry, J. “Progress and Challenges in Enzyme Development for Biomass Utilization.” Adv. Biochem. Engin./Biotechnol.; Vol. 108, 2007; pp. 95-120.
61. Dean, D.; Dodge, T.; Valle, F.; Chotani, G. “Development of biorefineries—technical and economic considerations.” Kamm, B. et al., ed. Biorefineries—industrial processes and products. Status quo and future directions. Vol. 1, Weinheim, Germany: Wiley VCH, 2006; pp. 67–83.
62. “New Enzymes Turn Waste into Fuel.” Press release. Novozymes, Inc., February 15, 2010. http://novozymes.com/en/news/news-archive/Pages/45713.aspx.
63. “Genencor Introduces Accellerase DUET.” Press release. Genencor, February 15, 2010. http://www.genencor.com/wps/wcm/connect/genencor/genencor/media_relations/news/archive/2010/pressrelease_509_en.htm.
64. Ahmetović, E.; Martin, M.; Grossman, I.E. “Optimization of energy and water consumption in corn-based ethanol plants,” Ind. Eng. Chem. Res.; Vol. 49, 2010; pp. 7972-7982.
65. Steinwinder, T.; Gill, E.; Gerhardt, M. Process Design of Wastewater Treatment for the NREL Cellulosic Ethanol Model. NREL/SR-5100-51838. Work performed by Brown and Caldwell, Nashville, TN, under NREL Subcontract RGB-0-40607. Golden, CO: National Renewable Energy Laboratory, September 2011. http://www.nrel.gov/docs/fy11osti/51838.pdf.
66. Mohagheghi, A.; Ruth, M.; Schell, D. “Conditioning Hemicellulosic Hydrolysates for Fermentation: Effects of Overliming pH on Sugar and Ethanol Yields.” Process Biochemistry; Vol. 41, 2006; pp. 1806-1811.
67. Reaction Engineering International. Steam and Electricity Generation Options for the Biomass-To-Ethanol Process. Work performed by Reaction Engineering International, Salt Lake City, UT, under NREL Subcontract ACO-8-18019-01. Golden, CO: National Renewable Energy Laboratory, March 1998.

93
68. Philippek, C.; Knöbig, T.; Schönfelder, H.; Werther, J. “NOx Formation and Reduction During Combustion of Wet Sewage Sludge in the Circulating Fluidized Bed.” Proceedings of the 14th International Conference on Fluidized Bed Combustion; Vol. 2, New York: ASME Press, 1997.
69. Chemical Engineering Magazine Plant Cost Index. Chemical Engineering Magazine. http://www.che.com/pci/.
70. SRI Consulting. “U.S. Producer Price Indexes – Chemicals and Allied Products/Industrial Inorganic Chemicals Index.” Chemical Economics Handbook. Menlo Park, CA: SRI Consulting, October 2008.
71. “National Employment, Hours, and Earnings Catalog, Industry: Chemicals and Allied Products.” Bureau of Labor Statistics Data website, Series ID: CEU3232500008, Years 1980-2009, annual average. http://data.bls.gov/cgi-bin/srgate.
72. North American Electric Reliability Corporation. “Wholesale Average Electricity Price Table.” U.S. Energy Information Administration website, http://www.eia.doe.gov/cneaf/electricity/wholesale/wholesale.html.
73. Garrett, D.E. Chemical Engineering Economics. New York: Van Nostrand Reinhold, 1989.
74. Peters, M.S.; Timmerhaus, K.D. Plant Design and Economics for Chemical Engineers. 5th Ed., New York: McGraw-Hill, 2003.
75. Chem Systems. Biomass to Ethanol Process Evaluation. NREL Final Subcontract Report. Work performed by Chem Systems, Tarrytown, NY. Golden, CO: National Renewable Energy Laboratory, December 1994. http://biodev.nrel.gov/pdfs/3925.pdf.
76. Walas, S.M. Chemical Process Equipment - Selection and Design. Newton, MA: Butterworth Heinemann, 1988.
77. Cran, J. “Improved factored method gives better preliminary cost estimates.” Chemical Engineering, April 6, 1981; pp. 65-79.
78. “Sugar and Sweeteners Yearbook Tables: Excel Spreadsheets.” Table 7—U.S. wholesale list price for glucose syrup, Midwest markets, monthly, quarterly, and by calendar and fiscal year. United States Department of Agriculture Economic Research Service website, http://www.ers.usda.gov/Briefing/Sugar/data.htm#yearbook. Direct download link for Table 7: http://www.ers.usda.gov/Briefing/Sugar/Data/TABLE07.XLS. 
79. Urbanchuck, J. Contribution of the Ethanol Industry to the Economy of the United States. Prepared by LECG, LLC for the Renewable Fuels Association, 2008. 
80. SRI Consulting. PEP Yearbook. Menlo Park, CA: SRI Consulting, 2008. http://www.sriconsulting.com/.

94
81. Short, W.; Packey, D.J.; Holt, T. A Manual for the Economic Evaluation and Energy Efficiency and Renewable Energy Technologies. Report No. TP-462-5173. Golden, CO: National Renewable Energy Laboratory, March 1995.
82. Internal Revenue Service. How to Depreciate Property. Publication #946. Washington, DC: Department of the Treasury Internal Revenue Service, 2009. http://www.irs.gov/pub/irs-pdf/p946.pdf.
83. Perry, R.H.; Green, D.W. Perry’s Chemical Engineers’ Handbook. 7th Ed., New York: McGraw-Hill, 1997.
84. Gary, J.H.; Handwerk, G.E. Petroleum Refining, Technology and Economics. 3rd Ed., New York: Marcel Dekker, Inc., 1994.
85. Macknick, J.; Newmark, R.; Heath, G.; Hallet, K.C. A Review of Operational Water Consumption and Withdrawal Factors for Electricity Generating Technologies. Report No. NREL/TP-6A20-50900. Golden, CO: National Renewable Energy Laboratory, March 2011. http://www.nrel.gov/docs/fy11osti/50900.pdf.
86. Dutta, A.; Ibsen, K.; Dowe, N. Complete Integrated Tests of Pretreatment and Enzymatic Hydrolysis in Conjunction with Existing Fermentation Organisms at Bench-Scale on Corn Stover that Validate $0.125 per Pound Sugars on the Pathway to Achieving $0.064 per Pound in 2012. Joule Milestone Report. Golden, CO: National Renewable Energy Laboratory, September 2007. http://devafdc.nrel.gov/bcfcdoc/9985.pdf. Rev. February 2008. http://devafdc.nrel.gov/bcfcdoc/10087.pdf.
87. Humbird, D. Demonstrate Alternative Pretreatment Technologies at Bench-Scale using Advanced Cellulase Enzymes and Integrated Technologies that have the Potential of Achieving $0.12/lb Sugar on the Pathway to $0.073/lb by 2012 (in 2007$). Joule Milestone Report, Document #10572. Golden, CO: National Renewable Energy Laboratory, September 2009. http://biodev.nrel.gov/bcfcdoc/10572.pdf.
88. “Natural Gas Prices.” U.S. Energy Information Administration website, http://tonto.eia.doe.gov/dnav/ng/ng_pri_sum_a_EPG0_PIN_DMcf_a.htm.
89. Keller and Heckmann LLP. Assessment Plan for Corn Steep Liquor (CAS #66071-94-1) in Accordance with the USEPA High Production Volume Chemical Challenge Program. Prepared for The Corn Refiners Association, 2006.
90. Verevkin, S.P.; Emel’yanenko V.N; Stepurko, E.N.; Ralys, R.V,; Zaitsau, D.H.; Stark, A. “Biomass-derived platform chemicals: Thermodynamic studies on the conversion of 5- hydroxymethylfurfural into bulk intermediates.” Ind. Eng. Chem. Res.; Vol. 48, 2009; pp. 10087-10093.
91. Lewis Sr., R.J. (295
92. Merrill, A.L.; Watt, B.K. Energy Value of Foods: Basis and Derivation. USDA ARS Handbook #74, 1973. http://www.ars.usda.gov/SP2UserFiles/Place/12354500/Data/Classics/ah74.pdf.
93. Roels, J.A. Energetics and Kinetics in Biotechnology. Amsterdam: Elsevier Biomedical Press, 1983.
94. Bailey, J.E.; Ollis, D.F. Biochemical Engineering Fundamentals. 2nd Ed., New York: McGraw-Hill, 1986.007). Hawley's Condensed Chemical Dictionary. 15th Ed., New York: John Wiley & Sons, 2007.

96
Appendix A. Individual Equipment Costs Summary

The left side of the following table shows abbreviated specifications and the purchased cost for each piece of equipment in the PFDs. The right side of the table shows the calculations used to scale the purchased cost for size and installation. Although each piece of equipment has its own line, many were quoted as part of a package so their scaling calculations are grayed out. Note that the package prices are generally listed on the first associated line-item.

NREL and Harris Group would like to acknowledge the equipment vendors who assisted us with the cost estimation effort for this design report.


97
Mechanical Equipment List Scaled Installed Costs
EQUIPMENT TITLE VENDOR DESCRIPTION HP MATERIAL
NUM REQD
$
Year of
Quote
Scaling Variable
Scaling Val
Units
Scaling Exp
Inst Factor
New Val
Size Ratio
Scaled Purch
Cost
Purch Cost in
Proj year
Inst Cost in Proj
year
C- 101 Transfer Conveyor Dearborn Midwest 160 MTPH ea., enclosed, 60 in. x 65 ft. long 20 hp ea. CS 2 $5,397,000 2009 STRM.101 94697 kg/hr 0.60 1.7 104167 1.10 $5,714,628 $5,752,952 $9,780,018
C- 102 High Angle Transfer Conveyor Dearborn Midwest 160 MTPH ea., enclosed, 72 in. wide 50 hp ea. CS 2 INCLUDED
C- 103 Reversing Load-in Conveyor Dearborn Midwest 320 MT / hr, enclosed, 84 in. wide 20 hp CS 1 INCLUDED
C- 104 Dome Reclaim System Cambelt 100 MTPH ea. 45 kw ea. CS 2 $3,046,000 2009 STRM.101 94697 kg/hr 0.60 1.7 104167 1.10 $3,225,265 $3,246,895 $5,519,721
C- 105 Reclaim Conveyor Dearborn Midwest 100 MTPH ea., enclosed, 48 in. x 125 ft. long 10 hp ea. CS 2 INCLUDED
C- 106 High Angle Transfer Conveyor Dearborn Midwest 100 MTPH, enclosed, 72 in. wide 20 hp CS 1 INCLUDED
C- 107 Elevated Transfer Conveyor Dearborn Midwest 100 MTPH, enclosed, 48 in. x 200 ft. long 10 hp CS 1 INCLUDED
C- 108 Process Feed Conveyor Dearborn Midwest 70 MTPH ea., enclosed, 42 in. x 25 ft. long 5 hp ea. CS 1 INCLUDED
M-101 Truck Scale St. Louis Scale 10' x 70', 200,000 lb CONCRETE 2 $110,000 2009 STRM.101 94697 kg/hr 0.60 1.7 104167 1.10 $116,474 $117,255 $199,333
M-102 Truck Dumper Jeffrey Rader 70' x 55 ton x 63 degree 2 x 50 hp CS 2 $484,000 2009 STRM.101 94697 kg/hr 0.60 1.7 104167 1.10 $512,485 $515,922 $877,067
M-103 Truck Dumper Hopper Jeffrey Rader 3500 cu.ft. hopper w/ drag chain conveyor 50 hp ea. CS 2 $502,000 2009 STRM.101 94697 kg/hr 0.60 1.7 104167 1.10 $531,544 $535,109 $909,685
M-104 Concrete Feedstock Storage Dome Domtec 98 ft. dia., 160 ft. high., 4000 MT CONCRETE 2 $3,500,000 2009 STRM.101 94697 kg/hr 0.60 1.7 104167 1.10 $3,705,984 $3,730,838 $6,342,424
M-105 Belt Scale Tecweigh Scale plus processor CS 2 $10,790 2009 STRM.101 94697 kg/hr 0.60 1.7 104167 1.10 $11,425 $11,502 $19,553
M-106 Dust Collection System Sly 8500 ACFM 25 hp ea. CS 6 $279,900 2009 STRM.101 94697 kg/hr 0.60 1.7 104167 1.10 $296,373 $298,360 $507,213
Area 100 Totals $14,114,178 $14,208,831 $24,155,013
EQPT NO

98
Mechanical Equipment List Scaled Installed Costs
EQUIPMENT TITLE VENDOR DESCRIPTION HP MATERIAL
NUM REQD
$
Year of
Quote
Scaling Variable
Scaling Val
Units
Scaling Exp
Inst Factor
New Val
Size Ratio
Scaled Purch
Cost
Purch Cost in
Proj year
Inst Cost in Proj
year
A- 201 In-line Sulfuric Acid Mixer KOMAX Kynar Lined - 600 gpm H2O - 5 gpm acid SS304 1 $6,000 2009 strm.a200.214 136260 kg/hr 0.50 1.0 38801 0.28 $3,202 $3,223 $3,223
A- 203 Blowdown Tank Agitator Andritz Side-mounted, 3 x 75 hp. ( 170 kW) 170 kW 316LSS 1 INCLUDED
A- 204 Flash Tank Agitator UET Mixers Side-mounted, 3 x 75 hp. ( 170 kW) 170 kW 316LSS 3 $90,000 2009 strm.a200.254 252891 kg/hr 0.50 1.5 278194 1.10 $94,395 $95,028 $142,542
A- 208 Oligomer Hold Tank Agitator UET Mixers Side-mounted, 3 x 75 hp. ( 170 kW) 170 kW 316LSS 3 $90,000 2009 strm.a200.222 264116 kg/hr 0.50 1.5 292060 1.11 $94,641 $95,276 $142,914
A- 209 Ammonia Addition Tank Agitator Lotus 10 hp SS 1 $21,900 2009 strm.a200.228 410369 kg/hr 0.50 1.5 429554 1.05 $22,406 $22,556 $33,835
A- 210 Ammonia Static Mixer KOMAX SS 1 $5,000 2009 strm.a200.275 157478 kg/hr 0.50 1.0 151360 0.96 $4,902 $4,935 $4,935
A- 224 Reacidification Tank Agitator Lotus 20 hp SS 1 $0 2009 strm.a200.239 410846 kg/hr 0.50 1.5 429554 1.05 $0 $0 $0
C- 201 Transfer Conveyor Andritz 800 mm x 7600 mm (2'-8" x 25') 40 kW ea. AL-6XN 2 INCLUDED
C- 202 Distribution Conveyor Andritz 800 mm x 7600 mm (2'-8" x 25') 40 kW ea. AL-6XN 2 INCLUDED
C- 203 Overfeed Conveyor Andritz 800 mm x 7600 mm (2'-8" x 25') 40 kW ea. AL-6XN 4 INCLUDED
C- 204 Pressurized Heating Screw Andritz 2500 mm x 9500 mm (8' x 31') 75 kW Dup. 2205 1 INCLUDED
C- 205 Pressurized Pre-heater Discharge Andritz 850 mm x 3500 mm (2'-10" x 12') 40 kW ea. Dup. 2205 2 INCLUDED
C- 206 Pressurized Transport - No. 1 Andritz 900 mm x 3500 mm (3' x 12') 20 kW Incoloy 825-
CLAD; CS 1 INCLUDED
C- 207 Pressurized Transport - No. 2 Andritz 1200 mm x 3500 mm (4' x 12') 40 kW Incoloy 825-
CLAD; CS 1 INCLUDED
H- 201 Pretreatment Water Heater Mueller 29.9 MMBtu 304SS 1 $92,000 2010 Heat.A200.QH201 -8 Gcal/hr 0.70 2.2 -9 1.15 $101,545 $97,091 $213,600
H- 244 Waste Vapor Condenser Mueller Copied H-201 304SS 1 $34,000 2009 Heat.A200.QH244 2 Gcal/hr 0.70 2.2 7 3.98 $89,346 $89,946 $197,880
M-201 Doffing Roll Storage Bins Andritz 60 cu. m. (2100 cu.ft.) with conveyors/scrapers 40 kW ea. 304/316SS 2 INCLUDED
M-202 Pin Drum Feeder Andritz 15 kW ea. 316LSS 2 INCLUDED
M-203 Plug Screw Feeder Andritz 1100kW
ea.
316LSS 2 INCLUDED
M-204 Prehydrolysis / Vertical Preheater Andritz 16' x 62' - 10 min. residence time 45 kW Dup. 2205 1 INCLUDED
M-205 Pin Drum Feeder Andritz 15 kW ea. Incoloy 825-
CLAD; CS 2 INCLUDED
M-206 Plug Screw Feeder Andritz 1100 kW
ea.
Incoloy 825-
CLAD; CS 2 INCLUDED
M-207 Pretreatment Reactor Andritz 2600 mm x 9000 mm (9' x 30') - 2 min. residence
time
Incoloy 825-
CLAD; CS 3 $19,812,400 2009 DRY101 83333 kg/hr 0.60 1.5 83333 1.00 $19,812,448 $19,945,315 $29,917,973
P- 201 Sulfuric Acid Pump Goulds 9 GPM, 245 FT TDH 316SS 1 $8,000 2009 strm.710 3720 kg/hr 0.80 2.3 1981 0.53 $4,832 $4,864 $11,187
P- 203 Blowdown Tank Discharge Pump Viking 1900 GPM, 150 FT TDH 125 316SS 1 $25,635 2010 strm.a200.222 292407 kg/hr 0.80 2.3 292060 1.00 $25,611 $24,487 $56,321
P- 204 Flash Tank Discharge Pump Viking 900 GPM, 150 FT TDH 75 316SS 1 $30,000 2009 strm.a200.254 204390 kg/hr 0.80 2.3 278194 1.36 $38,391 $38,649 $88,892
P- 208 Oligomer Hold Tank Discharge Viking 900 GPM, 150 FT TDH 75 316SS 1 $17,408 2010 strm.a200.223 292407 kg/hr 0.80 2.3 292060 1.00 $17,391 $16,629 $38,246
P- 209 Hydrolyzate Pump Goulds 1771 GPM, 150 FT TDH 100 316SS 1 $22,500 2009 strm.a200.228 402194 kg/hr 0.80 2.3 429554 1.07 $23,716 $23,875 $54,913
P- 239 Reacidified Hydrolyzate Pump Goulds 1771 GPM, 100 FT TDH 60 316SS 1 $0 2009 strm.a200.239 402194 kg/hr 0.80 2.3 429554 1.07 $0 $0 $0
S- 205 Hydrolyzate Solid-Liquid Separator Larox $35,000,000 2009 scis.a200.254b 39000 kg/hr 0.70 1.7 0 0.00 $0 $0 $0
T- 201 Sulfuric Acid Tank 12,800 gal, 24hr residence time PLASTIC 1 $6,210 2010 strm.710 1981 kg/hr 0.70 3.0 1981 1.00 $6,209 $5,937 $17,810
T- 203 Blowdown Tank Andritz 23' x 48' - 25 min. - 110,000 gal. SS316 1 INCLUDED
T- 204 Flash Tank 23' x 48' - 110,000 gal. SS316 1 $511,000 2009 strm.a200.223 264116 kg/hr 0.70 2.0 292060 1.11 $548,271 $551,948 $1,103,895
T- 208 Oligomer Conversion Tank 2.6 atm, 130C operating
30 min. hold = 30,000 gal SS316 1 $203,000 2009 strm.a200.223 264116 kg/hr 0.70 2.0 292060 1.11 $217,806 $219,267 $438,534
T- 209 Ammonia Addition Tank 118,000 gal, 1hr residence time SS304 1 $236,000 2009 strm.a200.228 410369 kg/hr 0.70 2.0 429554 1.05 $243,670 $245,304 $490,609
T- 224 Reacidification Tank Mueller 500,000 gallon SS304 1 $0 2009 strm.a200.239 410369 kg/hr 0.70 2.0 429554 1.05 $0 $0 $0
Area 200 Totals $21,348,782 $21,484,330 $32,957,310
EQPT NO

98
Mechanical Equipment List Scaled Installed Costs
EQUIPMENT TITLE VENDOR DESCRIPTION HP MATERIAL
NUM REQD
$
Year of
Quote
Scaling Variable
Scaling Val
Units
Scaling Exp
Inst Factor
New Val
Size Ratio
Scaled Purch
Cost
Purch Cost in
Proj year
Inst Cost in Proj
year
A- 201 In-line Sulfuric Acid Mixer KOMAX Kynar Lined - 600 gpm H2O - 5 gpm acid SS304 1 $6,000 2009 strm.a200.214 136260 kg/hr 0.50 1.0 38801 0.28 $3,202 $3,223 $3,223
A- 203 Blowdown Tank Agitator Andritz Side-mounted, 3 x 75 hp. ( 170 kW) 170 kW 316LSS 1 INCLUDED
A- 204 Flash Tank Agitator UET Mixers Side-mounted, 3 x 75 hp. ( 170 kW) 170 kW 316LSS 3 $90,000 2009 strm.a200.254 252891 kg/hr 0.50 1.5 278194 1.10 $94,395 $95,028 $142,542
A- 208 Oligomer Hold Tank Agitator UET Mixers Side-mounted, 3 x 75 hp. ( 170 kW) 170 kW 316LSS 3 $90,000 2009 strm.a200.222 264116 kg/hr 0.50 1.5 292060 1.11 $94,641 $95,276 $142,914
A- 209 Ammonia Addition Tank Agitator Lotus 10 hp SS 1 $21,900 2009 strm.a200.228 410369 kg/hr 0.50 1.5 429554 1.05 $22,406 $22,556 $33,835
A- 210 Ammonia Static Mixer KOMAX SS 1 $5,000 2009 strm.a200.275 157478 kg/hr 0.50 1.0 151360 0.96 $4,902 $4,935 $4,935
A- 224 Reacidification Tank Agitator Lotus 20 hp SS 1 $0 2009 strm.a200.239 410846 kg/hr 0.50 1.5 429554 1.05 $0 $0 $0
C- 201 Transfer Conveyor Andritz 800 mm x 7600 mm (2'-8" x 25') 40 kW ea. AL-6XN 2 INCLUDED
C- 202 Distribution Conveyor Andritz 800 mm x 7600 mm (2'-8" x 25') 40 kW ea. AL-6XN 2 INCLUDED
C- 203 Overfeed Conveyor Andritz 800 mm x 7600 mm (2'-8" x 25') 40 kW ea. AL-6XN 4 INCLUDED
C- 204 Pressurized Heating Screw Andritz 2500 mm x 9500 mm (8' x 31') 75 kW Dup. 2205 1 INCLUDED
C- 205 Pressurized Pre-heater Discharge Andritz 850 mm x 3500 mm (2'-10" x 12') 40 kW ea. Dup. 2205 2 INCLUDED
C- 206 Pressurized Transport - No. 1 Andritz 900 mm x 3500 mm (3' x 12') 20 kW Incoloy 825-
CLAD; CS 1 INCLUDED
C- 207 Pressurized Transport - No. 2 Andritz 1200 mm x 3500 mm (4' x 12') 40 kW Incoloy 825-
CLAD; CS 1 INCLUDED
H- 201 Pretreatment Water Heater Mueller 29.9 MMBtu 304SS 1 $92,000 2010 Heat.A200.QH201 -8 Gcal/hr 0.70 2.2 -9 1.15 $101,545 $97,091 $213,600
H- 244 Waste Vapor Condenser Mueller Copied H-201 304SS 1 $34,000 2009 Heat.A200.QH244 2 Gcal/hr 0.70 2.2 7 3.98 $89,346 $89,946 $197,880
M-201 Doffing Roll Storage Bins Andritz 60 cu. m. (2100 cu.ft.) with conveyors/scrapers 40 kW ea. 304/316SS 2 INCLUDED
M-202 Pin Drum Feeder Andritz 15 kW ea. 316LSS 2 INCLUDED
M-203 Plug Screw Feeder Andritz 1100kW
ea.
316LSS 2 INCLUDED
M-204 Prehydrolysis / Vertical Preheater Andritz 16' x 62' - 10 min. residence time 45 kW Dup. 2205 1 INCLUDED
M-205 Pin Drum Feeder Andritz 15 kW ea. Incoloy 825-
CLAD; CS 2 INCLUDED
M-206 Plug Screw Feeder Andritz 1100 kW
ea.
Incoloy 825-
CLAD; CS 2 INCLUDED
M-207 Pretreatment Reactor Andritz 2600 mm x 9000 mm (9' x 30') - 2 min. residence
time
Incoloy 825-
CLAD; CS 3 $19,812,400 2009 DRY101 83333 kg/hr 0.60 1.5 83333 1.00 $19,812,448 $19,945,315 $29,917,973
P- 201 Sulfuric Acid Pump Goulds 9 GPM, 245 FT TDH 316SS 1 $8,000 2009 strm.710 3720 kg/hr 0.80 2.3 1981 0.53 $4,832 $4,864 $11,187
P- 203 Blowdown Tank Discharge Pump Viking 1900 GPM, 150 FT TDH 125 316SS 1 $25,635 2010 strm.a200.222 292407 kg/hr 0.80 2.3 292060 1.00 $25,611 $24,487 $56,321
P- 204 Flash Tank Discharge Pump Viking 900 GPM, 150 FT TDH 75 316SS 1 $30,000 2009 strm.a200.254 204390 kg/hr 0.80 2.3 278194 1.36 $38,391 $38,649 $88,892
P- 208 Oligomer Hold Tank Discharge Viking 900 GPM, 150 FT TDH 75 316SS 1 $17,408 2010 strm.a200.223 292407 kg/hr 0.80 2.3 292060 1.00 $17,391 $16,629 $38,246
P- 209 Hydrolyzate Pump Goulds 1771 GPM, 150 FT TDH 100 316SS 1 $22,500 2009 strm.a200.228 402194 kg/hr 0.80 2.3 429554 1.07 $23,716 $23,875 $54,913
P- 239 Reacidified Hydrolyzate Pump Goulds 1771 GPM, 100 FT TDH 60 316SS 1 $0 2009 strm.a200.239 402194 kg/hr 0.80 2.3 429554 1.07 $0 $0 $0
S- 205 Hydrolyzate Solid-Liquid Separator Larox $35,000,000 2009 scis.a200.254b 39000 kg/hr 0.70 1.7 0 0.00 $0 $0 $0
T- 201 Sulfuric Acid Tank 12,800 gal, 24hr residence time PLASTIC 1 $6,210 2010 strm.710 1981 kg/hr 0.70 3.0 1981 1.00 $6,209 $5,937 $17,810
T- 203 Blowdown Tank Andritz 23' x 48' - 25 min. - 110,000 gal. SS316 1 INCLUDED
T- 204 Flash Tank 23' x 48' - 110,000 gal. SS316 1 $511,000 2009 strm.a200.223 264116 kg/hr 0.70 2.0 292060 1.11 $548,271 $551,948 $1,103,895
T- 208 Oligomer Conversion Tank 2.6 atm, 130C operating
30 min. hold = 30,000 gal SS316 1 $203,000 2009 strm.a200.223 264116 kg/hr 0.70 2.0 292060 1.11 $217,806 $219,267 $438,534
T- 209 Ammonia Addition Tank 118,000 gal, 1hr residence time SS304 1 $236,000 2009 strm.a200.228 410369 kg/hr 0.70 2.0 429554 1.05 $243,670 $245,304 $490,609
T- 224 Reacidification Tank Mueller 500,000 gallon SS304 1 $0 2009 strm.a200.239 410369 kg/hr 0.70 2.0 429554 1.05 $0 $0 $0
Area 200 Totals $21,348,782 $21,484,330 $32,957,310
EQPT NO

100
Mechanical Equipment List Scaled Installed Costs
EQUIPMENT TITLE VENDOR DESCRIPTION HP MATERIAL
NUM REQD
$
Year of
Quote
Scaling Variable
Scaling Val
Units
Scaling Exp
Inst Factor
New Val
Size Ratio
Scaled Purch
Cost
Purch Cost in
Proj year
Inst Cost in Proj
year
A- 530 Filtrate Tank Agitator Lotus 7.5 hp SS 1 $26,000 2009 strm.a500.evap.572 337439 kg/hr 0.50 1.5 355024 1.05 $26,669 $26,848 $40,272
C- 501 Lignin Wet Cake Conveyor KWS/Barnard-Boe Belt 100 ft. long x 24" wide, enclosed 10 SS304 1 $70,000 2009 strm.a500.571 28630 kg/hr 0.80 1.7 36538 1.28 $85,082 $85,653 $145,610
C- 502 Lignin Wet Cake Screw KWS/Barnard-Boe Screw conveyor - 25 ft lg x 14" dia 15 SS304 1 $20,000 2009 strm.a500.571 28630 kg/hr 0.80 1.7 36538 1.28 $24,309 $24,472 $41,603
D- 501 Beer Column Megtec 14' dia. x 76' tall, 32 trays, 24" spacing 316SS 1 $3,407,000 2009 strm.a500.511 30379 kg/hr 0.60 2.4 29213 0.96 $3,327,914 $3,350,232 $8,040,557
D- 502 Rectification Column Megtec Top 13' dia. x 68' h, Bottom 4'6" x 31' h 316SS 1 INCLUDED
H- 501 Beer Column Reboiler Megtec S & T 316SS;CS 1 INCLUDED
H- 502 Rectification Column Reboiler Megtec S & T 316SS;CS 1 INCLUDED
H- 504 Beer Column Condenser Megtec S & T 316SS;CS 1 INCLUDED
H- 505 Rectification Column Condenser GEA Rainey 92.2 MM Btu/hr 3 cells 300 tot CS 1 $487,000 2010 heat.a500.qcd502 23 Gcal/hr 0.60 2.8 23 1.00 $486,746 $465,399 $1,303,116
H- 512 Beer Column Feed Interchanger Megtec Plate & Frame 316SS 1 INCLUDED
M-503 Molecular Sieve Package (9 pieces) Delta-T SS 1 $2,601,000 2009 strm.a500.515 22687 kg/hr 0.60 1.8 21808 0.96 $2,540,057 $2,557,091 $4,602,764
M-505 Pressure Filter Pressing Compr Atlas-Copco 460 SCFM, 300 psig 150 hp 1 $75,200 2009 strm.a500.evap.sqairin 808 kg/hr 0.60 1.6 809 1.00 $75,245 $75,750 $121,199
M-507 Pressure Filter Drying Compr Atlas-Copco 4000 SCFM, 130 psig (ea) 700 hp ea. 2 $405,000 2009 strm.a500.evap.557 12233 kg/hr 0.60 1.6 12105 0.99 $402,453 $405,152 $648,243
P- 501 Beer Column Bottoms Recirc Pump Megtec 10,000 gpm 200 316SS 1 INCLUDED
P- 503 Beer Column Reflux Pump Megtec 15 gpm 2 316SS 1 INCLUDED
P- 504 Rectification Column Btms Pump Megtec 150 gpm 15 316SS 1 INCLUDED
P- 505 Rectification Column Reflux Pump Megtec 500 gpm 50 316SS 1 INCLUDED
P- 506 Beer Column Stillage Pump Megtec 2000 gpm 75 316SS 1 INCLUDED
P- 515 Scrubber Bottoms Pump Goulds 108 GPM, 104 FT TDH 316SS 1 $6,300 2009 strm.551 24527 kg/hr 0.80 2.3 27197 1.11 $6,843 $6,889 $15,844
P- 530 Filtrate Tank Discharge Pump Sulzer 590 GPM, 100 FT TDH SIZE 4X3-13 SS 1 $13,040 2010 strm.a500.evap.571 31815 kg/hr 0.80 2.3 36538 1.15 $14,567 $13,928 $32,035
P- 531 Feed Pump Warman 1014 GPM 230 FT TDH SIZE 8X6-15 100 hp SS 1 $18,173 2010 strm.a500.evap.571 31815 kg/hr 0.80 2.3 36538 1.15 $20,301 $19,411 $44,645
P- 532 Manifold Flush Pump Warman 100 hp SS 1 $17,057 2010 strm.a500.evap.571 31815 kg/hr 0.80 2.3 36538 1.15 $19,054 $18,219 $41,903
P- 533 Cloth Wash Pump Warman 150 hp SS 1 $29,154 2010 strm.a500.evap.571 31815 kg/hr 0.80 2.3 36538 1.15 $32,568 $31,140 $71,621
P- 581 Filtrate Discharge Pump Sulzer 590 GPM, 100 FT TDH SIZE 4X3-13 75 hp SS 1 $13,040 2010 strm.a500.evap.571 31815 kg/hr 0.80 2.3 36538 1.15 $14,567 $13,928 $32,035
S- 505 Pressure Filter Larox 384 sq. m fitration area ea incl packing SS316 2 $3,294,700 2010 strm.a500.evap.571 31815 kg/hr 0.80 1.7 36538 1.15 $3,680,519 $3,519,098 $5,982,467
T- 503 Beer Column Reflux Drum Megtec 4' dia, 6' high, 50 psig design 316SS 1 INCLUDED
T- 505 Rectification Column Reflux Drum Megtec 4' dia, 6' high, 50 psig design 316SS 1 INCLUDED
T- 512 Vent Scrubber Envitech Inlet Gas: 9681 acfm, 91°F, 1.97 mass% Ethanol SS304;PP 1 $215,000 2009 strm.a500.523 22608 kg/hr 0.60 2.4 21759 0.96 $210,121 $211,530 $507,673
T- 530 Filtrate Tank 13,750 gal 14' dia x 12' H SS 1 $103,000 2010 strm.a500.evap.571 31815 kg/hr 0.70 2.0 36538 1.15 $113,480 $108,503 $217,006
T- 531 Feed Tank 20,300 gal 14' dia x 18' H SS 1 $174,800 2010 strm.a500.evap.571 31815 kg/hr 0.70 2.0 36538 1.15 $192,585 $184,139 $368,278
T- 532 Recycled Water Tank Harrington Plastic 4000 gal. HDPE 1 $1,520 2010 strm.a500.evap.571 31815 kg/hr 0.70 3.0 36538 1.15 $1,675 $1,601 $4,804
T- 533 Pressing Air Compressor Receiver 1350 gal., 300 psig design CS 1 $8,000 2010 strm.a500.evap.571 31815 kg/hr 0.70 3.1 36538 1.15 $8,814 $8,427 $26,125
T- 534 Drying Air Compressor Receiver 9,000 gal., 150 psig design CS 2 $17,000 2010 strm.a500.evap.571 31815 kg/hr 0.70 3.1 36538 1.15 $18,730 $17,908 $55,516
Area 500 Totals $11,302,300 $11,145,318 $22,343,314
EQPT NO

101
Mechanical Equipment List Scaled Installed Costs
EQUIPMENT TITLE VENDOR DESCRIPTION HP MATERIAL
NUM REQD
$
Year of
Quote
Scaling Variable
Scaling Val
Units
Scaling Exp
Inst Factor
New Val
Size Ratio
Scaled Purch
Cost
Purch Cost in
Proj year
Inst Cost in Proj
year
B- 606 Biogas Blower ADI 3000 ACFM, 10 PSI 200.0 4 INCLUDED
B- 608 Aerobic Digester Blower ADI 14,000 SCFM @ 10.3 psig 1,000 8 $1,933,750 2010 strm.a600.601 393100 kg/hr 0.60 1.0 411178 1.05 $1,986,627 $1,899,498 $1,899,498
C- 614 Aerobic Sludge Screw CS 1 $25,000 2010 strm.a600.601 393100 kg/hr 0.60 1.0 411178 1.05 $25,684 $24,557 $24,557
H- 602 Anaerobic Digestor Feed Cooler ALFA LAVAL Wide gap plate & frame 2.5 mgd SS316; CS 1 $83,863 2010 strm.a600.601 393100 kg/hr 0.60 1.0 411178 1.05 $86,156 $82,378 $82,378
M-606 Biogas Emergency Flare ADI 4 $32,955 2010 strm.a600.601 393100 kg/hr 0.60 1.0 411178 1.05 $33,856 $32,371 $32,371
M-630 Polymer Addition System ADI 11.4 gph neat polymer 10.0 1 $9,300 2010 strm.a600.601 393100 kg/hr 0.60 1.0 411178 1.05 $9,554 $9,135 $9,135
M-632 Caustic Feed System ADI 0-300 gph Aerobic Digesters #1- #3 1.5 3 $22,800 2010 strm.a600.601 393100 kg/hr 0.60 1.0 411178 1.05 $23,423 $22,396 $22,396
M-640 Evaporator System $3,801,095 2010 strm.a600.601 393100 kg/hr 0.60 1.0 411178 1.05 $3,905,034 $3,733,767 $3,733,767
P- 602 Anaerobic Reactor Feed Pump ADI 2500 gpm submersible rail mounted 50.0 CS 4 $231,488 2010 strm.a600.601 393100 kg/hr 0.60 1.0 411178 1.05 $237,818 $227,388 $227,388
P- 606 Anaerobic Reactor Recirc Pump ADI 400 gpm, 50 ft TDH 7.5 4 INCLUDED
P- 607 Waste Anaerobic Sludge Pump ADI 10 gpm 3.0 6 $93,300 2010 strm.a600.601 393100 kg/hr 0.60 1.0 411178 1.05 $95,851 $91,647 $91,647
P- 608 Aeration Basin Feed Pump ADI 15.0 4 $84,000 2010 strm.a600.601 393100 kg/hr 0.60 1.0 411178 1.05 $86,297 $82,512 $82,512
P- 609 Return Activated Sludge Pump ADI 40.0 6 $177,300 2010 strm.a600.601 393100 kg/hr 0.60 1.0 411178 1.05 $182,148 $174,160 $174,160
P- 610 Reverse Osmosis Feed Pump ADI ? 1 INCLUDED
P- 611 Centrifuge Feed Pump ADI 10.0 2 $61,200 2010 strm.a600.601 393100 kg/hr 0.60 1.0 411178 1.05 $62,873 $60,116 $60,116
P- 612 Centrate Pump ADI 15.0 2 $70,800 2010 strm.a600.601 393100 kg/hr 0.60 1.0 411178 1.05 $72,736 $69,546 $69,546
P- 616 Treated Water Pump CS 1 INCLUDED
R- 609 Membrane Bioreactor ADI Includes membrane CIP and Scour system 3 $5,248,750 2010 strm.a600.601 393100 kg/hr 0.60 1.0 411178 1.05 $5,392,274 $5,155,780 $5,155,780
S- 610 Reverse Osmosis System ADI 1 $2,210,979 2010 strm.a600.601 393100 kg/hr 0.60 1.0 411178 1.05 $2,271,437 $2,171,816 $2,171,816
S- 611 Centrifuge 3 $6,493,500 2010 strm.a600.601 393100 kg/hr 0.60 1.0 411178 1.05 $6,671,062 $6,378,482 $6,378,482
T- 606 Anaerobic Basin ADI 31 Million gallonwith cover CONCRETE 4 $27,000,000 2010 strm.a600.601 393100 kg/hr 0.60 1.0 411178 1.05 $27,738,302 $26,521,754 $26,521,754
T- 608 Aeration Digester ADI 25 ft H x 115 ft x 344 ft 2 ft floor/wall thkness CONCRETE 3 $2,700,000 2010 strm.a600.601 393100 kg/hr 0.60 1.0 411178 1.05 $2,773,830 $2,652,175 $2,652,175
T- 609 Sludge Holding Tank ADI 1 INCLUDED
Area 600 Totals $51,654,964 $49,389,478 $49,389,478
A- 701 Denaturant In-line Mixer 4 inch SS304 1 $3,850 2009 strm.703 23154 kg/hr 0.50 1.0 22273 0.96 $3,776 $3,801 $3,801
A- 720 CSL Storage Tank Agitator Lotus 10 hp SS304 1 $21,200 2009 strm.735 1393 kg/hr 0.50 1.5 1323 0.95 $20,660 $20,798 $31,198
A- 760 DAP Make-up Tank Agitator Lotus 5.5 hp SS304 1 $9,800 2009 strm.755 163 kg/hr 0.50 1.5 142 0.87 $9,152 $9,214 $13,820
C- 755 DAP Bulk Bag Unloader Flexicon Super sack unloader 1 $30,000 2009 strm.755 163 kg/hr 0.60 1.7 142 0.87 $27,636 $27,822 $47,297
P- 701 Ethanol Product Pump Goulds 150 GPM, 112 FT TDH 5.0 CS 2 $9,200 2009 strm.a500.515 22681 kg/hr 0.80 3.1 21808 0.96 $8,916 $8,975 $27,824
P- 703 Sulfuric Acid Pump Goulds 5 GPM, 150 FT TDH SIZE 2X1-10 0.5 SS316 1 $7,493 2010 strm.710 1981 kg/hr 0.80 2.3 1981 1.00 $7,492 $7,163 $16,475
P- 704 Firewater Pump Goulds 2500 GPM, 150 FT TDH 125.0 CS 1 $15,000 2009 strm.a700.713 8343 kg/hr 0.80 3.1 8021 0.96 $14,536 $14,633 $45,362
P- 710 Gasoline Pump Goulds 4 GPM, 60 FT 0.5 CS 1 $3,000 2009 strm.a700.701 473 kg/hr 0.80 3.1 465 0.98 $2,959 $2,979 $9,234
P- 720 CSL Pump Goulds 8 GPM, 80 FT TDH 0.5 CS 1 $3,000 2009 strm.735 1393 kg/hr 0.80 3.1 1323 0.95 $2,879 $2,898 $8,984
P- 760 DAP Pump Goulds 2 GPM, 100 FT TDH 0.5 CS 1 $3,000 2009 strm.755 163 kg/hr 0.80 3.1 142 0.87 $2,689 $2,707 $8,392
T- 701 Ethanol Product Storage Tank Mueller 750,000 gal., 7 day storage, Floating roof A285C 2 $1,340,000 2009 strm.a500.515 22681 kg/hr 0.70 1.7 21808 0.96 $1,303,683 $1,312,426 $2,231,125
T- 703 Sulfuric Acid Storage Tank 12,600 gal, 12' dia x15' H SS 1 $96,000 2010 strm.710 1981 kg/hr 0.70 1.5 1981 1.00 $95,987 $91,777 $137,666
T- 704 Firewater Storage Tank 600,000 gal - 4 hrs @ 2500 gpm Glass lined 1 $803,000 2009 strm.a700.713 8343 kg/hr 0.70 1.7 8021 0.96 $781,201 $786,440 $1,336,948
T- 706 Ammonia Storage Tank Chemithon 28,000 gal SA- 516-70 2 $196,000 2010 strm.717 1171 kg/hr 0.70 2.0 1166 1.00 $195,389 $186,820 $373,639
T- 710 Gasoline Storage Tank 65,000 gal., floating roof CS 1 $200,000 2009 strm.a700.701 473 kg/hr 0.70 1.7 465 0.98 $197,602 $198,927 $338,176
T- 720 CSL Storage Tank 70,000 gal Glass lined CS 1 $70,000 2009 strm.735 1393 kg/hr 0.70 2.6 1323 0.95 $67,516 $67,969 $176,720
T- 755 DAP Bulk Bag Holder Flexicon Super sack holder 1 INCLUDED
T- 760 DAP Make-up Tank 12,800 gal SS304 1 $102,000 2009 strm.717 1615 kg/hr 0.70 1.8 1166 0.72 $81,192 $81,737 $147,126
Area 700 Totals $2,823,265 $2,827,086 $4,953,786
EQPT NO

102
Mechanical Equipment List Scaled Installed Costs
EQUIPMENT TITLE VENDOR DESCRIPTION HP MATERIAL
NUM REQD
$
Year of
Quote
Scaling Variable
Scaling Val
Units
Scaling Exp
Inst Factor
New Val
Size Ratio
Scaled Purch
Cost
Purch Cost in
Proj year
Inst Cost in Proj
year
H- 801 Burner Combustion Air Preheater Babcock & Wilcox 1 INCLUDED
H- 811 BFW Preheater Babcock & Wilcox 1 INCLUDED
H- 812 Pretreatment/BFW heat recovery Mueller 9.4 MM Btu/hr SS304 1 $41,000 2009 heat.QH812 -2 Gcal/hr 0.70 2.2 -2 0.93 $38,856 $39,117 $86,057
M-802 Air Intake Fan Babcock & Wilcox INCLUDED
M-803 Boiler Babcock & Wilcox 525,000 lb/hr @ 900 psig 2752 kW CS 1 $28,550,000 2010 strm.a800.a810.812 238686 kg/hr 0.60 1.8 234784 0.98 $28,269,041 $27,029,216 $48,652,589
M-804 Combustion Gas Baghouse Babcock & Wilcox INCLUDED WITH FGD SYSTEM INCLUDED
M-811 Turbine/Generator Siemens 23.6 kW, 2 extractions 1 $9,500,000 2010 work.wtotal -42200 kW 0.60 1.8 -41324 0.98 $9,381,215 $8,969,773 $16,145,591
M-820 Hot Process Water Softener System Proctor Sales 1 $78,000 2010 strm.a800.a810.812 235803 kg/hr 0.60 1.8 234784 1.00 $77,798 $74,386 $133,894
M-830 Amine Addition Pkg. Proctor Sales 1 $40,000 2010 strm.a800.a810.812 235803 kg/hr 0.00 1.8 234784 1.00 $40,000 $38,246 $68,842
M-832 Ammonia Addition Pkg Proctor Sales 1 INCLUDED
M-834 Phosphate Addition Pkg. Proctor Sales 1 INCLUDED
P- 804 Condensate Pump Proctor Sales SS316 2 INCLUDED
P- 811 Turbine Condensate Pump Proctor Sales SS304 2 INCLUDED
P- 824 Deaerator Feed Pump Proctor Sales SS304 2 INCLUDED
P- 826 BFW Pump Proctor Sales SS316 5 INCLUDED
P- 828 Blowdown Pump Proctor Sales CS 2 INCLUDED
P- 830 Amine Transfer Pump Proctor Sales CS 1 INCLUDED
T- 804 Condensate Collection Tank Proctor Sales A285C 1 INCLUDED
T- 824 Condensate Surge Drum Proctor Sales SS304 1 INCLUDED
T- 826 Deaerator Proctor Sales Tray type CS;SS316 1 $305,000 2010 strm.a800.a810.812 235803 kg/hr 0.60 3.0 234784 1.00 $304,209 $290,867 $872,600
T- 828 Blowdown Flash Drum Proctor Sales CS 1 INCLUDED
T- 830 Amine Drum Proctor Sales SS316 1 INCLUDED
Area 800 Totals $38,111,118 $36,441,604 $65,959,573
M-902 Cooling Tower System Marley SPX 44,200 gpm 750 hp FIBERGLASS 1 $1,375,000 2010 strm.a900.945 10037820 kg/hr 0.60 1.5 11923904 1.19 $1,524,650 $1,457,782 $2,186,673
M-904 Plant Air Compressor Rogers Machinery 400 SCFM@125 psig 150 hp 1 $28,000 2010 DRY101 83333 kg/hr 0.60 1.6 83333 1.00 $28,000 $26,772 $42,835
M-908 Chilled Water Package Trane 2 x 2350 tons (14.2 MM kcal/hr) 3400 hp 1 $1,275,750 2010 heat.a900.qchwop 14 Gcal/hr 0.60 1.6 13 0.95 $1,234,354 $1,180,217 $1,888,348
M-910 CIP System 100,000 GAL SS304/SS316 1 $421,000 2009 strm.a900.914 63 kg/hr 0.60 1.8 145 2.30 $694,222 $698,878 $1,257,980
P- 902 Cooling Water Pump Goulds 16,120 GPM, 100 FT TDH SIZE 20X20-28 500.0 CS 3 $283,671 2010 strm.a900.945 10982556 kg/hr 0.80 3.1 11923904 1.09 $302,961 $289,674 $897,989
P- 912 Make-up Water Pump Goulds 685 GPM, 75 FT TDH SIZE 6X4-13 20.0 CS 1 $6,864 2010 strm.a900.904 155564 kg/hr 0.80 3.1 147140 0.95 $6,565 $6,277 $19,459
P- 914 Process Water Circulating Pump Goulds 2285 GPM, 75 FT TDH SIZE 8X6-13 75.0 CS 1 $15,292 2010 strm.a900.905 518924 kg/hr 0.80 3.1 523463 1.01 $15,399 $14,724 $45,643
S- 904 Instrument Air Dryer Zeks 670 SCFM - CYCLING TYPE CS 1 $15,000 2009 DRY101 83333 kg/hr 0.60 1.8 83333 1.00 $15,000 $15,101 $27,181
T- 904 Plant Air Receiver Rogers Machinery 3800 gal - 72" x 228" vertical CS 1 $16,000 2009 DRY101 83333 kg/hr 0.60 3.1 83333 1.00 $16,000 $16,107 $49,933
T- 914 Process Water Tank No. 1 250,000 gal CS 1 $250,000 2009 strm.a900.905 451555 kg/hr 0.70 1.7 523463 1.16 $277,245 $279,104 $474,476
Area 900 Totals $4,114,396 $3,984,635 $6,890,517
Grand Totals $158,381,833 $154,486,458 $232,035,959
EQPT NO

103
Appendix B. Discounted Cash Flow Rate of Return Worksheet


104
Year -2 -1 0 1 2 3 4 5 6
Fixed Capital Investment $12,819,631 $96,147,231 $51,278,523
Land $1,848,000
Working Capital $20,030,673
Loan Payment $35,821,932 $35,821,932 $35,821,932 $35,821,932 $35,821,932 $35,821,932
Loan Interest Payment $1,538,356 $13,076,023 $19,229,446 $19,229,446 $17,902,047 $16,468,457 $14,920,179 $13,248,038 $11,442,127
Loan Principal $19,229,446 $163,450,293 $240,368,078 $223,775,593 $205,855,708 $186,502,233 $165,600,480 $143,026,587 $118,646,782
Ethanol Sales $114,997,260 $131,425,440 $131,425,440 $131,425,440 $131,425,440 $131,425,440
By-Product Credit $5,745,024 $6,565,742 $6,565,742 $6,565,742 $6,565,742 $6,565,742
Total Annual Sales $120,742,284 $137,991,181 $137,991,181 $137,991,181 $137,991,181 $137,991,181
Annual Manufacturing Cost
Feedstock $39,550,982 $45,201,122 $45,201,122 $45,201,122 $45,201,122 $45,201,122
Baghouse Bags $466,183 $466,183
Other Variable Costs $25,025,596 $26,693,969 $26,693,969 $26,693,969 $26,693,969 $26,693,969
Fixed Operating Costs $10,655,826 $10,655,826 $10,655,826 $10,655,826 $10,655,826 $10,655,826
Total Product Cost $75,698,586 $82,550,916 $82,550,916 $82,550,916 $82,550,916 $83,017,099
Annual Depreciation
General Plant Writedown 14% 24.49% 17.49% 12.49% 8.93% 8.92%
Depreciation Charge $47,822,041 $81,956,738 $58,530,965 $41,798,271 $29,884,592 $29,851,127
Remaining Value $286,831,849 $204,875,112 $146,344,146 $104,545,875 $74,661,283 $44,810,156
Steam Plant Writedown 3.75% 7.22% 6.68% 6.18% 5.71% 5.29%
Depreciation Charge $2,473,484 $4,761,622 $4,404,121 $4,074,323 $3,768,270 $3,485,963
Remaining Value $63,486,089 $58,724,468 $54,320,347 $50,246,024 $46,477,754 $42,991,790
Net Revenue ($24,481,274) ($49,180,142) ($23,963,278) ($5,352,508) $8,539,364 $10,194,864
Losses Forward ($24,481,274) ($73,661,416) ($97,624,694) ($102,977,201) ($94,437,838)
Taxable Income ($24,481,274) ($73,661,416) ($97,624,694) ($102,977,201) ($94,437,838) ($84,242,973)
Income Tax $0 $0 $0 $0 $0 $0
Annual Cash Income $9,221,766 $19,618,333 $19,618,333 $19,618,333 $19,618,333 $19,152,150
Discount Factor 1.2100 1.1000 1.0000 0.9091 0.8264 0.7513 0.6830 0.6209 0.5645
Annual Present Value $227,041,341 $8,383,423 $16,213,498 $14,739,544 $13,399,585 $12,181,441 $10,810,889
Total Capital Investment + Interest $19,609,244 $120,145,580 $90,538,643
Net Present Worth $0
Year 7 8 9 10 11 12 13 14 15 16
Fixed Capital Investment
Land
Working Capital
Loan Payment $35,821,932 $35,821,932 $35,821,932 $35,821,932 $0 $0 $0 $0 $0 $0
Loan Interest Payment $9,491,743 $7,385,327 $5,110,399 $2,653,476 $0 $0 $0 $0 $0 $0
Loan Principal $92,316,592 $63,879,988 $33,168,455 $0 $0 $0 $0 $0 $0 $0
Ethanol Sales $131,425,440 $131,425,440 $131,425,440 $131,425,440 $131,425,440 $131,425,440 $131,425,440 $131,425,440 $131,425,440 $131,425,440
By-Product Credit $6,565,742 $6,565,742 $6,565,742 $6,565,742 $6,565,742 $6,565,742 $6,565,742 $6,565,742 $6,565,742 $6,565,742
Total Annual Sales $137,991,181 $137,991,181 $137,991,181 $137,991,181 $137,991,181 $137,991,181 $137,991,181 $137,991,181 $137,991,181 $137,991,181
Annual Manufacturing Cost
Feedstock $45,201,122 $45,201,122 $45,201,122 $45,201,122 $45,201,122 $45,201,122 $45,201,122 $45,201,122 $45,201,122 $45,201,122
Baghouse Bags $466,183 $466,183
Other Variable Costs $26,693,969 $26,693,969 $26,693,969 $26,693,969 $26,693,969 $26,693,969 $26,693,969 $26,693,969 $26,693,969 $26,693,969
Fixed Operating Costs $10,655,826 $10,655,826 $10,655,826 $10,655,826 $10,655,826 $10,655,826 $10,655,826 $10,655,826 $10,655,826 $10,655,826
Total Product Cost $82,550,916 $82,550,916 $82,550,916 $82,550,916 $83,017,099 $82,550,916 $82,550,916 $82,550,916 $82,550,916 $83,017,099
Annual Depreciation
General Plant Writedown 8.93% 4.46%
Depreciation Charge $29,884,592 $14,925,564
Remaining Value $14,925,564 $0
Steam Plant Writedown 4.89% 4.52% 4.46% 4.46% 4.46% 4.46% 4.46% 4.46% 4.46% 4.46%
Depreciation Charge $3,224,104 $2,982,692 $2,943,116 $2,942,457 $2,943,116 $2,942,457 $2,943,116 $2,942,457 $2,943,116 $2,942,457
Remaining Value $39,767,686 $36,784,995 $33,841,878 $30,899,422 $27,956,306 $25,013,849 $22,070,733 $19,128,276 $16,185,160 $13,242,704
Net Revenue $12,839,826 $30,146,682 $47,386,750 $49,844,332 $52,030,966 $52,497,808 $52,497,149 $52,497,808 $52,497,149 $52,031,625
Losses Forward ($84,242,973) ($71,403,147) ($41,256,465) $0 $0 $0 $0 $0 $0 $0
Taxable Income ($71,403,147) ($41,256,465) $6,130,284 $49,844,332 $52,030,966 $52,497,808 $52,497,149 $52,497,808 $52,497,149 $52,031,625
Income Tax $0 $0 $2,145,599 $17,445,516 $18,210,838 $18,374,233 $18,374,002 $18,374,233 $18,374,002 $18,211,069
Annual Cash Income $19,618,333 $19,618,333 $17,472,734 $2,172,817 $36,763,244 $37,066,032 $37,066,263 $37,066,032 $37,066,263 $36,763,013
Discount Factor 0.5132 0.4665 0.4241 0.3855 0.3505 0.3186 0.2897 0.2633 0.2394 0.2176
Annual Present Value $10,067,307 $9,152,097 $7,410,145 $837,715 $12,885,293 $11,810,380 $10,736,776 $9,760,645 $8,873,369 $8,000,703
Total Capital Investment + Interest
Net Present Worth


105
Year 17 18 19 20 21 22 23 24 25 26
Fixed Capital Investment
Land
Working Capital
Loan Payment $0 $0 $0 $0 $0 $0 $0 $0 $0 $0
Loan Interest Payment $0 $0 $0 $0 $0 $0 $0 $0 $0 $0
Loan Principal $0 $0 $0 $0 $0 $0 $0 $0 $0 $0
Ethanol Sales $131,425,440 $131,425,440 $131,425,440 $131,425,440 $131,425,440 $131,425,440 $131,425,440 $131,425,440 $131,425,440 $131,425,440
By-Product Credit $6,565,742 $6,565,742 $6,565,742 $6,565,742 $6,565,742 $6,565,742 $6,565,742 $6,565,742 $6,565,742 $6,565,742
Total Annual Sales $137,991,181 $137,991,181 $137,991,181 $137,991,181 $137,991,181 $137,991,181 $137,991,181 $137,991,181 $137,991,181 $137,991,181
Annual Manufacturing Cost
Feedstock $45,201,122 $45,201,122 $45,201,122 $45,201,122 $45,201,122 $45,201,122 $45,201,122 $45,201,122 $45,201,122 $45,201,122
Baghouse Bags $466,183 $466,183
Other Variable Costs $26,693,969 $26,693,969 $26,693,969 $26,693,969 $26,693,969 $26,693,969 $26,693,969 $26,693,969 $26,693,969 $26,693,969
Fixed Operating Costs $10,655,826 $10,655,826 $10,655,826 $10,655,826 $10,655,826 $10,655,826 $10,655,826 $10,655,826 $10,655,826 $10,655,826
Total Product Cost $82,550,916 $82,550,916 $82,550,916 $82,550,916 $83,017,099 $82,550,916 $82,550,916 $82,550,916 $82,550,916 $83,017,099
Annual Depreciation
General Plant Writedown
Depreciation Charge
Remaining Value
Steam Plant Writedown 4.46% 4.46% 4.46% 4.46% 2.23%
Depreciation Charge $2,943,116 $2,942,457 $2,943,116 $2,942,457 $1,471,558
Remaining Value $10,299,587 $7,357,131 $4,414,015 $1,471,558 $0
Net Revenue $52,497,149 $52,497,808 $52,497,149 $52,497,808 $53,502,524 $55,440,265 $55,440,265 $55,440,265 $55,440,265 $54,974,082
Losses Forward $0 $0 $0 $0 $0 $0 $0 $0 $0 $0
Taxable Income $52,497,149 $52,497,808 $52,497,149 $52,497,808 $53,502,524 $55,440,265 $55,440,265 $55,440,265 $55,440,265 $54,974,082
Income Tax $18,374,002 $18,374,233 $18,374,002 $18,374,233 $18,725,883 $19,404,093 $19,404,093 $19,404,093 $19,404,093 $19,240,929
Annual Cash Income $37,066,263 $37,066,032 $37,066,263 $37,066,032 $36,248,199 $36,036,172 $36,036,172 $36,036,172 $36,036,172 $35,733,153
Discount Factor 0.1978 0.1799 0.1635 0.1486 0.1351 0.1228 0.1117 0.1015 0.0923 0.0839
Annual Present Value $7,333,362 $6,666,652 $6,060,630 $5,509,629 $4,898,240 $4,426,899 $4,024,453 $3,658,594 $3,325,994 $2,998,206
Total Capital Investment + Interest
Net Present Worth
Year 27 28 29 30
Fixed Capital Investment
Land ($1,848,000)
Working Capital ($20,030,673)
Loan Payment $0 $0 $0 $0
Loan Interest Payment $0 $0 $0 $0
Loan Principal $0 $0 $0 $0
Ethanol Sales $131,425,440 $131,425,440 $131,425,440 $131,425,440
By-Product Credit $6,565,742 $6,565,742 $6,565,742 $6,565,742
Total Annual Sales $137,991,181 $137,991,181 $137,991,181 $137,991,181
Annual Manufacturing Cost
Feedstock $45,201,122 $45,201,122 $45,201,122 $45,201,122
Baghouse Bags
Other Variable Costs $26,693,969 $26,693,969 $26,693,969 $26,693,969
Fixed Operating Costs $10,655,826 $10,655,826 $10,655,826 $10,655,826
Total Product Cost $82,550,916 $82,550,916 $82,550,916 $82,550,916
Annual Depreciation
General Plant Writedown
Depreciation Charge
Remaining Value
Steam Plant Writedown
Depreciation Charge
Remaining Value
Net Revenue $55,440,265 $55,440,265 $55,440,265 $55,440,265
Losses Forward $0 $0 $0 $0
Taxable Income $55,440,265 $55,440,265 $55,440,265 $55,440,265
Income Tax $19,404,093 $19,404,093 $19,404,093 $19,404,093
Annual Cash Income $36,036,172 $36,036,172 $36,036,172 $36,036,172
Discount Factor 0.0763 0.0693 0.0630 0.1486
Annual Present Value $2,748,756 $2,498,869 $2,271,699 $5,356,547
Total Capital Investment + Interest ($3,252,125)
Net Present Worth

106
Appendix C. Process Parameters/Operating Summary
Feedstock Conditioning Boiler/Turbogenerator
Moisture Content 20% Ammonia Loading (% stoich. XS 0.0% WWT sludge moisture % 79.0%
Pretreatment Ammonia Loading (g/L hydrolyzate) 4.7 First effect lignin moisture % 35.0%
Acid Conc (wt%) 0.82 Sugar Losses: Combined boiler feed moisture 44.3%
Acid Loading (mg/g dry biomass) 22.1 Xylose 1.0% Boiler feed combustion energy MMkcal/hr -181
Total Solids (wt%) 30.0% Arabinose 1.0% % from lignin cake 54%
Insoluble Solids in (wt%) 22.6% Glucose 0.0% % from biogas 36%
Insoluble Solids out (wt%) 16.6% Galactose 1.0% Boiler feed heating value (kcal/kg) -497
Temperature (°C) 158 Mannose 1.0% Boiler feed heating value (Btu/lb) -895
Pressure (atm) 5.7 Cellobiose 1.0%
Conversions Overall Fermentation Boiler efficiency (feed/steam) 80%
Cellulose to Glucolig 0.3% Total Solids (wt%) 19.8%
Cellulose to Cellobiose 0.0% Insoluble Solids (wt%) 5.1% Steam loop flow (kg/hr) 234,784
Cellulose to Glucose 9.9% Temperature (°C) 32 Total Generator Output (kW) -41,324
Cellulose to HMF 0.3% Pressure (atm) 1.0 to A100 Feedstock Handling 859
Xylan to Oligomer 2.4% Residence Time (days) 1.5 to A200 Pretreatment 5,680
Xylan to Xylose 90.0% Conversions: to A300 Hydrolysis & Fermentation 2,636
Xylan to Furfural 5.0% Glucose to Ethanol 95.0% to A400 Enzyme Production 5,340
Xylan to Tar 0.0% Glucose to Zymo (cell mass) 2.0% to A500 Recovery 2,124
Mannan to Oligomer 2.4% Glucose to Glycerol 0.4% to A600 Wastewater 7,368
Mannan to Mannose 90.0% Glucose to Succinic Acid 0.6% to A700 Storage 11
Mannan to HMF 5.0% Glucose to Acetic Acid 0.0% to A800 Boiler/Turbogen 1,368
Galactan to Oligomer 2.4% Glucose to Lactic Acid 0.0% to A900 Utilities 3,141
Galactan to Galactose 90.0% Xylose to Ethanol 85.0% Excess electricity to grid 12,797
Galactan to HMF 5.0% Xylose to Zymo 1.9% Electricity Used (kW) 28,527
Arabinan to Oligomer 2.4% Xylose to Glycerol 0.3% Electricity Used (%) 69%
Arabinan to Arabinose 90.0% Xylose to Xylitol 4.6% Wastewater Treatment
Arabinan to Furfural 5.0% Xylose to Succinic Acid 0.9% NH3-N to Ferm mg/L 1,608
Arabinan to Tar 0.0% Xylose to Acetic Acid 0.0% NH3-N out of Ferm mg/L 1,565
Acetate to Oligomer 0.0% Xylose to Lactic Acid 0.0% Protein-N 0
Acetate to Acetic Acid 100.0% Arabinose to Ethanol 85.0% Cellulase-N 202
Furfural to Tar 100.0% Arabinose to Zymo 1.9% NH3-N in Combined WW mg/L 667
HMF to Tar 100.0% Arabinose to Glycerol 0.3% Protein-N 0
Lignin to Soluble Lignin 5.0% Arabinose to Succinic Acid 1.5% Cellulase-N 43
Xylose olig to xylose Arabinose to Acetic Acid 0.0% Hydraulic Load (L/hr) 416,673
Mannose olig to mannose Arabinose to Lactic Acid 0.0% Hydraulic Load (gpm) 1,835
Arabinose olig to arabinose Galactose to Ethanol 0.0% Hydraulic Load (MMgal/day) 2.6
Galactose olig to galactose Galactose to Zymo 0.0% Total COD (kg/hr) 26,536
Enzymatic Hydrolysis Galactose to Glycerol 0.0% Total COD (g/L) 63.7
Enzyme Loading (mg/g cell) 19.9 Galactose to Succinic Acid 0.0%
Total Solids (wt%) 20.0% Galactose to Acetic Acid 0.0% Biogas composition (Dry molar%) CH4 51%
Insoluble Solids (wt%) 10.6% Galactose to Lactic Acid 0.0% CO2 49%
Temperature (°C) 32 Mannose to Ethanol 0.0% methane produced (kg/kg COD) 0.223
Pressure (atm) 1.0 Mannose to Zymo 0.0% cell mass 0.044
Residence Time (days) 3.5 Mannose to Glycerol 0.0%
Conversions: Overall Mannose to Succinic Acid 0.0%
Cellulose to Glucolig 4.0% Mannose to Acetic Acid 0.0%
Cellulose to Cellobiose 1.2% Mannose to Lactic Acid 0.0%
Cellulose to Glucose 90.0%
Glucolig to Cellobiose 0.0% Corn Steep Liquor loading wt% 0.00%
Glucolig to Glucose 0.0% Contamination Loss 3.0%
Cellobiose to Glucose 0.0% Ethanol Out of Fermenters (wt%) 5.4%
Xylan to Oligomer 0.0% Enzyme Production
Xylan to Xylose 0.0% Glucose feed (kg/hr) 2,418
Xylose Oligomer to Xylose 0.0% Protein produced (kg/hr) 579
Xylan to Tar 0.0% Protein yield (kg/kg substrate) 0.24
Arabinan to Oligomer 0.0% Protein harvest titer (g/L) 40
Arabinan to Arabinose 0.0%
Galactan to Oligomer 0.0% Compressor electricity (kW) 1408
Galactan to Galactose 0.0% Agitator electricity (kW) 2093
Galactose Oligomer to Galactose 0.0% Chiller system electricity (kW) 1587
Mannan to Oligomer 0.0% A400 total electricity (kW) 5340
Mannan to Mannose 0.0%
Mannose Oligomer to Mannose 0.0% Electricity demand (kWh/kg protn) 9
Production selectivity:
Selectivity to protein 31.3%
Selectivity to cell mass 4.1%
Selectivity to CO2 67.6%


107
Appendix D. Aspen Properties
The first table in this appendix is a list of the components used in the Aspen model. Previous
versions of the model used custom property databanks created at NREL. Where possible in the
new model, these components have been replaced with components from Aspen’s native
databanks. Property definitions for the few remaining custom components were moved into the
model itself (i.e., inside the simulation file) and are discussed here.
The second table is a list of combustion energies (LHV and HHV) computed using heats of
formation from Aspen.
The component CSL (corn steep liquor) used in previous models was removed. CSL streams are
now modeled as 50% water, 25% protein, and 25% lactic acid [89].



108
Component Property Quantity Units Reference
H2O - - - Native Aspen component
ETHANOL - - - Native Aspen component
GLUCOSE - - - Native Aspen component (dextrose)
GALACTOS - - - Duplicate of GLUCOSE
MANNOSE - - - Duplicate of GLUCOSE
XYLOSE DHFORM -216752.65 cal/mol Native Aspen component (d-xylose) with DHFORM specified (5/6 of GLUCOSE
DHFORM)
ARABINOS - - - Duplicate of XYLOSE
CELLOB - - - Cellobiose. Used native Aspen component sucrose
SUCROSE - - - Native Aspen component
GLUCOLIG MW 162.1424 Glucose oligomers. Most properties from GLUCOSE; MW is GLUCOSE minus
H2O
DHFORM -192875.34 cal/mol Back-calculated to match ΔHc of CELLULOS
GALAOLIG - - - Galactose oligomers. Duplicate of GLUCOLIG
MANOLIG - - - Mannose oligomers. Duplicate of GLUCOLIG
XYLOLIG MW 132.11612 Xylose oligomers. Most properties from XYLOSE; MW is XYLOSE minus H2O
DHFORM -149412.58 cal/mol Back-calculated to match ΔHc of XYLAN
ARABOLIG - - - Arabinose oligomers. Duplicate of XYLOLIG
EXTRACT - - - Organic extractives. Duplicate of GLUCOSE
LGNSOL - - - Solubilized lignin. Native Aspen component vanillin (see note at LIGNIN)


109
Component Property Quantity Units Reference
HMF MW 126.11 (5-hydroxymethylfurfural) Properties for HMF were estimated within Aspen using
NIST TDE routines. Specify molecular structure, MW, TB and DHFORM. From
[90].
TB 532.7 K
DHFORM -79774.53 cal/mol
DHVLWT-
1
80550000 J/kmol
TC 731.012 K NIST TDE
PC 5235810 Pa
OMEGA 0.993646710
VC 0.3425 m3/kmol
RKTZRA 0.198177974
FURFURAL - - - Native Aspen component
AACID - - - Native Aspen component (acetic acid)
LACID - - - Native Aspen component (lactic acid)
XYLITOL - - - Native Aspen component
GLYCEROL - - - Native Aspen component
SUCCACID - - - Native Aspen component (Succinic acid)
NH3 - - - Native Aspen component
H2SO4 - - - Native Aspen component
NH4SO4 - - - Native Aspen component (ammonium sulfate)
NH4ACET PLXANT/1 -1E20 atm Native Aspen component (ammonium acetate) forced non-volatile
DAP - - - Native Aspen component (diammonium phosphate)
HNO3 - - - Native Aspen component
NANO3 - - - Native Aspen component
NAOH - - - Native Aspen component
CNUTR - - - Cellulase nutrient mix. Duplicate of glucose
WNUTR - - - WWT nutrient mix. Duplicate of glucose
DENAT - - - Denaturant. Native Aspen component (n-heptane)
OIL - - - Corn oil antifoam. Native Aspen component (oleic acid)
O2 - - - Native Aspen component



110
Component Property Quantity Units Reference
N2 - - - Native Aspen component
NO - - - Native Aspen component
NO2 - - - Native Aspen component
CO - - - Native Aspen component
CO2 - - - Native Aspen component
CH4 - - - Native Aspen component
H2S - - - Native Aspen component
SO2 - - - Native Aspen component
CELLULOS DHSFRM -233200.06 cal/mol Native Aspen component with specified heat of formation; back-calculated
GALACTAN - - - Duplicate of CELLULOS
MANNAN - - - Duplicate of CELLULOS
XYLAN Formula C5H8O4 (monomer)
MW 132.117
DHSFRM -182099.93 cal/mol From [22]. Assumes the ratio of ΔHc of glucose:xylose is the same for
cellulose:xylan.
ARABINAN - - - Duplicate of xylan
LIGNIN - - - Used native Aspen component vanillin (C8H8O3). The HHV of this compound (-
23,906 BTU/kg) is very close to what we previously assumed for lignin as a
custom component (-24,206)
ACETATE - - - Used native Aspen component acetic acid
PROTEIN Formula CH1.57O0.31N0.29S0.007 Wheat gliadin [91]
MW 22.8396
DHSFRM -17618 cal/mol From literature value of gliadin ΔHc [92]
PLXANT/1 -1E20 atm Forces non-volatility
ASH - - - Native Aspen component CaO
ENZYME Formula CH1.59O0.42N0.24S0.01 Provided by Novozymes [55]
MW 24.0156
DHSFRM -17618 cal/mol copied from PROTEIN
DENZ - - - Denatured enzyme. Duplicate of enzyme



111
Component Property Quantity Units Reference
ZYMO Formula CH1.8O0.5N0.2 Z. mobilis cell mass. Average composition of several microorganisms outlined
in [93]
MW 24.6264
DHSFRM -31169.39 cal/mol From [22] after [94]
TRICHO Formula CH1.645O0.445N0.205S0.005 T. reesei cell mass. Average of generic cell mass [56] and the ENZYME
composition
MW 23.8204
DHSFRM -23200.01 cal/mol Copied BIOMASS
BIOMASS Formula CH1.64O0.39N0.23S0.0035 WWT sludge.
MW 23.238
DHSFRM -23200.01 cal/mol From [22] after [94]
TAR - - - Modeled as solid xylose
LIME - - - Aspen native component (calcium hydroxide)
CASO4 - - - Aspen native component
C - - - Aspen native component (graphite carbon)



112
MW ΔHf (IG) ΔHf (L) ΔHf (S)
cal/mol cal/mol cal/mol cal/mol Gcal/kmol BTU/lb cal/mol Gcal/kmol BTU/lb
GLUCOSE 180.16 -260103 -300428 GLUCOSE + 6 O2 → 6 H2O + 6 CO2 -610039 -0.610039 -6095 -672895 -0.672895 -6723
XYLOSE 150.13 -216753 -249440 XYLOSE + 5 O2 → 5 H2O + 5 CO2 -509283 -0.509283 -6106 -561662 -0.561662 -6734
SUCROSE 342.30 -459301 -480900 SUCROSE + 12 O2 → 11 H2O + 12 CO2 -1282278 -1.282278 -6743 -1397513 -1.397513 -7349
EXTRACT 180.16 -260103 -300428 EXTRACT + 6 O2 → 6 H2O + 6 CO2 -610039 -0.610039 -6095 -672895 -0.672895 -6723
ARABINOS 150.13 -216753 -249440 ARABINOS + 5 O2 → 5 H2O + 5 CO2 -509283 -0.509283 -6106 -561662 -0.561662 -6734
GALACTOS 180.16 -260103 -300428 GALACTOS + 6 O2 → 6 H2O + 6 CO2 -610039 -0.610039 -6095 -672895 -0.672895 -6723
MANNOSE 180.16 -260103 -300428 MANNOSE + 6 O2 → 6 H2O + 6 CO2 -610039 -0.610039 -6095 -672895 -0.672895 -6723
GLUCOLIG 162.14 -192875 -233200 GLUCOLIG + 6 O2 → 5 H2O + 6 CO2 -619511 -0.619511 -6877 -671890 -0.671890 -7459
CELLOB 342.30 -459301 -480900 CELLOB + 12 O2 → 11 H2O + 12 CO2 -1282278 -1.282278 -6743 -1397513 -1.397513 -7349
XYLOLIG 132.12 -149413 -182100 XYLOLIG + 5 O2 → 4 H2O + 5 CO2 -518866 -0.518866 -7069 -560770 -0.560770 -7640
MANOLIG 162.14 -192875 -233200 MANOLIG + 6 O2 → 5 H2O + 6 CO2 -619511 -0.619511 -6877 -671890 -0.671890 -7459
GALAOLIG 162.14 -192875 -233200 GALAOLIG + 6 O2 → 5 H2O + 6 CO2 -619511 -0.619511 -6877 -671890 -0.671890 -7459
ARABOLIG 132.12 -149413 -182100 ARABOLIG + 5 O2 → 4 H2O + 5 CO2 -518866 -0.518866 -7069 -560770 -0.560770 -7640
XYLITOL 152.15 -222246 -243145 -267149 XYLITOL + 5.5 O2 → 6 H2O + 5 CO2 -573334 -0.573334 -6783 -636190 -0.636190 -7527
LGNSOL 152.15 -88134 -108248 LGNSOL + 8.5 O2 → 4 H2O + 8 CO2 -874683 -0.874683 -10348 -916587 -0.916587 -10844
ETHANOL 46.07 -56117 -66278 ETHANOL + 3 O2 → 3 H2O + 2 CO2 -294968 -0.294968 -11525 -326395 -0.326395 -12753
H2O 18.02 -57756 -68232 -69963 NA
FURFURAL 96.09 -36066 -47738 FURFURAL + 5 O2 → 2 H2O + 5 CO2 -537716 -0.537716 -10073 -558667 -0.558667 -10466
HMF 126.11 -79775 -99677 HMF + 6 O2 → 3 H2O + 6 CO2 -637521 -0.637521 -9099 -668949 -0.668949 -9548
H2SO4 98.08 -175600 -189490 H2SO4 + -0.5 O2 → 1 H2O + 1 SO2 60835 0.060835 1116 50359 0.050359 924
N2 28.01 0 -- -- NA
CO2 44.01 -93988 -95245 NA
O2 32.00 0 -- -- NA
CH4 16.04 -17799 -- -- CH4 + 2 O2 → 2 H2O + 1 CO2 -191702 -0.191702 -21509 -212654 -0.212654 -23860
NO 30.01 21556 -- NO + 0.5 O2 → 1 NO2 -13631 -0.013631 -818 -13631 -0.013631 -818
NO2 46.01 7925 -1179 NA
NH3 17.03 -10963 -15706 NH3 + 0.75 O2 → 1.5 H2O + 0.5 N2 -75672 -0.075672 -7998 -91386 -0.091386 -9659
LACID 90.08 -143212 -163122 LACID + 3 O2 → 3 H2O + 3 CO2 -292112 -0.292112 -5837 -323539 -0.323539 -6465
AACID 60.05 -103373 -108966 AACID + 2 O2 → 2 H2O + 2 CO2 -194523 -0.194523 -5831 -215474 -0.215474 -6459
NH4SO4 132.14 -282029 -288994 -282041 NH4SO4 + 1 O2 → 4 H2O + 1 N2 + 1 SO2 -12930 -0.012930 -176 -54834 -0.054834 -747
NH4ACET 77.08 -147163 -154701 -147163 NH4ACET + 2.75 O2 → 3.5 H2O + 2 CO2 + 0.5 N2 -235422 -0.235422 -5498 -272088 -0.272088 -6354
GLYCEROL 92.09 -138029 -159483 GLYCEROL + 3.5 O2 → 4 H2O + 3 CO2 -353507 -0.353507 -6909 -395411 -0.395411 -7728
SUCCACID 118.09 -196546 -221160 -231172 SUCCACID + 3.5 O2 → 3 H2O + 4 CO2 -328062 -0.328062 -5001 -359490 -0.359490 -5480
DAP 132.06 -276457 -283996 -374250 NA
DENAT 100.20 -44819 -53568 DENAT + 11 O2 → 8 H2O + 7 CO2 -1066400 -1.066400 -19156 -1150207 -1.150207 -20662
OIL 282.47 -169628 -196067 OIL + 25.5 O2 → 17 H2O + 18 CO2 -2477579 -2.477579 -15788 -2655669 -2.655669 -16923
CNUTR 180.16 -260103 -300428 CNUTR + 6 O2 → 6 H2O + 6 CO2 -610039 -0.610039 -6095 -672895 -0.672895 -6723
WNUTR 180.16 -260103 -300428 WNUTR + 6 O2 → 6 H2O + 6 CO2 -610039 -0.610039 -6095 -672895 -0.672895 -6723
LHV HHV



113
MW ΔHf (IG) ΔHf (L) ΔHf (S)
cal/mol cal/mol cal/mol cal/mol Gcal/kmol BTU/lb cal/mol Gcal/kmol BTU/lb
SO2 64.06 -70899 -76380 NA
H2S 34.08 -4927 -8300 H2S + 1.5 O2 → 1 H2O + 1 SO2 -123728 -0.123728 -6535 -134204 -0.134204 -7088
CO 28.01 -26400 -- CO + 0.5 O2 → 1 CO2 -67589 -0.067589 -4343 -67589 -0.067589 -4343
HNO3 63.01 -32077 -41406 HNO3 + -1.75 O2 → 0.5 H2O + 0.5 N2 12528 0.012528 358 -2039 -0.002039 -58
NA2O -6965 NA
NAOH 40.00 -47234 -67046 NAOH + 0 O2 → 0.5 H2O + 0.5 NA2O 34685 0.034685 1561 9636 0.009636 434
NANO3 84.99 -118756 NANO3 + -1.25 O2 → 0.5 N2 + 0.5 NA2O 115273 0.115273 2441 115273 0.115273 2441
CELLULOS 162.14 -233200 CELLULOS + 6 O2 → 5 H2O + 6 CO2 -619511 -0.619511 -6877 -671890 -0.671890 -7459
XYLAN 132.12 -182100 XYLAN + 5 O2 → 4 H2O + 5 CO2 -518866 -0.518866 -7069 -560770 -0.560770 -7640
LIGNIN 152.15 -108248 LIGNIN + 8.5 O2 → 4 H2O + 8 CO2 -874683 -0.874683 -10348 -916587 -0.916587 -10844
ENZYME 24.02 -17900 ENZYME + 1.1975 O2 → 0.795 H2O + 1 CO2 + 0.12 N2 + 0.01 SO2 -122713 -0.122713 -9198 -130333 -0.130333 -9769
DENZ 24.02 -17900 DENZ + 1.1975 O2 → 0.795 H2O + 1 CO2 + 0.12 N2 + 0.01 SO2 -122713 -0.122713 -9198 -130333 -0.130333 -9769
BIOMASS 23.24 -23200 BIOMASS + 1.2185 O2 → 0.82 H2O + 1 CO2 + 0.115 N2 + 0.0035 SO2 -118397 -0.118397 -9171 -126739 -0.126739 -9817
ZYMO 24.63 -31169 ZYMO + 1.2 O2 → 0.9 H2O + 1 CO2 + 0.1 N2 -114800 -0.114800 -8391 -124228 -0.124228 -9080
ACETATE 60.05 -103373 -108992 ACETATE + 2 O2 → 2 H2O + 2 CO2 -194497 -0.194497 -5830 -215449 -0.215449 -6458
ARABINAN 132.12 -182100 ARABINAN + 5 O2 → 4 H2O + 5 CO2 -518866 -0.518866 -7069 -560770 -0.560770 -7640
MANNAN 162.14 -233200 MANNAN + 6 O2 → 5 H2O + 6 CO2 -619511 -0.619511 -6877 -671890 -0.671890 -7459
GALACTAN 162.14 -233200 GALACTAN + 6 O2 → 5 H2O + 6 CO2 -619511 -0.619511 -6877 -671890 -0.671890 -7459
TAR 150.13 -182100 TAR + 5 O2 → 5 H2O + 5 CO2 -576623 -0.576623 -6913 -629002 -0.629002 -7541
ASH 56.08 10485 -151688 NA
TRICHO 23.82 -23200 TRICHO + 1.19375 O2 → 0.8225 H2O + 1 CO2 + 0.1025 N2 + 0.005 SO2 -118647 -0.118647 -8966 -126909 -0.126909 -9590
PROTEIN 22.84 -17618 PROTEIN + 1.2445 O2 → 0.785 H2O + 1 CO2 + 0.145 N2 + 0.007 SO2 -122205 -0.122205 -9631 -129932 -0.129932 -10240
CARBON 12.01 0 C + 1 O2 → 1 CO2 -93988 -0.093988 -14085 -93988 -0.093988 -14085
LIME 74.09 -145878 -235522 Ca(OH)2 → 1 H2O + 1 Ash 26078 0.026078 634 15602 0.015602 379
CASO4 136.14 -315682 -342531 CaSO4 + -0.5 O2 → 1 SO2 + 1 Ash 119944 0.119944 1586 119944 0.119944 1586
LHV HHV


114
Appendix E. Process Flow Diagrams
The full set of PFDs for this process follow. Space for stream tables was limited; below is a key
to lumped components. See Section 5.1 for a discussion on how LHV is computed.
Other sugars (SS) arabinose, mannose, galactose, cellobiose, sucrose
Sugar oligomers (SS) oligomers of glucose, xylose, and all minor sugars
Organic soluble solids (SS) ammonium acetate, solubilized lignin, organic extractives, lactic acid,
cellulase and WWT nutrients
Inorganic soluble solids (SS) ammonium sulfate, diammonium phosphate, sodium hydroxide, nitric
acid, sodium nitrate
Furfurals furfural, HMF
Other organics glycerol, gasoline denaturant, corn oil, succinic acid, xylitol
CO/SOX/NOX/H2S NO, NO2, SO2, CO, H2S
Other struct. carbohydr. (IS) arabinan, mannan, galactan
Protein (IS) corn protein, cellulase, denatured cellulase
Cell mass (IS) WWT sludge, Z. mobilis from fermentation, T. reesei from cellulase
production
Other insoluble solids (IS) tar, ash, carbon, lime, gypsum


Work Stream kW Gcal/
WC101 32 0.0
WC102 79 0.0
WC103 16 0.0
WC104 96 0.0
WC105 16 0.0
WC106 16 0.0
WC107 8 0.0
WC108 4 0.0
WM102 317 0.2
WM103 158 0.1
WM106 119 0.1
COMPONENT UNITS 101 105 840
Total Flow kg/hr 104,167 104,167 0
Insoluble Solids % 67.7% 67.7% 0.0%
Soluble Solids % 12.3% 12.3% 0.0%
Temperature °C 25 25 25
Pressure atm 1.0 1.0 1.0
Vapor Fraction 0.0 0.0 1.0
Ethanol kg/hr
Water kg/hr 20,833 20,833
Glucose (SS) kg/hr
Xylose (SS) kg/hr
Other sugars (SS) kg/hr 642 642
Sugar Oligomers (SS) kg/hr
Organic Soluble Solids (SS) kg/hr 12,208 12,208
Inorganic Soluble Solids (SS) kg/hr
Ammonia kg/hr
Acetic Acid kg/hr
Sulfuric Acid kg/hr
Furfurals kg/hr
Other Organics kg/hr
Carbon Dioxide kg/hr
Methane kg/hr 0
O2 kg/hr
N2 kg/hr
CO/SOX/NOX/H2S kg/hr
Cellulose (IS) kg/hr 29,205 29,205
Xylan (IS) kg/hr 16,273 16,273
Other Struct. Carbohydr. (IS) kg/hr 3,675 3,675
Acetate (IS) kg/hr 1,508 1,508
Lignin (IS) kg/hr 13,132 13,132
Protein (IS) kg/hr 2,583 2,583
Cell Mass (IS) kg/hr
Other Insoluble Solids (IS) kg/hr 4,108 4,108
Carbon Mole Flow kmol/hr 3,117 3,117 0
COD kg/hr 101,238 101,238 0
LHV | 25°C Gcal/hr -315.6 -315.6 0.0


COMPONENT UNITS 105 212 214 215 216 217 218 222 232 516 710
Total Flow kg/hr 104,167 140,850 38,801 3,490 24,534 311,842 19,782 292,060 1,980 36,821 1,981
Insoluble Solids % 67.7% 0.0% 0.0% 0.0% 0.0% 14.8% 0.0% 15.8% 0.0% 0.0% 0.0%
Soluble Solids % 12.3% 0.0% 0.0% 0.0% 0.0% 12.0% 0.0% 12.8% 0.0% 0.0% 0.0%
Temperature °C 25 95 113 268 268 158 130 130 22 114 21
Pressure atm 1.0 4.7 6.1 13.0 13.0 5.7 2.6 9.6 11.8 6.1 5.4
Vapor Fraction 0.0 0.0 0.0 1.0 1.0 0.0 1.0 0.0 0.0 0.0 0.0
Ethanol kg/hr 18 18 8 10 18
Water kg/hr 20,833 140,850 36,767 3,490 24,534 224,002 19,533 204,469 139 36,629 139
Glucose (SS) kg/hr 0 3,550 0 3,550 0
Xylose (SS) kg/hr 0 16,643 0 16,643 0
Other sugars (SS) kg/hr 642 0 3,720 0 3,720 0
Sugar Oligomers (SS) kg/hr 0 566 0 566 0
Organic Soluble Solids (SS) kg/hr 12,208 1 12,866 0 12,866 1
Inorganic Soluble Solids (SS) kg/hr
Ammonia kg/hr 0 0 0 0 0
Acetic Acid kg/hr 1,508 36 1,473
Sulfuric Acid kg/hr 1,842 1,842 0 1,842 1,842 1,842
Furfurals kg/hr 172 1,034 205 829 172
Other Organics kg/hr 0 0 0 0 0
Carbon Dioxide kg/hr
Methane kg/hr
O2 kg/hr
N2 kg/hr
CO/SOX/NOX/H2S kg/hr 0 0
Cellulose (IS) kg/hr 29,205 26,138 26,138
Xylan (IS) kg/hr 16,273 423 423
Other Struct. Carbohydr. (IS) kg/hr 3,675 96 96
Acetate (IS) kg/hr 1,508
Lignin (IS) kg/hr 13,132 12,475 12,475
Protein (IS) kg/hr 2,583 2,583 2,583
Cell Mass (IS) kg/hr
Other Insoluble Solids (IS) kg/hr 4,108 4,377 4,377
Carbon Mole Flow kmol/hr 3,117 10 3,127 12 3,115 10
COD kg/hr 101,238 327 101,565 396 101,168 327
LHV | 25°C Gcal/hr -315.6 72.2 18.2 -0.4 -2.7 -231.7 -2.9 -230.0 1.2 16.9 1.2
Work Stream kW Gcal/hr
WC201 80 0.069
WC202 80 0.069
WC203 160 0.138
WC204 75 0.064
WC205 80 0.069
WC206 20 0.017
WC207 40 0.034
WM201 80 0.069
WM202 30 0.026
WM203 2000 1.720
WM204 45 0.039
WM205 30 0.026
WM206 2000 1.720
WM207 82 0.071
WP201 1 0.001
WP203 64 0.055
WT203 170 0.146
116



COMPONENT UNITS 211 212 222 223 224 250 251 252 253 254 255 260 273 274 275 301
Total Flow kg/hr 140,850 140,850 292,060 292,060 13,866 15,932 3,850 13,682 16,117 278,194 13,682 33,648 1,051 150,310 151,360 429,554
Insoluble Solids % 0.0% 0.0% 15.8% 15.8% 0.0% 0.0% 0.0% 0.0% 0.0% 16.6% 0.0% 0.0% 0.0% 0.0% 0.0% 10.8%
Soluble Solids % 0.0% 0.0% 12.8% 12.8% 0.0% 0.0% 0.0% 0.0% 0.0% 13.4% 0.0% 0.0% 0.0% 0.0% 0.0% 9.7%
Temperature °C 33 95 130 131 101 100 100 100 100 97 99 100 20 33 36 78
Pressure atm 5.0 4.7 9.6 5.7 1.0 1.0 1.0 1.0 1.0 1.0 1.0 1.0 9.0 5.0 5.0 4.3
Vapor Fraction 0.0 0.0 0.0 0.0 1.0 1.0 0.0 1.0 0.0 0.0 0.0 0.0 0.0 0.0 0.0 0.0
Ethanol kg/hr 10 10 4 8 0 11 1 6 11 13 6
Water kg/hr 140,850 140,850 204,469 204,469 13,715 15,702 3,831 13,382 16,035 190,754 13,382 33,248 150,310 150,310 341,063
Glucose (SS) kg/hr 3,550 3,550 0 0 0 0 0 3,550 0 0 3,550
Xylose (SS) kg/hr 16,643 16,643 0 0 0 0 0 16,643 0 0 16,476
Other sugars (SS) kg/hr 3,720 3,720 0 0 0 0 0 3,720 0 0 3,682
Sugar Oligomers (SS) kg/hr 566 566 0 0 0 0 0 566 0 0 566
Organic Soluble Solids (SS) kg/hr 12,866 12,866 0 0 0 0 0 12,866 0 0 14,727
Inorganic Soluble Solids (SS) kg/hr 2,482
Ammonia kg/hr 0 0 0 0 0 0 0 0 0 0 1,051 1,051
Acetic Acid kg/hr 1,473 1,473 23 25 11 15 32 1,450 15 58
Sulfuric Acid kg/hr 1,842 1,842 0 0 0 0 0 1,842 0 0
Furfurals kg/hr 829 829 124 197 8 274 48 705 274 329 705
Other Organics kg/hr 0 0 0 0 0 0 0 0 0 0 0
Carbon Dioxide kg/hr
Methane kg/hr
O2 kg/hr
N2 kg/hr
CO/SOX/NOX/H2S kg/hr
Cellulose (IS) kg/hr 26,138 26,138 26,138 26,138
Xylan (IS) kg/hr 423 423 423 423
Other Struct. Carbohydr. (IS) kg/hr 96 96 96 96
Acetate (IS) kg/hr
Lignin (IS) kg/hr 12,475 12,475 12,475 12,475
Protein (IS) kg/hr 2,583 2,583 2,583 2,583
Cell Mass (IS) kg/hr
Other Insoluble Solids (IS) kg/hr 4,377 4,377 4,377 4,581
Carbon Mole Flow kmol/hr 3,115 3,115 7 11 1 15 4 3,107 15 20 3,107
COD kg/hr 101,168 101,168 239 372 25 495 116 100,929 495 636 100,929
LHV | 25°C Gcal/hr 80.9 72.2 -230.0 -230.2 -1.5 -1.7 1.9 -2.1 7.8 -228.9 5.1 14.8 -4.4 86.3 81.3 -147.2
Heat Stream Gcal/hr Work Stream kW Gcal/hr
QH201 -8.636 WP204 56 0.048
QH244 7.276 WP208 100 0.086
WP209 90 0.077
WT204 127 0.109
WT208 127 0.109
WT209 90 0.077
117


COMPONENT UNITS 303 304 305 309 310
Total Flow kg/hr 44,339 42,607 1,969 211 26
Insoluble Solids % 5.0% 5.7% 0.0% 25.0% 0.0%
Soluble Solids % 15.6% 6.3% 0.0% 24.8% 100.0%
Temperature °C 32 33 32 20 20
Pressure atm 1.0 5.0 1.0 1.0 1.0
Vapor Fraction 0.0 0.0 1.0 0.0 0.0
Ethanol kg/hr 1 2,009 32
Water kg/hr 35,149 35,248 38 106
Glucose (SS) kg/hr 2,969 148 0
Xylose (SS) kg/hr 1,648 168 0
Other sugars (SS) kg/hr 401 401 0
Sugar Oligomers (SS) kg/hr 161 161 0
Organic Soluble Solids (SS) kg/hr 1,477 1,529 0 52
Inorganic Soluble Solids (SS) kg/hr 248 272 26
Ammonia kg/hr 0 0 0
Acetic Acid kg/hr
Sulfuric Acid kg/hr
Furfurals kg/hr 71 70 0
Other Organics kg/hr 1 138 0
Carbon Dioxide kg/hr 0 51 1,882
Methane kg/hr
O2 kg/hr 0 0 17
N2 kg/hr 0 0 0
CO/SOX/NOX/H2S kg/hr 0 0 0
Cellulose (IS) kg/hr 125 125
Xylan (IS) kg/hr 42 42
Other Struct. Carbohydr. (IS) kg/hr 10 10
Acetate (IS) kg/hr
Lignin (IS) kg/hr 1,248 1,248
Protein (IS) kg/hr 320 364 53
Cell Mass (IS) kg/hr 11 162
Other Insoluble Solids (IS) kg/hr 458 458
Carbon Mole Flow kmol/hr 314 273 44 4
COD kg/hr 10,201 10,280 67 132
LHV | 25°C Gcal/hr -12.7 -12.6 -0.2 -0.4 0.0
Heat Stream Gcal/hr Work Stream kW Gcal/hr
QF301-5 0.451 WF301-5 99 0.085
WP301 7 0.006
WP302 7 0.006
WT301 15 0.013
118



COMPONENT UNITS 301 302 303 304 306 311 312 315 317 422 501 551
Total Flow kg/hr 429,554 429,554 44,339 42,607 443,391 948 116 423,542 19,180 13,836 450,740 27,197
Insoluble Solids % 10.8% 10.8% 5.0% 5.7% 10.6% 25.0% 0.0% 5.5% 0.0% 5.3% 5.2% 0.0%
Soluble Solids % 9.7% 9.7% 15.6% 6.3% 9.4% 24.7% 100.0% 5.8% 0.0% 0.3% 5.4% 0.0%
Temperature °C 78 49 32 33 48 20 20 32 32 29 32 34
Pressure atm 4.3 2.5 1.0 5.0 5.1 1.0 1.0 1.0 1.0 1.9 6.0 4.3
Vapor Fraction 0.0 0.0 0.0 0.0 0.0 0.0 0.0 0.0 1.0 0.0 0.0 0.0
Ethanol kg/hr 6 6 1 2,009 6 21,517 331 21,941 424
Water kg/hr 341,063 341,063 35,149 35,248 354,117 476 351,782 369 13,054 378,525 26,743
Glucose (SS) kg/hr 3,550 3,550 2,969 148 3,550 521 0 521
Xylose (SS) kg/hr 16,476 16,476 1,648 168 16,476 1,062 0 1,062 0
Other sugars (SS) kg/hr 3,682 3,682 401 401 3,682 2,175 0 2,175 0
Sugar Oligomers (SS) kg/hr 566 566 161 161 566 1,612 0 1,612 0
Organic Soluble Solids (SS) kg/hr 14,727 14,727 1,477 1,529 14,768 235 16,421 0 41 16,421 0
Inorganic Soluble Solids (SS) kg/hr 2,482 2,482 248 272 2,482 116 2,610 2,610
Ammonia kg/hr 0 0 0 0 0 0 0 0
Acetic Acid kg/hr
Sulfuric Acid kg/hr
Furfurals kg/hr 705 705 71 70 705 703 2 706 3
Other Organics kg/hr 0 0 1 138 13 1,400 0 13 1,400 0
Carbon Dioxide kg/hr 0 51 1 520 18,323 1 549 28
Methane kg/hr
O2 kg/hr 0 0 0 0 155 0 0 0
N2 kg/hr 0 0 0 0 0 0 0 0
CO/SOX/NOX/H2S kg/hr 0 0 0 0 0 0 0 0
Cellulose (IS) kg/hr 26,138 26,138 125 125 26,138 1,255 1,255
Xylan (IS) kg/hr 423 423 42 42 423 423 423
Other Struct. Carbohydr. (IS) kg/hr 96 96 10 10 96 96 96
Acetate (IS) kg/hr
Lignin (IS) kg/hr 12,475 12,475 1,248 1,248 12,475 12,475 12,475
Protein (IS) kg/hr 2,583 2,583 320 364 3,203 237 3,445 620 3,445
Cell Mass (IS) kg/hr 11 162 108 944 108 944
Other Insoluble Solids (IS) kg/hr 4,581 4,581 458 458 4,581 4,581 4,581
Carbon Mole Flow kmol/hr 3,107 3,107 314 273 3,140 18 2,685 431 33 2,704 19
COD kg/hr 100,929 100,929 10,201 10,280 102,010 592 102,130 693 1,081 103,018 888
LHV | 25°C Gcal/hr -147.2 -136.5 -12.7 -12.6 -133.1 -1.7 0.0 -123.0 -2.1 3.6 -110.5 12.6
Heat Stream Gcal/hr Work Stream kW Gcal/hr
QC301 10.636 WA308 75 0.064
QT300 4.417 WP306 106 0.091
QC310 5.946 WP310 55 0.047
WT300 1354 1.164
WT306 15 0.013
119


COMPONENT UNITS 403 404 405 406 409 435 450 452 453 454
Total Flow kg/hr 790 8 0 6 770 1,586 32,583 32,583 31,031 1,552
Insoluble Solids % 0.5% 25.0% 0.0% 0.0% 5.3% 0.0% 0.0% 0.0% 0.0% 0.0%
Soluble Solids % 15.3% 24.7% 0.0% 0.0% 1.9% 0.0% 0.0% 0.0% 0.0% 0.0%
Temperature °C 62 20 28 28 28 28 25 40 40 40
Pressure atm 3.0 1.0 3.0 9.0 2.0 1.0 1.0 3.0 3.0 3.0
Vapor Fraction 0.0 0.0 1.0 1.0 0.0 1.0 1.0 1.0 1.0 1.0
Ethanol kg/hr
Water kg/hr 665 4 714 37 638 638 608 30
Glucose (SS) kg/hr 121 12 0
Xylose (SS) kg/hr
Other sugars (SS) kg/hr
Sugar Oligomers (SS) kg/hr
Organic Soluble Solids (SS) kg/hr 0 2 2 0
Inorganic Soluble Solids (SS) kg/hr
Ammonia kg/hr 0 6 0 0
Acetic Acid kg/hr
Sulfuric Acid kg/hr
Furfurals kg/hr
Other Organics kg/hr 0 0 0
Carbon Dioxide kg/hr 0 0 95
Methane kg/hr
O2 kg/hr 0 0 287 7,440 7,440 7,086 354
N2 kg/hr 0 0 1,167 24,504 24,504 23,337 1,167
CO/SOX/NOX/H2S kg/hr 0 0 0 0
Cellulose (IS) kg/hr
Xylan (IS) kg/hr
Other Struct. Carbohydr. (IS) kg/hr
Acetate (IS) kg/hr
Lignin (IS) kg/hr
Protein (IS) kg/hr 3 2 7
Cell Mass (IS) kg/hr 1 34
Other Insoluble Solids (IS) kg/hr
Carbon Mole Flow kmol/hr 4 0 2 2
COD kg/hr 135 5 0 73 0
LHV | 25°C Gcal/hr -0.1 0.0 0.0 0.0 0.2 0.0 0.0 0.0 0.0 0.0
Heat Stream Gcal/hr Work Stream kW Gcal/hr
QM401 1.172 WM401 1408 1.211
QF401-3 0.468 WP401 0 0.000
WT401-3 232 0.200
120



COMPONENT UNITS 400 401 402 403 405 409 410 416 422 423 440 441 442 443 446 453
Total Flow kg/hr 11,419 2,845 15,801 790 0 770 15,011 224 13,836 31,801 67 109 16 157 13 31,031
Insoluble Solids % 0.0% 0.0% 0.5% 0.5% 0.0% 5.3% 0.5% 17.5% 5.3% 0.0% 0.0% 0.0% 0.0% 25.0% 0.0% 0.0%
Soluble Solids % 0.0% 85.0% 15.3% 15.3% 0.0% 1.9% 15.3% 47.4% 0.3% 0.0% 100.0% 0.0% 0.0% 24.7% 0.0% 0.0%
Temperature °C 33 28 62 62 28 28 62 34 29 28 20 28 28 20 20 40
Pressure atm 5.0 1.0 3.0 3.0 3.0 2.0 3.0 2.0 1.9 1.0 1.0 9.0 3.0 1.0 3.2 3.0
Vapor Fraction 0.0 0.0 0.0 0.0 1.0 0.0 0.0 0.0 0.0 1.0 0.0 1.0 1.0 0.0 0.0 1.0
Ethanol kg/hr
Water kg/hr 11,419 427 13,296 665 714 12,631 79 13,054 737 79 608
Glucose (SS) kg/hr 2,418 2,418 121 12 2,297
Xylose (SS) kg/hr
Other sugars (SS) kg/hr
Sugar Oligomers (SS) kg/hr
Organic Soluble Solids (SS) kg/hr 5 0 2 4 106 41 0 67 39
Inorganic Soluble Solids (SS) kg/hr
Ammonia kg/hr 0 0 0 0 0 0 109
Acetic Acid kg/hr
Sulfuric Acid kg/hr
Furfurals kg/hr
Other Organics kg/hr 1 0 0 1 13 0 13
Carbon Dioxide kg/hr 0 0 0 0 1 2,287
Methane kg/hr
O2 kg/hr 0 0 0 0 0 5,440 7,086
N2 kg/hr 0 0 0 0 0 23,337 23,337
CO/SOX/NOX/H2S kg/hr 0 0 0 0 0 0 0 16
Cellulose (IS) kg/hr
Xylan (IS) kg/hr
Other Struct. Carbohydr. (IS) kg/hr
Acetate (IS) kg/hr
Lignin (IS) kg/hr
Protein (IS) kg/hr 69 3 7 65 39 620 39
Cell Mass (IS) kg/hr 12 1 34 11 108
Other Insoluble Solids (IS) kg/hr
Carbon Mole Flow kmol/hr 81 84 4 2 80 5 33 52 2 3 1
COD kg/hr 2,577 2,697 135 0 73 2,562 170 1,081 0 72 4 98 39
LHV | 25°C Gcal/hr 6.6 -7.9 -1.4 -0.1 0.0 0.2 -1.3 -0.5 3.6 0.0 -0.2 -0.5 0.0 -0.3 -0.1 0.0
Heat Stream Gcal/hr Work Stream kW Gcal/hr
QF400 8.104 WP400 1 0.001
QT405 -0.414 WP405 2 0.002
WP406 0 0.000
WP410 1 0.001
WP420 0 0.000
WT400 2093 1.800
WT405 6 0.005
WT406 2 0.002
WT410 7 0.006
121


COMPONENT UNITS 501 506 507 508 509 510
Total Flow kg/hr 450,740 450,740 391,501 391,501 610 58,629
Insoluble Solids % 5.2% 5.2% 5.9% 5.9% 0.0% 0.0%
Soluble Solids % 5.4% 5.4% 6.2% 6.2% 0.0% 0.0%
Temperature °C 32 103 125 47 60 117
Pressure atm 6.0 6.0 6.3 6.3 2.0 2.1
Vapor Fraction 0.0 0.0 0.0 0.0 1.0 1.0
Ethanol kg/hr 21,941 21,941 184 184 66 21,691
Water kg/hr 378,525 378,525 341,765 341,765 23 36,737
Glucose (SS) kg/hr 521 521 521 521 0 0
Xylose (SS) kg/hr 1,062 1,062 1,062 1,062 0 0
Other sugars (SS) kg/hr 2,175 2,175 2,175 2,175 0 0
Sugar Oligomers (SS) kg/hr 1,612 1,612 1,612 1,612 0 0
Organic Soluble Solids (SS) kg/hr 16,421 16,421 16,420 16,420 0 1
Inorganic Soluble Solids (SS) kg/hr 2,610 2,610 2,610 2,610
Ammonia kg/hr 0 0 0 0 0 0
Acetic Acid kg/hr
Sulfuric Acid kg/hr
Furfurals kg/hr 706 706 533 533 0 172
Other Organics kg/hr 1,400 1,400 1,400 1,400 0 0
Carbon Dioxide kg/hr 549 549 522 27
Methane kg/hr
O2 kg/hr 0 0 0 0 0 0
N2 kg/hr 0 0 0 0 0 0
CO/SOX/NOX/H2S kg/hr 0 0 0 0 0 0
Cellulose (IS) kg/hr 1,255 1,255 1,255 1,255
Xylan (IS) kg/hr 423 423 423 423
Other Struct. Carbohydr. (IS) kg/hr 96 96 96 96
Acetate (IS) kg/hr
Lignin (IS) kg/hr 12,475 12,475 12,475 12,475
Protein (IS) kg/hr 3,445 3,445 3,445 3,445
Cell Mass (IS) kg/hr 944 944 944 944
Other Insoluble Solids (IS) kg/hr 4,581 4,581 4,581 4,581
Carbon Mole Flow kmol/hr 2,704 2,704 1,738 1,738 15 951
COD kg/hr 103,018 103,018 57,393 57,393 137 45,489
LHV | 25°C Gcal/hr -110.5 -139.9 -25.6 3.8 -0.4 -137.3
Heat Stream Gcal/hr Work Stream kW Gcal/hr
QCD501 0.462 WP501 309 0.266
QH512 29.396 WP503 1 0.000
QRD501 -33.022 WP506 56 0.048
122


COMPONENT UNITS 305 317 509 510 511 516 521 523 524 550 551
Total Flow kg/hr 1,969 19,180 610 58,629 29,213 36,821 7,405 21,759 26,836 21,398 27,197
Insoluble Solids % 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0%
Soluble Solids % 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0%
Temperature °C 32 32 60 117 91 114 71 33 33 34 34
Pressure atm 1.0 1.0 2.0 2.1 1.6 6.1 1.7 1.0 5.0 0.9 4.3
Vapor Fraction 1.0 1.0 1.0 1.0 1.0 0.0 0.0 1.0 0.0 1.0 0.0
Ethanol kg/hr 32 331 66 21,691 27,022 18 5,349 428 4 424
Water kg/hr 38 369 23 36,737 2,164 36,629 2,056 429 26,836 522 26,743
Glucose (SS) kg/hr 0 0 0 0 0 0
Xylose (SS) kg/hr 0 0 0 0 0 0 0
Other sugars (SS) kg/hr 0 0 0 0 0 0 0
Sugar Oligomers (SS) kg/hr 0 0 0 0 0 0 0
Organic Soluble Solids (SS) kg/hr 0 0 0 1 1 0 0 0
Inorganic Soluble Solids (SS) kg/hr
Ammonia kg/hr 0 0 0 0 0 0 0 0 0
Acetic Acid kg/hr
Sulfuric Acid kg/hr
Furfurals kg/hr 0 2 0 172 0 172 3 0 3
Other Organics kg/hr 0 0 0 0 0 0 0 0
Carbon Dioxide kg/hr 1,882 18,323 522 27 27 20,727 20,699 28
Methane kg/hr
O2 kg/hr 17 155 0 0 0 172 172 0
N2 kg/hr 0 0 0 0 0 0 0 0
CO/SOX/NOX/H2S kg/hr 0 0 0 0 0 0 0 0 0
Cellulose (IS) kg/hr
Xylan (IS) kg/hr
Other Struct. Carbohydr. (IS) kg/hr
Acetate (IS) kg/hr
Lignin (IS) kg/hr
Protein (IS) kg/hr
Cell Mass (IS) kg/hr
Other Insoluble Solids (IS) kg/hr
Carbon Mole Flow kmol/hr 44 431 15 951 1,174 10 232 490 471 19
COD kg/hr 67 693 137 45,489 56,309 327 11,147 897 9 888
LHV | 25°C Gcal/hr -0.2 -2.1 -0.4 -137.3 -167.8 16.9 -33.3 -2.7 15.4 -0.1 12.6
Heat Stream Gcal/hr Work Stream kW Gcal/hr
QCD502 23.180 WH505 223 0.192
QRD502 -5.654 WP504 8 0.007
WP505 13 0.011
WP515 5 0.004
123


COMPONENT UNITS 511 511A 512 514 515 517 519 521
Total Flow kg/hr 29,213 29,213 7,405 21,808 21,808 7,405 21,808 7,405
Insoluble Solids % 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0%
Soluble Solids % 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0%
Temperature °C 91 116 116 116 38 35 92 71
Pressure atm 1.6 1.6 1.6 1.6 1.0 2.5 1.4 1.7
Vapor Fraction 1.0 1.0 1.0 1.0 0.0 0.0 1.0 0.0
Ethanol kg/hr 27,022 27,022 5,349 21,673 21,673 5,349 21,673 5,349
Water kg/hr 2,164 2,164 2,056 108 108 2,056 108 2,056
Glucose (SS) kg/hr
Xylose (SS) kg/hr
Other sugars (SS) kg/hr
Sugar Oligomers (SS) kg/hr
Organic Soluble Solids (SS) kg/hr
Inorganic Soluble Solids (SS) kg/hr
Ammonia kg/hr 0 0 0 0 0
Acetic Acid kg/hr
Sulfuric Acid kg/hr
Furfurals kg/hr 0 0 0 0 0
Other Organics kg/hr
Carbon Dioxide kg/hr 27 27 27 27 27
Methane kg/hr
O2 kg/hr 0 0 0 0 0
N2 kg/hr 0 0 0 0 0
CO/SOX/NOX/H2S kg/hr 0 0 0 0 0
Cellulose (IS) kg/hr
Xylan (IS) kg/hr
Other Struct. Carbohydr. (IS) kg/hr
Acetate (IS) kg/hr
Lignin (IS) kg/hr
Protein (IS) kg/hr
Cell Mass (IS) kg/hr
Other Insoluble Solids (IS) kg/hr
Carbon Mole Flow kmol/hr 1,174 1,174 232 941 941 232 941 232
COD kg/hr 56,309 56,309 11,147 45,162 45,162 11,147 45,162 11,147
LHV | 25°C Gcal/hr -167.8 -168.1 -33.3 -134.7 -138.9 -33.1 -134.5 -33.3
Heat Stream Gcal/hr Work Stream kW Gcal/hr
QH503 2.565 WM503 151 0.130
QH506 -0.301
QH507 0.214
QH509 5.187
124



COMPONENT UNITS 508 535 559 560 571 572
Total Flow kg/hr 391,501 355,024 12,105 12,044 36,538 355,024
Insoluble Solids % 5.9% 0.1% 0.0% 0.0% 62.3% 0.1%
Soluble Solids % 6.2% 6.6% 0.0% 0.0% 2.5% 6.6%
Temperature °C 47 47 80 55 55 47
Pressure atm 6.3 3.9 6.9 6.9 6.9 1.0
Vapor Fraction 0.0 0.0 1.0 1.0 0.0 0.0
Ethanol kg/hr 184 177 1 6 177
Water kg/hr 341,765 329,030 237 175 12,797 329,030
Glucose (SS) kg/hr 521 502 0 19 502
Xylose (SS) kg/hr 1,062 1,022 0 40 1,022
Other sugars (SS) kg/hr 2,175 2,094 0 81 2,094
Sugar Oligomers (SS) kg/hr 1,612 1,552 0 60 1,552
Organic Soluble Solids (SS) kg/hr 16,420 15,808 0 612 15,808
Inorganic Soluble Solids (SS) kg/hr 2,610 2,513 97 2,513
Ammonia kg/hr 0 0 0 0 0
Acetic Acid kg/hr
Sulfuric Acid kg/hr
Furfurals kg/hr 533 513 1 19 513
Other Organics kg/hr 1,400 1,348 0 52 1,348
Carbon Dioxide kg/hr
Methane kg/hr
O2 kg/hr 0 0 2,764 2,764 1 0
N2 kg/hr 0 0 9,104 9,103 1 0
CO/SOX/NOX/H2S kg/hr 0 0 0
Cellulose (IS) kg/hr 1,255 25 1,230 25
Xylan (IS) kg/hr 423 8 415 8
Other Struct. Carbohydr. (IS) kg/hr 96 2 94 2
Acetate (IS) kg/hr
Lignin (IS) kg/hr 12,475 250 12,226 250
Protein (IS) kg/hr 3,445 69 3,376 69
Cell Mass (IS) kg/hr 944 19 925 19
Other Insoluble Solids (IS) kg/hr 4,581 92 4,489 92
Carbon Mole Flow kmol/hr 1,738 801 0 937 801
COD kg/hr 57,393 25,900 4 31,489 25,900
LHV | 25°C Gcal/hr 3.8 100.8 -0.2 -0.1 -97.3 100.9
Heat Stream Gcal/hr Work Stream kW Gcal/hr
QM505 0.093 WC501 7 0.006
QM507 0.733 WC502 11 0.009
WM505 112 0.096
WM507 1043 0.897
WP530 37 0.032
WP531 76 0.066
WP532 7 0.006
WP533 11 0.010
WP581 37 0.032
WT530 6 0.005
125




COMPONENT UNITS 260 535 601 602 611 612 615 640 821 903 904 944
Total Flow kg/hr 33,648 355,024 411,178 411,178 360,712 28,626 21,860 21 4,681 147,140 147,140 17,680
Insoluble Solids % 0.0% 0.1% 0.1% 0.1% 0.1% 4.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0%
Soluble Solids % 0.0% 6.6% 5.7% 5.7% 0.8% 0.8% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0%
Temperature °C 100 47 52 35 35 35 38 86 100 13 59 28
Pressure atm 1.0 3.9 1.3 1.3 1.0 1.0 1.0 1.0 5.4 4.0 2.0 5.1
Vapor Fraction 0.0 0.0 0.0 0.0 0.0 0.0 1.0 1.0 0.0 0.0 0.0 0.0
Ethanol kg/hr 13 177 190 190 15 1 1 0
Water kg/hr 33,248 329,030 384,784 384,784 356,069 27,158 751 9 4,681 147,140 147,140 17,679
Glucose (SS) kg/hr 0 502 502 502 42 3 0 0
Xylose (SS) kg/hr 0 1,022 1,022 1,022 85 7 0 0
Other sugars (SS) kg/hr 0 2,094 2,094 2,094 175 13 0 0
Sugar Oligomers (SS) kg/hr 0 1,552 1,552 1,552 130 10 0 0
Organic Soluble Solids (SS) kg/hr 0 15,808 15,808 15,808 2,387 182 0 0
Inorganic Soluble Solids (SS) kg/hr 2,513 2,513 2,513 110 8 0 0
Ammonia kg/hr 0 0 0 0 633 48 27 0
Acetic Acid kg/hr 58 58 58 5 0 0 0
Sulfuric Acid kg/hr 0 0 0 0 0 0 0
Furfurals kg/hr 329 513 842 842 70 5 1 0
Other Organics kg/hr 0 1,348 1,348 1,348 113 9 0 0
Carbon Dioxide kg/hr 181 14 14,269 3
Methane kg/hr 3 0 5,378 0
O2 kg/hr 0 0 0 1 0 1,143 3 0
N2 kg/hr 0 0 0 0 0 5 5 0
CO/SOX/NOX/H2S kg/hr 0 0 0 300 23 285 1
Cellulose (IS) kg/hr 25 25 25 6 19
Xylan (IS) kg/hr 8 8 8 2 6
Other Struct. Carbohydr. (IS) kg/hr 2 2 2 0 1
Acetate (IS) kg/hr
Lignin (IS) kg/hr 250 250 250 64 186
Protein (IS) kg/hr 69 69 69 18 51
Cell Mass (IS) kg/hr 19 19 19 280 813
Other Insoluble Solids (IS) kg/hr 92 92 92 23 68
Carbon Mole Flow kmol/hr 20 801 820 820 115 56 660 0
COD kg/hr 636 25,900 26,536 26,536 4,180 1,892 21,994 1
LHV | 25°C Gcal/hr 14.8 100.8 128.3 134.6 187.8 8.9 -65.5 0.0 2.4 87.2 80.8 10.2
Heat Stream Gcal/hr Work Stream kW Gcal/hr
QH602 6.339 WB606 25 0.021
QT606 -1.734 WP602 4 0.004
WT606 200 0.172
126



COMPONENT UNITS 611 612 613 614 616 620 621 622 623 624 625 626 627 628 629 630 632 640
Total Flow kg/hr 360,712 28,626 91,727 120,354 110,595 2,679,447 2,201,450 221,417 9,758 386,274 2,293,177 376,324 9,929 305,040 81,234 223,602 4,504 21
Insoluble Solids % 0.1% 4.0% 1.0% 1.7% 0.1% 0.8% 1.0% 0.0% 20.0% 0.0% 1.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0%
Soluble Solids % 0.8% 0.8% 1.3% 1.1% 1.2% 1.3% 1.3% 0.0% 0.9% 1.3% 1.3% 0.0% 49.5% 0.0% 6.0% 0.0% 50.0% 0.0%
Temperature °C 35 35 25 29 29 25 25 25 29 25 25 27 100 25 25 25 20 86
Pressure atm 1.0 1.0 2.0 2.0 1.0 1.0 2.0 1.0 2.0 4.4 1.0 1.0 1.0 1.0 1.0 1.0 2.0 1.0
Vapor Fraction 0.0 0.0 0.0 0.0 0.0 0.0 0.0 1.0 0.0 0.0 0.0 0.0 0.0 0.0 0.0 1.0 0.0 1.0
Ethanol kg/hr 15 1 0 1 1 1 1 0 0 0 1 0 0 0
Water kg/hr 356,069 27,158 89,647 116,805 109,098 2,622,465 2,151,522 4,350 7,708 381,300 2,241,169 376,324 4,967 305,040 76,260 4,379 2,252 9
Glucose (SS) kg/hr 42 3 0 3 3 2 2 0 0 0 2 0 0 0
Xylose (SS) kg/hr 85 7 0 7 6 4 3 0 0 1 3 1 1 0
Other sugars (SS) kg/hr 175 13 0 14 13 8 6 0 1 1 7 1 1 0
Sugar Oligomers (SS) kg/hr 130 10 0 10 9 7 6 0 1 1 6 1 1 0
Organic Soluble Solids (SS) kg/hr 2,387 182 19 201 187 545 447 0 13 79 466 79 79 0
Inorganic Soluble Solids (SS) kg/hr 110 8 1,135 1,143 1,068 33,206 27,243 0 75 4,828 28,378 4,828 4,828 2,252 0
Ammonia kg/hr 633 48 1 49 46 19 16 1 3 3 16 3 3 0
Acetic Acid kg/hr 5 0 0 0 0 0 0 0 0 0 0 0 0 0
Sulfuric Acid kg/hr 0 0 0 0 0 0 0 0 0 0 0 0 0 0
Furfurals kg/hr 70 5 0 5 5 3 3 0 0 0 3 0 0 0
Other Organics kg/hr 113 9 0 9 8 8 6 0 1 1 7 1 1 0
Carbon Dioxide kg/hr 181 14 2 15 14 44 36 3,857 1 6 38 3 6 3
Methane kg/hr 3 0 0 0 0 0 0 3 0 0 0 0 0 0
O2 kg/hr 1 0 1 1 1 19 16 44,765 0 3 17 0 3 51,061 3
N2 kg/hr 0 0 1 1 1 37 31 168,157 0 5 32 0 5 168,162 5
CO/SOX/NOX/H2S kg/hr 300 23 10 33 31 304 249 284 2 44 259 44 44 1
Cellulose (IS) kg/hr 6 19 8 26 1 194 186 25 194
Xylan (IS) kg/hr 2 6 3 9 0 65 63 8 65
Other Struct. Carbohydr. (IS) kg/hr 0 1 1 2 0 15 14 2 15
Acetate (IS) kg/hr
Lignin (IS) kg/hr 64 186 77 263 13 1,925 1,848 250 1,925
Protein (IS) kg/hr 18 51 4 55 3 90 86 52 90
Cell Mass (IS) kg/hr 280 813 791 1,604 80 19,778 18,987 1,523 19,778
Other Insoluble Solids (IS) kg/hr 23 68 28 96 5 707 679 92 707
Carbon Mole Flow kmol/hr 115 56 40 95 12 995 952 88 83 4 991 4 4 0
COD kg/hr 4,180 1,892 1,347 3,239 448 33,869 32,322 543 2,791 200 33,669 199 200 1
LHV | 25°C Gcal/hr 187.8 8.9 48.9 57.6 62.8 1451.4 1174.7 -1.1 -5.2 227.5 1223.7 218.1 8.2 177.3 50.2 0.0 3.3 0.0
Heat Stream Gcal/hr Work Stream kW Gcal/hr
QT608 25.640 WB608 4299 3.696
WC614 1 0.000
WM640 2171 1.867
WP609 76 0.065
WP610 301 0.259
WP611 5 0.004
WP612 4 0.004
WP616 47 0.040
WP632 0 0.000
WS611 235 0.202
127



COMPONENT UNITS 309 311 404 443 515 701 703 710 713 735
Total Flow kg/hr 211 948 8 157 21,808 465 22,273 1,981 8,021 1,323
Insoluble Solids % 25.0% 25.0% 25.0% 25.0% 0.0% 0.0% 0.0% 0.0% 0.0% 25.0%
Soluble Solids % 24.8% 24.7% 24.7% 24.7% 0.0% 0.0% 0.0% 0.0% 0.0% 24.7%
Temperature °C 20 20 20 20 38 21 20 21 20 20
Pressure atm 5.4 5.4 1.0 1.0 1.0 6.9 1.0 5.4 1.0 1.0
Vapor Fraction 0.0 0.0 0.0 0.0 0.0 0.0 0.0 0.0 0.0 0.0
Ethanol kg/hr 21,673 21,673
Water kg/hr 106 476 4 79 108 108 139 8,021 665
Glucose (SS) kg/hr
Xylose (SS) kg/hr
Other sugars (SS) kg/hr
Sugar Oligomers (SS) kg/hr
Organic Soluble Solids (SS) kg/hr 52 235 2 39 327
Inorganic Soluble Solids (SS) kg/hr
Ammonia kg/hr 0 0
Acetic Acid kg/hr
Sulfuric Acid kg/hr 1,842
Furfurals kg/hr 0 0
Other Organics kg/hr 465 465
Carbon Dioxide kg/hr 27 27
Methane kg/hr
O2 kg/hr 0 0
N2 kg/hr 0 0
CO/SOX/NOX/H2S kg/hr 0 0
Cellulose (IS) kg/hr
Xylan (IS) kg/hr
Other Struct. Carbohydr. (IS) kg/hr
Acetate (IS) kg/hr
Lignin (IS) kg/hr
Protein (IS) kg/hr 53 237 2 39 331
Cell Mass (IS) kg/hr
Other Insoluble Solids (IS) kg/hr
Carbon Mole Flow kmol/hr 4 18 0 3 941 32 974 25
COD kg/hr 132 592 5 98 45,162 1,633 46,795 826
LHV | 25°C Gcal/hr -0.4 -1.7 0.0 -0.3 -138.9 -4.9 -143.6 1.2 4.7 -2.4
Work Stream kW Gcal/hr
WP701 5 0.004
WP703 1 0.000
WP704 0 0.000
WP710 0 0.000
WP720 0 0.000
WT720 2 0.002
128



COMPONENT UNITS 273 310 312 406 441 717 755
Total Flow kg/hr 1,051 26 116 6 109 1,166 142
Insoluble Solids % 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0%
Soluble Solids % 0.0% 100.0% 100.0% 0.0% 0.0% 0.0% 100.0%
Temperature °C 20 20 20 28 28 20 20
Pressure atm 17.0 1.0 1.0 9.0 9.0 17.0 1.0
Vapor Fraction 0.0 0.0 0.0 1.0 1.0 0.0 0.0
Ethanol kg/hr
Water kg/hr
Glucose (SS) kg/hr
Xylose (SS) kg/hr
Other sugars (SS) kg/hr
Sugar Oligomers (SS) kg/hr
Organic Soluble Solids (SS) kg/hr
Inorganic Soluble Solids (SS) kg/hr 26 116 142
Ammonia kg/hr 1,051 6 109 1,166
Acetic Acid kg/hr
Sulfuric Acid kg/hr
Furfurals kg/hr
Other Organics kg/hr
Carbon Dioxide kg/hr
Methane kg/hr
O2 kg/hr
N2 kg/hr
CO/SOX/NOX/H2S kg/hr
Cellulose (IS) kg/hr
Xylan (IS) kg/hr
Other Struct. Carbohydr. (IS) kg/hr
Acetate (IS) kg/hr
Lignin (IS) kg/hr
Protein (IS) kg/hr
Cell Mass (IS) kg/hr
Other Insoluble Solids (IS) kg/hr
Carbon Mole Flow kmol/hr
COD kg/hr
LHV | 25°C Gcal/hr -4.4 0.0 0.0 0.0 -0.5 -4.8 0.0
Work Stream kW Gcal/hr
WC755 0 0.000
WP760 0 0.000
WT760 3 0.002
129



COMPONENT UNITS 560 615 802 803 804 806 807 809 810 850 851
Total Flow kg/hr 12,044 21,860 318,399 318,399 284,495 364,696 364,696 5,725 363,445 3,579 895
Insoluble Solids % 0.0% 0.0% 0.0% 0.0% 0.0% 1.2% 1.2% 100.0% 0.0% 0.0% 100.0%
Soluble Solids % 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0%
Temperature °C 55 38 29 192 25 278 149 0 145 33 25
Pressure atm 6.9 1.0 1.0 1.0 1.0 1.0 1.0 1.0 1.0 5.0 1.0
Vapor Fraction 1.0 1.0 1.0 1.0 1.0 1.0 1.0 0.0 1.0 0.0 0.0
Ethanol kg/hr 1 1 2 2
Water kg/hr 175 751 6,498 6,498 5,572 50,698 50,698 54,451 3,579
Glucose (SS) kg/hr 0 0 0 0
Xylose (SS) kg/hr 0 0 0 0
Other sugars (SS) kg/hr 0 0 0 0
Sugar Oligomers (SS) kg/hr 0 0 0 0
Organic Soluble Solids (SS) kg/hr 0 0 0 0
Inorganic Soluble Solids (SS) kg/hr 0 0 0 80 80 80
Ammonia kg/hr 0 27 27 27 30 30 30
Acetic Acid kg/hr 0 0 0
Sulfuric Acid kg/hr 0 0 0 0 0 0
Furfurals kg/hr 1 1 2 2
Other Organics kg/hr 0 0 0 0
Carbon Dioxide kg/hr 14,269 14,269 14,269 73,396 73,396 73,396
Methane kg/hr 5,378 5,378 5,378
O2 kg/hr 2,764 1,143 68,873 68,873 64,966 11,479 11,479 11,324
N2 kg/hr 9,103 5 223,065 223,065 213,957 223,985 223,985 223,985
CO/SOX/NOX/H2S kg/hr 285 285 285 797 797 178
Cellulose (IS) kg/hr
Xylan (IS) kg/hr
Other Struct. Carbohydr. (IS) kg/hr
Acetate (IS) kg/hr
Lignin (IS) kg/hr
Protein (IS) kg/hr
Cell Mass (IS) kg/hr
Other Insoluble Solids (IS) kg/hr 4,230 4,230 5,725 895
Carbon Mole Flow kmol/hr 0 660 660 660 1,680 1,680 10 1,670
COD kg/hr 4 21,994 21,997 21,997 530 530 326 49
LHV | 25°C Gcal/hr -0.1 -65.5 -65.7 -78.8 0.0 -26.4 -13.3 0.1 -11.6 2.1 0.3
Heat Stream Gcal/hr Work Stream kW Gcal/hr
QH801 13.112 WCOMBFAN 142 0.122
WM804 596 0.512
130



COMPONENT UNITS 215 216 571 623 801 803 806 812 812B 813A 813B 815 815A 815E 816 816A 821 823 840
Total Flow kg/hr 3,490 24,534 36,538 9,758 46,297 318,399 364,696 234,784 30,132 242,044 242,045 75,071 104 101,453 101,453 101,453 4,681 30,132 0
Insoluble Solids % 0.0% 0.0% 62.3% 20.0% 53.4% 0.0% 1.2% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0%
Soluble Solids % 0.0% 0.0% 2.5% 0.9% 2.2% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0%
Temperature °C 266 266 55 29 47 192 278 454 266 114 176 233 233 46 46 46 100 192 25
Pressure atm 13.0 13.0 6.9 2.0 1.0 1.0 1.0 59.9 13.0 62.2 62.2 9.5 9.5 0.1 0.1 5.0 5.4 13.0 1.0
Vapor Fraction 1.0 1.0 0.0 0.0 0.0 1.0 1.0 1.0 1.0 0.0 0.0 1.0 1.0 0.9 0.0 0.0 0.0 0.0 1.0
Ethanol kg/hr 6 0 6 2
Water kg/hr 3,490 24,534 12,797 7,708 20,505 6,498 50,698 234,784 30,132 242,044 242,045 75,071 104 101,453 101,453 101,453 4,681 30,132
Glucose (SS) kg/hr 19 0 20 0
Xylose (SS) kg/hr 40 0 40 0
Other sugars (SS) kg/hr 81 1 82 0
Sugar Oligomers (SS) kg/hr 60 1 61 0
Organic Soluble Solids (SS) kg/hr 612 13 625 0
Inorganic Soluble Solids (SS) kg/hr 97 75 173 0 80
Ammonia kg/hr 0 3 3 27 30
Acetic Acid kg/hr 0 0 0
Sulfuric Acid kg/hr 0 0 0 0
Furfurals kg/hr 19 0 20 2
Other Organics kg/hr 52 1 53 0
Carbon Dioxide kg/hr 1 1 14,269 73,396
Methane kg/hr 0 0 5,378 0
O2 kg/hr 1 0 1 68,873 11,479
N2 kg/hr 1 0 1 223,065 223,985
CO/SOX/NOX/H2S kg/hr 2 2 285 797
Cellulose (IS) kg/hr 1,230 25 1,255
Xylan (IS) kg/hr 415 8 423
Other Struct. Carbohydr. (IS) kg/hr 94 2 96
Acetate (IS) kg/hr
Lignin (IS) kg/hr 12,226 250 12,475
Protein (IS) kg/hr 3,376 52 3,428
Cell Mass (IS) kg/hr 925 1,523 2,448
Other Insoluble Solids (IS) kg/hr 4,489 92 4,581 4,230
Carbon Mole Flow kmol/hr 937 83 1,021 660 1,680 0
COD kg/hr 31,489 2,791 34,279 21,997 530 0
LHV | 25°C Gcal/hr -0.3 -2.5 -97.3 -5.2 -102.4 -78.8 -26.4 -42.9 -3.0 119.4 103.9 -6.4 0.0 6.3 56.9 56.9 2.4 12.4 0.0
Heat Stream Gcal/hr Work Stream kW Gcal/hr
QBOILER 144.629 WKNET -12797 -11.003
QH811 15.467 WP811 20 0.017
QM811 50.717 WPLANT -28527 -24.529
WTOTAL -41324 -35.532
131




COMPONENT UNITS 218 250 251 811 811A 811B 811H 812E 813 813A 815A 816A 821 821V 823 896
Total Flow kg/hr 19,782 15,932 3,850 35,284 206,656 241,940 35,284 0 242,044 242,044 104 101,453 4,681 2,580 30,132 75,071
Insoluble Solids % 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0%
Soluble Solids % 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0%
Temperature °C 130 100 100 33 114 111 95 0 113 114 233 46 100 100 192 171
Pressure atm 2.6 1.0 1.0 5.4 5.2 4.4 5.4 1.5 1.5 62.2 9.5 5.0 5.4 1.0 13.0 8.0
Vapor Fraction 1.0 1.0 0.0 0.0 0.0 0.0 0.0 0.0 0.0 0.0 1.0 0.0 0.0 1.0 0.0 0.0
Ethanol kg/hr 8 8 0
Water kg/hr 19,533 15,702 3,831 35,284 206,656 241,940 35,284 242,044 242,044 104 101,453 4,681 2,580 30,132 75,071
Glucose (SS) kg/hr 0 0 0
Xylose (SS) kg/hr 0 0 0
Other sugars (SS) kg/hr 0 0 0
Sugar Oligomers (SS) kg/hr 0 0 0
Organic Soluble Solids (SS) kg/hr 0 0 0
Inorganic Soluble Solids (SS) kg/hr
Ammonia kg/hr 0 0 0
Acetic Acid kg/hr 36 25 11
Sulfuric Acid kg/hr 0 0 0
Furfurals kg/hr 205 197 8
Other Organics kg/hr 0 0 0
Carbon Dioxide kg/hr
Methane kg/hr
O2 kg/hr
N2 kg/hr
CO/SOX/NOX/H2S kg/hr
Cellulose (IS) kg/hr
Xylan (IS) kg/hr
Other Struct. Carbohydr. (IS) kg/hr
Acetate (IS) kg/hr
Lignin (IS) kg/hr
Protein (IS) kg/hr
Cell Mass (IS) kg/hr
Other Insoluble Solids (IS) kg/hr
Carbon Mole Flow kmol/hr 12 11 1
COD kg/hr 396 372 25
LHV | 25°C Gcal/hr -2.9 -1.7 1.9 20.2 101.8 119.9 18.1 0.0 119.5 119.4 0.0 56.9 2.4 -0.1 12.4 32.6
Heat Stream Gcal/hr Work Stream kW Gcal/hr
QH812 -2.185 WP804 8 0.007
WP824 9 0.008
WP826 559 0.481
WP828 2 0.002
132



Work Stream kW Gcal/hr
WM830 10 0.009
WM832 10 0.009
WM834 10 0.009
WP830 1 0.001
133




COMPONENT UNITS 940 941 944 945 948 949 950 951
Total Flow kg/hr 11,923,904 155,041 17,678 11,923,904 6,549,403 6,687,697 1,372,608 1,372,608
Insoluble Solids % 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0%
Soluble Solids % 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0%
Temperature °C 28 33 28 37 25 37 4 15
Pressure atm 5.0 5.0 5.1 5.0 1.0 1.0 4.1 4.1
Vapor Fraction 0.0 0.0 0.0 0.0 1.0 1.0 0.0 0.0
Ethanol kg/hr
Water kg/hr 11,923,687 155,041 17,678 11,923,687 128,274 266,568 1,372,608 1,372,608
Glucose (SS) kg/hr
Xylose (SS) kg/hr
Other sugars (SS) kg/hr
Sugar Oligomers (SS) kg/hr
Organic Soluble Solids (SS) kg/hr
Inorganic Soluble Solids (SS) kg/hr
Ammonia kg/hr
Acetic Acid kg/hr
Sulfuric Acid kg/hr
Furfurals kg/hr
Other Organics kg/hr
Carbon Dioxide kg/hr
Methane kg/hr
O2 kg/hr 80 0 80 1,495,590 1,495,590
N2 kg/hr 138 0 138 4,925,539 4,925,539
CO/SOX/NOX/H2S kg/hr
Cellulose (IS) kg/hr
Xylan (IS) kg/hr
Other Struct. Carbohydr. (IS) kg/hr
Acetate (IS) kg/hr
Lignin (IS) kg/hr
Protein (IS) kg/hr
Cell Mass (IS) kg/hr
Other Insoluble Solids (IS) kg/hr
Carbon Mole Flow kmol/hr
COD kg/hr
LHV | 25°C Gcal/hr 6898.7 89.0 10.2 6801.3 0.0 -20.3 824.1 810.6
Heat Stream Gcal/hr Work Stream kW Gcal/hr
QCHWOP 13.440 WM902 1021 0.878
QTTOTAL 97.401 WM904 186 0.160
WM908 2489 2.140
WP902 1598 1.374
134




COMPONENT UNITS 211 274 400 524 626 811 850 904 905 906 941
Total Flow kg/hr 140,850 150,310 11,419 26,836 376,324 35,284 3,579 147,140 523,463 145 155,041
Insoluble Solids % 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0%
Soluble Solids % 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0% 0.0%
Temperature °C 33 33 33 33 27 33 33 59 33 20 33
Pressure atm 5.0 5.0 5.0 5.0 1.0 5.0 5.0 2.0 5.0 1.0 5.0
Vapor Fraction 0.0 0.0 0.0 0.0 0.0 0.0 0.0 0.0 0.0 0.0 0.0
Ethanol kg/hr
Water kg/hr 140,850 150,310 11,419 26,836 376,324 35,284 3,579 147,140 523,463 145 155,041
Glucose (SS) kg/hr
Xylose (SS) kg/hr
Other sugars (SS) kg/hr
Sugar Oligomers (SS) kg/hr
Organic Soluble Solids (SS) kg/hr
Inorganic Soluble Solids (SS) kg/hr
Ammonia kg/hr
Acetic Acid kg/hr
Sulfuric Acid kg/hr
Furfurals kg/hr
Other Organics kg/hr
Carbon Dioxide kg/hr
Methane kg/hr
O2 kg/hr
N2 kg/hr
CO/SOX/NOX/H2S kg/hr
Cellulose (IS) kg/hr
Xylan (IS) kg/hr
Other Struct. Carbohydr. (IS) kg/hr
Acetate (IS) kg/hr
Lignin (IS) kg/hr
Protein (IS) kg/hr
Cell Mass (IS) kg/hr
Other Insoluble Solids (IS) kg/hr
Carbon Mole Flow kmol/hr
COD kg/hr
LHV | 25°C Gcal/hr 80.8 86.3 6.6 15.4 218.1 20.3 2.1 80.8 300.5 0.1 89.0
Heat Stream Gcal/hr Work Stream kW Gcal/hr
QT914 1.615 WP914 72 0.062
135





COMPONENT UNITS 906 909 914 916
Total Flow kg/hr 145 145 145 145
Insoluble Solids % 0.0% 0.0% 0.0% 0.0%
Soluble Solids % 0.0% 0.0% 0.0% 0.0%
Temperature °C 20 121 20 20
Pressure atm 1.0 1.0 1.0 1.0
Vapor Fraction 0.0 1.0 0.0 0.0
Ethanol kg/hr
Water kg/hr 145 145 145 145
Glucose (SS) kg/hr
Xylose (SS) kg/hr
Other sugars (SS) kg/hr
Sugar Oligomers (SS) kg/hr
Organic Soluble Solids (SS) kg/hr
Inorganic Soluble Solids (SS) kg/hr
Ammonia kg/hr
Acetic Acid kg/hr
Sulfuric Acid kg/hr
Furfurals kg/hr
Other Organics kg/hr
Carbon Dioxide kg/hr
Methane kg/hr
O2 kg/hr
N2 kg/hr
CO/SOX/NOX/H2S kg/hr
Cellulose (IS) kg/hr
Xylan (IS) kg/hr
Other Struct. Carbohydr. (IS) kg/hr
Acetate (IS) kg/hr
Lignin (IS) kg/hr
Protein (IS) kg/hr
Cell Mass (IS) kg/hr
Other Insoluble Solids (IS) kg/hr
Carbon Mole Flow kmol/hr
COD kg/hr
LHV | 25°C Gcal/hr 0.1 0.0 0.1 0.1
Heat Stream Gcal/hr Work Stream kW Gcal/hr
QH910 -0.091 WM910 250 0.215
136





F1147-E(10/2008)
REPORT DOCUMENTATION PAGE Form Approved
OMB No. 0704-0188
The public reporting burden for this collection of information is estimated to average 1 hour per response, including the time for reviewing instructions, searching existing data sources,
gathering and maintaining the data needed, and completing and reviewing the collection of information. Send comments regarding this burden estimate or any other aspect of this
collection of information, including suggestions for reducing the burden, to Department of Defense, Executive Services and Communications Directorate (0704-0188). Respondents
should be aware that notwithstanding any other provision of law, no person shall be subject to any penalty for failing to comply with a collection of information if it does not display a
currently valid OMB control number.
PLEASE DO NOT RETURN YOUR FORM TO THE ABOVE ORGANIZATION.
1. REPORT DATE (DD-MM-YYYY)
May 2011
2. REPORT TYPE
Technical Report
3. DATES COVERED (From - To)
4. TITLE AND SUBTITLE
Process Design and Economics for Biochemical Conversion of
Lignocellulosic Biomass to Ethanol: Dilute-Acid Pretreatment and
Enzymatic Hydrolysis of Corn Stover
5a. CONTRACT NUMBER
DE-AC36-08GO28308
5b. GRANT NUMBER
5c. PROGRAM ELEMENT NUMBER
6. AUTHOR(S)
D. Humbird, R. Davis, L. Tao, C. Kinchin, D. Hsu, A. Aden,
P. Schoen, J. Lukas, B. Olthof, M. Worley, D. Sexton, D. Dudgeon
5d. PROJECT NUMBER
NREL/TP-5100-47764
5e. TASK NUMBER
BB07.2410
5f. WORK UNIT NUMBER
7. PERFORMING ORGANIZATION NAME(S) AND ADDRESS(ES)
National Renewable Energy Laboratory
1617 Cole Blvd.
Golden, CO 80401-3393
8. PERFORMING ORGANIZATION
REPORT NUMBER
NREL/TP-5100-47764
9. SPONSORING/MONITORING AGENCY NAME(S) AND ADDRESS(ES) 10. SPONSOR/MONITOR'S ACRONYM(S)
NREL
11. SPONSORING/MONITORING
AGENCY REPORT NUMBER
12. DISTRIBUTION AVAILABILITY STATEMENT
National Technical Information Service
U.S. Department of Commerce
5285 Port Royal Road
Springfield, VA 22161
13. SUPPLEMENTARY NOTES
14. ABSTRACT (Maximum 200 Words)
This report describes one potential biochemical ethanol conversion process, conceptually based upon core
conversion and process integration research at NREL. The overarching process design converts corn stover to
ethanol by dilute-acid pretreatment, enzymatic saccharification, and co-fermentation. Building on design reports
published in 2002 and 1999, NREL, together with the subcontractor Harris Group Inc., performed a complete review
of the process design and economic model for the biomass-to-ethanol process. This update reflects NREL’s current
vision of the biochemical ethanol process and includes the latest research in the conversion areas (pretreatment,
conditioning, saccharification, and fermentation), optimizations in product recovery, and our latest understanding of
the ethanol plant’s back end (wastewater and utilities). The conceptual design presented here reports ethanol
production economics as determined by 2012 conversion targets and “nth-plant” project costs and financing. For the
biorefinery described here, processing 2,205 dry ton/day at 76% theoretical ethanol yield (79 gal/dry ton), the ethanol
selling price is $2.15/gal in 2007$.
15. SUBJECT TERMS
cellulosic ethanol; production economics; process simulation
16. SECURITY CLASSIFICATION OF: 17. LIMITATION
OF ABSTRACT
UL
18. NUMBER
OF PAGES
19a. NAME OF RESPONSIBLE PERSON
a. REPORT
Unclassified
b. ABSTRACT
Unclassified
c. THIS PAGE
Unclassified 19b. TELEPHONE NUMBER (Include area code)
Standard Form 298 (Rev. 8/98)
Prescribed by ANSI Std. Z39.18
