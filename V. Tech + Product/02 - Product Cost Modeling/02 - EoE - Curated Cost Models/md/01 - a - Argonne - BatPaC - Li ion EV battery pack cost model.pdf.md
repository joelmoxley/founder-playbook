Here's an example of a description that appears under a link.

15 MIN READ || Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Credit: [Argonne National Laboratory](https://www.anl.gov/)

{! search-content: !}


Argonne National Laboratory

Modeling the Performance and Cost of Lithium-Ion Batteries for Electric-Drive Vehicles
SECOND EDITION
Chemical Sciences and Engineering Division
ANL-12/55




About Argonne National Laboratory
Argonne is a U.S. Department of Energy laboratory managed by UChicago Argonne, LLC under contract DE-AC02-06CH11357. The Laboratory’s main facility is outside Chicago, at 9700 South Cass Avenue, Argonne, Illinois 60439. For information about Argonne and its pioneering science and technology programs, see www.anl.gov.

Availability of This Report
This report is available, at no cost, at http://www.osti.gov/bridge. It is also available on paper to the U.S. Department of Energy and its contractors, for a processing fee, from:
U.S. Department of Energy 
Offce of Scientifc and Technical Information
P.O. Box 62
Oak Ridge, TN 37831-0062
phone (865) 576-8401
fax (865) 576-5728
reports@adonis.osti.gov

Disclaimer
This report was prepared as an account of work sponsored by an agency of the United States Government. Neither the United States Government nor any agency thereof, nor UChicago Argonne, LLC, nor any of their employees or offcers, makes any warranty, express or implied, or assumes any legal liability or responsibility for the accuracy, completeness, or usefulness of any information, apparatus, product, or process disclosed, or represents that its use would not infringe privately owned rights. Reference herein to any specifc commercial product, process, or service by trade name, trademark, manufacturer, or otherwise, does not necessarily constitute or imply its endorsement, recommendation, or favoring by the United States Government or any agency thereof. The views and opinions of document authors expressed herein do not necessarily state or reﬂect those of the United States Government or any agency thereof, Argonne National Laboratory, or UChicago Argonne, LLC.



Modeling the Performance and Cost of Lithium-Ion Batteries for Electric-Drive Vehicles
SECOND EDITION
by
P.A. Nelson, K.G. Gallagher, I. Bloom, and D.W. Dees
Electrochemical Energy Storage Theme
Chemical Sciences and Engineering Division
Argonne National Laboratory
December 2012



This Page Intentionally Left Blank
iii
TABLE OF CONTENTS
LIST OF FIGURES ........................................................................................................ viii
LIST OF TABLES ............................................................................................................ xi
ABBREVIATIONS ......................................................................................................... xii
LIST OF SYMBOLS ...................................................................................................... xiv
ACKNOWLEDGEMENTS .......................................................................................... xviii
PREFACE TO THE SECOND EDITION ...................................................................... xix
EXECUTIVE SUMMARY ..............................................................................................xx
1. Introduction .....................................................................................................................1
2. Battery and Cell Design Format .....................................................................................3
2.1 Cell Design.........................................................................................................4
2.2 Module Design ..................................................................................................7
2.2.1 Modules Using Liquid Thermal Management....................................7
2.2.2 Modules Using Air Thermal Management .........................................7
2.3 Battery Pack Design ..........................................................................................8
2.3.1 Batteries Using Liquid Thermal Management....................................8
2.3.2 Batteries Using Air Thermal Management.......................................10
3. Modeling of Battery Design and Performance .............................................................13
3.1 Criteria for Power, Energy, and Life ..............................................................13
3.2 Voltage at Rated Power ..................................................................................15
3.3 Governing Equations ......................................................................................21
3.4 Calculation of the ASI ....................................................................................22
3.4.1 Current Collection Resistance ..........................................................24
iv
3.4.2 Potential and Current Distribution ...................................................26
3.4.3 Determination of Module Terminal Size ..........................................28
3.5 Calculation of Battery Dimensions .................................................................29
3.5.1 Cell Dimensions ...............................................................................29
3.5.2 Module Dimensions .........................................................................30
3.5.3 Battery Pack Dimensions .................................................................30
3.6 Maximum Electrode Thickness .......................................................................30
4. Thermal Management ...................................................................................................37
4.1 Heat Generation Rates in the Battery Pack during Driving ............................37
4.2 Heating under Adiabatic Conditions ...............................................................43
4.3 Active Thermal Management Systems ...........................................................43
4.3.1 Thermal Management with Ethylene-Glycol/Water Solution ..........44
4.3.2 Thermal Management with Cabin Air ..............................................50
4.4 Cooling and Heating Required to Maintain Pack Temperature ......................51
4.5 Heat-up from Cold Ambient Conditions .........................................................52
5. Modeling of Battery Pack Manufacturing Cost ............................................................53
5.1 Approach .........................................................................................................53
5.2 Materials Costs and Purchased Items .............................................................54
5.2.1 Battery Specific Materials Cost .......................................................54
5.2.2 Purchased Items Cost .......................................................................59
5.2.3 Pack Integration Cost .......................................................................59
5.3 Baseline Manufacturing Plant .........................................................................62
5.3.1 Receiving and Shipping ...................................................................63
v
5.3.2 Electrode Materials Preparation .......................................................65
5.3.3 Electrode Coating .............................................................................65
5.3.4 Calendering ......................................................................................66
5.3.5 Inter-Process Materials Handling ....................................................66
5.3.6 Electrode Slitting .............................................................................67
5.3.7 Final Electrode Drying .....................................................................67
5.3.8 Control Laboratory ...........................................................................67
5.3.9 Cell Stacking ....................................................................................68
5.3.10 Current Collector Welding .............................................................68
5.3.11 Enclosing Cell in Container ...........................................................68
5.3.12 Electrolyte Filling and Cell Sealing ...............................................69
5.3.13 Dry Room Management .................................................................69
5.3.14 Formation Cycling, Final Cell Sealing, etc ....................................69
5.3.15 Module and Battery Assembly .......................................................70
5.3.16 Rejected Cell and Scrap Recycle ...................................................71
5.3.17 Baseline Plant Summary ................................................................72
5.4 Adjustment of Costs for Rates ........................................................................72
5.5 Plant Investment Costs ....................................................................................75
5.6 Unit Costs for Battery Pack ............................................................................75
5.6.1 Variable Costs ..................................................................................75
5.6.2 Fixed Expenses ................................................................................76
5.6.3 Profits ...............................................................................................77
5.6.4 Battery Pack Warranty Costs ...........................................................77
vi
5.7 Summary of Baseline Battery Cost .................................................................77
5.8 Uncertainties in Price Estimates .....................................................................80
5.8.1 Materials and Capital Equipment......................................................80
5.8.2 Electrode Thickness..........................................................................80
5.8.3 Cell Capacity.....................................................................................81
5.8.4 Example of Contribution to Calculated Uncertainty ........................81
5.9 Breakdown of Costs ........................................................................................82
6. Description of Spreadsheet Model and Instructions for Use ........................................87
6.1 Background .....................................................................................................87
6.2 Instructions ......................................................................................................87
6.2.1 Enabling Calculation ........................................................................87
6.2.2 Chem Worksheet ..............................................................................87
6.2.3 Battery Design Worksheet ...............................................................87
6.2.4 Remaining Worksheets ....................................................................92
6.3 Battery Design Format Requirements .............................................................95
6.4 Troubleshooting and General Advice .............................................................95
6.5 Suggested Number of Cells, Modules, and Performance Inputs ....................96
6.6 Entering a New Material Couple .....................................................................96
6.7 Entering Parallel Cell, Module, or Pack Configurations .................................98
7. Illustrated Results ..........................................................................................................99
7.1 Number of Cells in Series ...............................................................................99
7.2 Cathode Materials ..........................................................................................100
7.3 Parallel-Connected Cell Groups and Electrode Thickness ...........................100
vii
7.4 Manufacturing Scale ......................................................................................102
8. Statement of Copyright ...............................................................................................105
References .......................................................................................................................106
Appendix A: BatPaC v1.0 Variation Study ....................................................................111

viii
LIST OF FIGURES
2.1 Cell sandwich inside of prismatic pouch cells ....................................................................4
2.2 Coated current collector foil for prismatic electrodes .........................................................5
2.3 Prismatic cell in stiff pouch container with aluminum conduction channel added for heat rejection from a liquid cooled module.................................................................................6
2.4 Provision for cooling cells with cabin air ............................................................................6
2.5 Module with hermetically sealed aluminum container for batteries utilizing a liquid thermal management approach ............................................................................................7
2.6 Module using air heat transfer fluid with polymer container open at top and bottom.........8
2.7 Insulated battery jacket with enclosed modules that are exposed on their upper and lower surfaces to an ethylene glycol-water heat transfer fluid ......................................................9
2.8 Battery pack utilizing air thermal management approach. ...............................................10
3.1. Summary flow of the design model ..................................................................................14
3.2 a) Required change in [V/U] to maintain rated power with increases in internal resistance over the life of the battery. b) Increase in current due to lowered [V/U] .........17
3.3 Change in heat rejection requirement from increases in resistance for batteries with different designed voltages at rated power .......................................................................18
3.4 Efficiencies for batteries designed to achieve rated power at different fractions of their open-circuit voltage ..................................................................................................20
3.5 The change in current and potential within the positive and negative foils. The current collection design results in a uniform current distribution along the length of the foil ....27
3.6 Cell capacity simulated at the C/1 and C/3 rate as a function of electrode thickness (loading) for NCA-Gr. .......................................................................................................33
3.7 Normalized electrolyte salt concentration at the end of discharge at the C/1 and C/3 discharge rates. ..................................................................................................................33
3.8 Calculated ASI from a simulated 10-s, 5C discharge pulse for the NCA-Gr cell couple at 60% SOC. .........................................................................................................................34
3.9 The potential of the negative electrode versus a hypothetical lithium reference electrode located in the center of separator during a 5C charge pulse for the NCA-Gr couple ........35
ix
4.1 Plot comparing the estimated resistance to heat transfer from the cell center to the cooled surface of the module to that calculated by the FlexPDE model ..........................46
4.2 Heat transfer from the module wall to the laminar flow heat transfer fluid. The temperature profile of the fluid is shown at different lengths down the path. ..................47
4.3 Temperature profile in the heat transfer fluid for various fractions of the dimensionless path length..........................................................................................................................49
4.4 Correlation of model simulation results relating the Graetz number and mean Nusselt number for laminar flow between an insulated surface and the module casing ................49
5.1 Metal ingot cost contribution to the current collector foils over a 20 year period ............58
5.2 Baseline lithium-ion battery manufacturing plant schematic diagram .............................63
5.3 Breakdown of installed capital equipment costs for the baseline plant ............................74
5.4 Breakdown of unit costs for baseline battery with total price to OEM of $2528 .............79
5.5. Effects of electric-vehicle range on price and error bars for battery pack with NMC441–Gr cell chemistry, 120-kW 360 V......................................................................................82
5.6 Overall distribution of costs of manufacturing battery packs, not including pack integration system ..............................................................................................................83
5.7 Distribution of materials and purchased items for the battery pack ..................................84
5.8 Distribution of overhead costs to materials, purchased items, and individual processes ..85
5.9 Redistribution of costs to basic cost factors.......................................................................86
6.1 Iteration must be enabled for the spreadsheet model to function .....................................88
6.2 The specific cell chemistry for the battery design is selected on the Chem worksheet ....88
6.3 Chem worksheet ................................................................................................................89
6.4 Top portion of Battery Design worksheet .........................................................................90
6.5 Middle portion of Battery Design worksheet ....................................................................91
6.6 Bottom portion of Battery Design worksheet ...................................................................93
6.7 Summary of Results worksheet ........................................................................................94
7.1 The effect of the number of cells for NMC441-Gr, 60-kW, PHEV20 packs with 8 kWh total energy (70% useable) ................................................................................................99
7.2 Mass and volume of electric vehicle battery packs with lithium iron phosphate (LFP), lithium manganese-spinel (LMO) and lithium nickel-manganese-cobalt oxide (NMC441) positive electrodes versus graphite designed to deliver 150 kW of power at 360 V (20% SOC). ..............................................................................................................................101
7.3 Total battery cost to OEM for LFP-Gr, LMO-Gr and NMC441-Gr battery packs for same designs as in Fig. 7.2. NMC441-Gr and LMO-Gr result in nearly the same price..........101
7.4 Battery pack cost as a function of number of parallel cells and for different maximum electrode thicknesses........................................................................................................103
7.5 The effects of manufacturing rate on the price calculated by the model for battery packs of various cell chemistries, power capabilities and vehicle types ..................................104


LIST OF TABLES
3.1 Criteria for designing batteries for a specific end-use application ....................................13
3.2 The effect of electrode loading on the price of a 17 kWh NCA-Gr PHEV40 battery with 96 cells ..........................................................................................................36
4.1 Energy Requirements for EREV Midsize 40AER ............................................................39
4.2 Comparison for calculated heat generation by Autonomie and BatPaC ...........................42
4.3 Sample calculations of composite thermal conductivities of cell structures across layer and parallel to layers .....................................................................................45
4.4 Range of parameter values for calculating heat transfer rates in FlexPDE model ...........45
5.1 Details of stated costs for cathodes, anodes, electrolyte, and separator ...........................55
5.2 Cost equations for purchased items ..................................................................................59
5.3 Costs to integrate battery pack into vehicle drivetrain.......................................................60
5.4 Summary table of the baseline plant .................................................................................64
5.5 Materials yields during electrode and cell fabrication ......................................................71
5.6 The effect of processing rate (R) on cost for various scale factors ...................................73
5.7 Battery pack manufacturing investment costs ..................................................................75
5.8 Unit cost of battery pack ...................................................................................................76
5.9 Summary of results for cost of baseline battery and that of similar batteries with double the power and double the capacity of the baseline battery ....................................78
5.10 Table for converting overhead costs back to their origins.................................................85
6.1 General suggestions for range of input parameters that change with battery type ...........96
xi


xii
ABBREVIATIONS
ASI area specific impedance
BOL beginning of life
DMC dimethyl carbonate
EC ethylene carbonate
EG/W ethylene-glycol/water heat transfer fluid
EMC ethyl methyl carbonate
EOL end of life
EV electric vehicle
Gr graphite
GSA General, Sales, and Administration
HEV hybrid electric vehicle
HEV-HP high-power assist hybrid electric vehicle
LCO lithium cobalt oxide
LFP lithium iron phosphate
Li lithium
Li-ion lithium-ion
LMO lithium manganese spinel
LMR lithium and manganese rich
LTO lithium titanate spinel
microHEV micro or mild power assist hybrid electric vehicle
MW molecular weight
NCA lithium nickel cobalt aluminum oxide
xiii
NMC lithium nickel manganese cobalt oxide
NMP N-Methyl-2-pyrrolidone
OCV open-circuit voltage
OEM original equipment manufacturer
PE polyethylene
PET polyethylene terephthalate
PHEV plug-in hybrid electric vehicle
PP polypropylene
R&D research and development
SOC state of charge
USGS United States Geological Survey
xiv
LIST OF SYMBOLS
Section 3, 4 and 6
a ratio of interfacial area to electrode volume, cm-1
Apos area of the positive electrode, cm2
Aterm area of the terminal, cm2
ASIenergy area specific impedance for energy, ohm cm2
ASIpower area specific impedance for power, ohm cm2
C cell capacity, Ah.
C1 parameter
Cpspecific heat capacity, J/g K
dH hydraulic radius, cm
e battery to wheels efficiency
E total energy, Wh
E  energy usage rate, Wh/mile
fPd vehicle drag factor, kW/mph3
fPf rolling friction factor, kW/mph
F Faraday constant, 96485.3 C/mol
G mass flowrate, g/s
h heat transfer coefficient, W/cm2 K
Hj height of j, cm
H/W aspect ratio of pouch cell
io exchange current density related to the interfacial area, A/cm2
I average current density, A/cm2
Ilimionic ionic limiting current density, A/cm2
xv
In local current density, A/cm2
Itotal total current density, A
k thermal conductivity, W/cm K
lj length of j, cm
Lj thickness of j, cm
mj mass of j, g
n parameter
Nj number of j
[N/P] negative to positive capacity ratio
P battery power, W
Pbatt maximum designed battery power (rated power), W
Pa accessory power, kW
Pd aerodynamic drag power, kW
Pf rolling friction power, kW
Ps battery power to sustain speed S, kW
q heating rate, W
Q specific capacity of the electrode, mAh/g
rC C-rate, h-1
rC,lim limiting C-rate, h-1
rj radius of j, cm
R universal gas constant, 8.3144 J/mol K
Rj resistance of j, ohm
S vehicle speed, mph
xvi
t time, s
T temperature, K
Uocv,P open-circuit voltage at SOC for power, V
Uocv,E open-circuit voltage at SOC for energy, V
v square root of dimensionless exchange current
Vcell cell voltage, V
[V/U] fraction of the open-circuit voltage
Wj width of j
x Cartesian coordinate, cm
X
comp compression factor
α constant, ohm cm3
β constant, ohm cm2
εact volume fraction of active material
η1st first cycle efficiency
µ fluid viscosity, g/cm s
Φ1,k metal potential of foil k, V
ρj density of j, g/cm3
σj conductivity of j, S/cm
Section 5.1
C final cost of lithiated oxide, $/kg
Ci cost of raw material for component i, $/kg
Co baseline cost of lithiated oxide, $/kg
xi molar stoichiometry of component i
xvii
MWi molecular weight of component i, g/mol
MW molecular weight of lithiated compound, g/mol
Section 5.4
C capital cost of an installed equipment for the designed battery, $
Co capital cost of an installed equipment for the baseline plant battery, $
p power factor
R designed battery processing rate for specific process step
Ro baseline plant processing rate for specific process step


xviii
ACKNOWLEDGEMENTS
Support from the Vehicle Technologies Program, Hybrid and Electric Systems, initially under Tien Duong and now David Howell, at the U.S. Department of Energy, Office of Energy Efficiency and Renewable Energy, is gratefully acknowledged. The submitted manuscript has been created by UChicago Argonne, LLC, Operator of Argonne National Laboratory (“Argonne”). Argonne, a U.S. Department of Energy Office of Science laboratory, is operated under contract no. DE-AC02-06CH11357. The U.S. Government retains for itself, and others acting on its behalf, a paid-up nonexclusive, irrevocable worldwide license in said article to reproduce, prepare derivative works, distribute copies to the public, and perform publicly and display publicly, by or on behalf of the Government. We especially thank Danilo Santini of Argonne’s Transportation R&D Center for his support and suggestions in carrying out this study. Ralph Brodd reviewed our baseline plant and made several suggestions which we have incorporated in the present design. Fritz Kalhammer and Haresh Kamath of the Electric Power Research Institute have reviewed our work over several years and made suggestions that resulted in improvements. We also thank the many industrial partners that privately reviewed our work resulting in a much improved final product. The work was done under the direction of Dennis Dees and Gary Henriksen of Electrochemical Energy Storage who provided guidance in carrying out the work and preparing this manuscript.


xix
PREFACE TO THE SECOND EDITION
The BatPaC model and report were first openly distributed to the public, free of charge, in November 2011 from the website www.cse.anl.gov/batpac. During the first year of release, over 450 independent downloads have occurred from leading universities, laboratories and companies around the world. Users of the model include PhD students, policy makers, high-profile startups, and Fortune 500 corporations. Some have modified the model for their own use, while others use it as is.
The major updates included in BatPaC v2.1 include the following:
* Air-based thermal management option
* Automatic calculation of uncertainty in point cost estimate
* Updated transition metal based cathode material costs
* Parallel pack and module option
* Improved heat generation estimation
* Multiple cost-breakdown formats
Currently, the calculations are based in a Microsoft® Office Excel spreadsheet. Instructions are provided for use; however, the format is admittedly not user-friendly. A parallel development effort has created an alternate version, the Battery Production Model (BatPro), based on a graphical user-interface that will be more intuitive to some users. BatPro is available from the Argonne software shop for a nominal fee.

xx
EXECUTIVE SUMMARY
This report details the Battery Performance and Cost model (BatPaC) developed at Argonne National Laboratory for lithium-ion battery packs used in automotive transportation. The model designs the battery for a specified power, energy, and type of vehicle battery. The cost of the designed battery is then calculated by accounting for every step in the lithium-ion battery manufacturing process. The assumed annual production level directly affects each process step. The total cost to the original equipment manufacturer calculated by the model includes the materials, manufacturing, and warranty costs for a battery produced in the year 2020 (in 2010 US$). At the time this report is written, this calculation is the only publically available model that performs a bottom-up lithium-ion battery design and cost calculation. Both the model and the report have been publically peer-reviewed by battery experts assembled by the U.S. Environmental Protection Agency. This report and accompanying model include changes made in response to the comments received during the peer-review.
The purpose of the report is to document the equations and assumptions from which the model has been created. A user of the model will be able to recreate the calculations and perhaps more importantly, understand the driving forces for the results. Instructions for use and an illustration of model results are also presented. Almost every variable in the calculation may be changed by the user to represent a system different from the default values pre-entered into the program. 
The distinct advantage of using a bottom-up cost and design model is that the entire power-to energy space may be traversed to examine the correlation between performance and cost. The BatPaC model accounts for the physical limitations of the electrochemical processes within the battery. Thus, unrealistic designs are penalized in energy density and cost, unlike cost models based on linear extrapolations. Additionally, the consequences on cost and energy density from hanges in cell capacity, parallel cell groups, and manufacturing capabilities are easily assessed with the model. New proposed materials may also be examined to translate bench-scale values to the design of full-scale battery packs providing realistic energy densities and prices to the original equipment manufacturer.


1
1. Introduction
The recent penetration of lithium-ion (Li-ion) batteries into the vehicle market has prompted interest in projecting and understanding the costs of this family of chemistries being used to electrify the automotive powertrain. The model described here-in is a calculation method that was developed at Argonne National Laboratory (Argonne) for estimating the manufacturing cost and performance of Li-ion batteries for electric-drive vehicles including hybrid-electrics (HEV), plug-in hybrids (PHEV), and pure electrics (EV). To date, a number of cost models of various levels of detail have been published in different forms.1-11 The cost of a battery will change depending upon the materials chemistry, battery design, and manufacturing process.12-14 Therefore, it is necessary to account for all three areas with a bottom-up cost model. Other bottom-up cost models exist but are not generally available and have not been explicitly detailed in a public document. The motivation for this work is based on a need for a battery cost model that meets the following requirements:
1. Open and available to the entire community
2. Transparent in the assumptions made and method of calculation
3. Capable of designing a battery specifically for the requirements of an application
4. Accounts for the physical limitations that govern battery performance
5. Based on a bottom-up calculation approach to account for every cost factor
The Battery Performance and Cost model (BatPaC) described here-in is the product of long-term research and development at Argonne. Over a period of years, Argonne has developed methods to design Li-ion batteries for electric-drive vehicles based on modeling with Microsoft® OfficeExcel spreadsheets.12-20 These design models provided all the data needed to estimate the annual materials requirements for manufacturing the batteries being designed. This facilitated the next step, which was to extend the effort to include modeling of the manufacturing costs of the batteries. In the following sections of this document, a model is presented that meets the above criteria and may be used to analyze the effect of battery design and materials properties on the cost of the final battery pack. Use of BatPaC requires some basic knowledge of battery packs; however, a user does not need to be an expert. For instance, the number of cells and thus battery pack voltage must be specified by the user. However, default values are available for more specific requirements such as experimentally measured values. In this way, a person with reasonable knowledge of batteries may be able to conduct cost comparisons and “what if” studies.
The battery pack design and cost calculated in BatPaC represent projections of a 2020 production year and a specified level of annual battery production, 20,000-500,000. As the goal is to predict the future cost of manufacturing batteries, a mature manufacturing process is assumed. The model designs a manufacturing plant with the sole purpose of producing the battery being modeled. The assumed battery design and manufacturing facility are based on common practice today but also assume some problems have been solved to result in a more efficient production process and a more energy dense battery. Our proposed solutions do not have to be the same methods used in the future by industry. We simply assume the leading battery manufacturers, those having successful operations in the year 2020, will reach these ends by some means.

2
Establishing the validity of the model calculation is important in justifying the conclusions drawn from exercising the model. The report and model have been subjected to a public peer review by battery experts assembled by the U.S. Environmental Protection Agency. Changes have been made in response to the comments received during the peer-review. The design methodology used has been previously validated against cylindrical wound cell formats.15 The calculated materials quantities agreed with the actual values within 3 %. Moving to a prismatic format simplifies the current collection calculation while leaving the governing equations unchanged. The new approach developed for calculating the cell impedance has been validated against experimental measurements from electrodes up to 100 m in thickness.20 The module and battery jacket construction is of lighter construction compared to contemporary designs. The battery pack energy density calculated in BatPaC is higher than the battery packs used in the first versions of the Nissan Leaf and Chevrolet Volt for equivalent cell designs (calculated value of 100 Wh/kg compared to a reported value near 84 Wh/kg for the Volt21). Significant engineering advances are necessary to minimize the current inactive material burden in the commercial pack designs, thereby reducing the cost, mass and dimensions of future automotive battery packs. We have assumed a design that we believe will be representative of the engineering progress achieved by successful manufacturers in the year 2020.
Validation of the input material and capital costs are more difficult to achieve as few values are ublically available. We have relied, to a large extent, on private communications from equipment manufacturers, materials suppliers, cell manufacturers, and original equipment manufacturers (OEM). Variation does exist amongst the communicated values and we have maintained a practical level of skepticism for their accuracy. Experts from all aspects of battery development have reviewed the model both privately and as part of a formal peer-review process. While the largest uncertainty in calculated values will exist in point cost estimates, themost instructive information may be gained by examining ranges in parameter values and  relative changes between material properties (e.g. the advantage of moving to a manganese spinel cathode from a layered-oxide material or from increases in cell capacity, etc). An initial variation study may be found in Appendix A.
The battery pack price to the OEM calculated by the model inherently assumes the existence of mature, high-volume manufacturing of Li-ion batteries for transportation applications. Therefore, the increased costs that current manufacturers face due to low scale of production, higher than expected cell failures in the field, and product launch issues are not accounted for in the calculation. The model results for year 2020 could be considered very optimistic if the transportation Li-ion market fails to develop as a result of insufficient investment in product research and development, reduced motivation for lowering petroleum consumption and greenhouse gas emissions, and/or a series of high-profile safety incidents.


3
2. Cell and Battery Pack Design Format
Various cell and battery design concepts are under development at battery manufacturers. Based upon experience gained from extensive previous work, we have found the exact design of the battery does not have an important effect on the cost for a set cell chemistry system; the amounts of electrode materials and the number, capacity and electrode area of the cells, are the determining cost factors. The most common cell designs for batteries nearing large-scaleproduction are cylindrical wound cells, flat wound cells, and prismatic cells with flat plates. Cylindrical cells probably have a slight advantage for the assembly of the electrode-separator unit because of the ease of making a cylindrical winding. For the different cell designs, there are small differences in the weights of the terminal extensions and the procedures for connecting these extensions to the current collector sheets, with a small advantage for flat plate cells. The flat-wound and flat-plate cells form a more compact module and have better heat rejection capabilities than the cylindrical cells. These small differences would have minor effects on the cost of batteries produced in high volume in a mature, automated production plant and all of the cell designs can be adequately cooled for most applications. We conclude that the cost calculations would be relevant for batteries differing considerably from the selected design approach.
To provide a specific design for the calculations, a prismatic cell in a stiff-pouch container was selected. The terminals are almost as wide as the full width of the cell with the positive terminal at one end of the cell and the negative terminal at the opposite end. The electrical performance of a cell with this construction is near optimum, with a very low fraction of the resistance in the current collection structure. This cell design is amenable to either liquid or air based thermal management approaches. In this study, most of our attention has been directed to batteries using liquid thermal management. For that approach, the cells are enclosed in hermetically sealed modules, which are cooled on their exterior surfaces by ethylene glycol-water solution. The module enclosure protects the cell terminals from the heat transfer fluid, which is an electrolyte. As an additional safety precaution, a dielectric liquid could be used as the heat transfer fluid, such as a transformer coolant, but that approach has not been studied in the work of this report.
For air thermal management, the broad cell area must be individually contacted by the fluid due to the poorer heat transfer properties of air. Therefore, the cells are enclosed in an aluminum sleeve which provides air flow channels; the module enclosure is open at the bottom and top to accommodate upward flow of air through these channels. Both the liquid and the air thermal anagement designs are configured to be compact, light-weight and amenable to low-cost manufacture. It is unlikely that we have selected the most viable designs in this short study; there may be serious flaws in some details. However, the calculated overall performance and low cost for the selected design will be challenging to match in actual production and will only be met by the most successful manufacturers, those that will dominate the market.
The paragraphs below in section 2, provide the overall cell, module and battery pack design formats. Additional design details and methods of calculations are provided in sections 3 and 4.


4
2.1 Cell Design
The prismatic cell of this design embodies individual positive and negative electrodes consisting of current collector foils coated with electrode materials on both sides. The current collectors are usually solid copper and aluminum foils for the positive and the negative. An illustration of a segment of the cell is detailed in Figure 2.1. Each electrode is made up of active material particles held together by a polymeric binder. A conductive additive, carbon black and/or graphite, is added to the positive electrode and sometimes to the negative electrode. The electrodes and separator each have porosity that is filled with the electrolyte solution. During discharge, the Li-ions move from the electrode particles into the electrolyte, across the separator, and then insert into the particles composing the opposite electrode. The electrons simultaneously leave the cell through the current collection system and then enter through the opposite side after doing external work. The materials currently used in Li-ion cells are based on an intercalation process. In this process, the Li-ion is inserted into or removed from the crystal structure of the active material. The oxidation state of the active material, or host, is concurrently changed by gaining or losing an electron. Other electrode materials based on conversion reactions or electrodeposition could be implemented into the model if the user desired.

The electrodes are easily and efficiently prepared by coating wide sheets of foil up to 2-meters in width with uncoated strips running the lengths of the foil being coated. The individual electrodes can be cut from these sheets with little waste of electrode coating material or foil (Fig. 2.2). 

The separator for these cells can be handled as a single sheet that is folded back and forth as the electrodes are inserted. The electrodes are inserted so that all of the positive tabs extend beyond the separator sheet in one direction and the negative tabs extend in the opposite direction. The design model selects the number of electrodes to meet a set cell thickness determined by the type of cell: HEV, 6 mm; PHEV, 8 mm; EV, 12 mm. These cell thicknesses are default values and may be changed to suit the designer. 

Figure 2.1. Cell sandwich inside of prismatic pouch cells.
separator
negative
electrode
+ – +
Li+
positive
electrode
e-


The stiff-pouch containment for the cell and the terminal seal is illustrated in Fig. 2.3. The cell terminals are formed from flat stock to be almost as wide as the entire cell. They are bent to the required shape and ultrasonically welded to the current collector tabs. The cell stack is then sealed between the two halves of the cell container. The cell housing material is a tri-layer consisting of an outer layer of polyethylene terephthalate (PEP) for strength, a middle layer of 0.1-mm aluminum for stiffness and impermeability to moisture and electrolyte solvent vapors and an inner layer of polypropylene (PP) for sealing by heating.18,19 The two halves of the cell container are pre-shaped to facilitate assembly. The aluminum foil in the cell container material provides stiffness and it may be increased in thickness to assist in conducting heat to the module container. After sealing the edges of the cell, the edges are flattened along the sides of the cell to form a compact shape. For liquid based thermal management, an aluminum conduction channel is added to assist in heat rejection at the sides of the cells (Fig. 2.3).

Figure 2.2. Illustration of coated current collector foil showing four rows of prismatic electrodes before slitting or stamping into individual electrodes

Electrode Coating
Lines Showing Places to Cut for Electrodes
Uncoated Area for CC Tabs

For batteries utilizing air based thermal management, the cell design format is the same as for liquid-based systems. To provide space for air flow between the cells, the cells are enclosed in an aluminum sleeve that provides the flow passages as illustrated in Fig. 2.4. The ridges between the air flow passages are 2-mm wide. The passages themselves are about 10-mm wide, the exactwidth being calculated to provide an integer number of passages across the length of the positive  electrode.


6
Figure 2.3. Prismatic cell in stiff pouch container with aluminum conduction channel added for heat rejection from a liquid cooled module
Figure 2.4. Provision for cooling cells with cabin air 
Cell with Stiff, Multi Layer Container
Terminal Seal
Polymer Seal of Cell Container to Terminal
Ultrasonic Welds of Terminal to Collector Foils
Cell Cross-Sections
After Edge Sealing
After Edge Shaping and Addition of Aluminum Conduction Channel
Aluminum Conduction Channel
6 mm
2 mm
̴10-20 mm
Aluminum Cell Sleeve Providing Channels for Air Flow


2.2 Module Design
2.2.1 Modules Using Liquid Thermal Management
The module format is based on a casing of 0.5-mm thick aluminum that is sealed by double seaming, a process that is well established and inexpensive because it is automated, rapid, and uses low-cost equipment that is common in the container industry. The sealing of the module provides an additional barrier to the loss of electrolyte solvent from the cells and the entrance of water vapor. These deleterious transfers through the seals of pouch cells may shorten their lives to less than the desired fifteen years.18
The cells are placed on their sides in the module and the terminals of adjacent cells are connected either mechanically with rivets and flat springs to maintain contact or by laser welding. Space is provided within the module casing on the left side, as sketched in Fig. 2.5, for an electronics package that includes cell monitoring for malfunctions (temperature and voltage) and for state of-charge (SOC) control. The SOC control is activated whenever the battery is at rest and it diverts charge from the cells at highest voltage to those at lowest voltage.
Figure 2.5. Module with hermetically sealed aluminum container for batteries utilizing a liquid thermal management approach
Heat Transfer Surfaces on Top and Bottom of Container in Contact with Cell Conductors
Cell Terminal Connections
Module Terminal
Double-Seamed Module Closure
Module with Sealed Aluminum Container Designed for Liquid Cooling
2.2.2 Modules Using Air Thermal Management
For systems using air as the heat transfer fluid, the module must be open to allow air to flow between the cells utilizing a larger surface area for heat transfer (Fig. 2.6).

8
Figure 2.6. Module using air heat transfer fluid with polymer container open at top and bottom

Cell State-of Charge Controller
Polymer Strip Blocking Air Flow at Cell Terminals
Module Terminal
Cell Sleeves
Air Flow Channels

2.3 Battery Pack Design
2.3.1 Batteries Using Liquid Thermal Management
The model designs the battery pack (Fig 2.7) in sufficient detail to provide a good estimate of the total weight and volume of the pack and the dimensions of the battery jacket so that its cost can be estimated. The modules are arranged within the battery jacket either in a single row, with theterminals facing the same side of the pack, or in an even number of rows with the terminals in one row facing the terminal of an adjacent row. For a pack with a single row of modules, a busbar must be provided to carry the current to the front of the battery pack. This feature results in an additional cost for the busbar. For batteries with more than one row of modules (Fig. 2.7), the terminals are laid out in the module so as not to interfere with those on the opposite row of modules, thus conserving space in the battery pack. The modules in a row are interconnected, negative to positive terminals, by copper connectors. The modules casings are compressed together between steel sheets at each end of the battery pack. The compression force is applied by steel bands wrapped around the top and bottom of the row of modules. The compression is necessary to ensure intimate contact between the active layers that make up the pouch cells that are tightly fit into the modules. The compressive force also serves to add structural support to the module casings.
The modules are supported by a tray that positions the modules mid-way between the inside top and bottom of the pack jacket and provides space for heat transfer fluid to flow so that it cools or heats the top and bottom of each module. The rows of modules are assembled, compressed between end plates, interconnected and attached to the module tray. The module tray is attached to the pack closure at the front of the pack so that all connections to the pack terminals that lead to the exterior of the pack and signal wire feedthroughs can be made before inserting the attached modules into the jacket and making the final closure. The bolts depicted in the diagram (Fig 2.7) for making this closure are only illustrative.


9
The battery jacket consists of a sheet of aluminum on each side of a 10-mm thick layer of ridged, light-weight high-efficiency insulation. The thickness of each of the aluminum layers is selected by the modeling program to be 1- to 2-mm thick, depending on the total volume of the modules. The insulation slows the interaction of the battery with the external environment that cools the battery in the winter and heats it in the hot summer weather.13
Figure 2.7. Insulated battery jacket with enclosed modules that are exposed on their upper and lower surfaces to an ethylene glycol-water heat transfer fluid. 
Although the main purpose of the battery pack design for the model is to provide a plausible list of materials to estimate the manufacturing cost of the battery, the overall design approach permits the battery to be shaped by the designer to fit dimensional objectives. If there is a height restriction for the battery pack, a high ratio of length-to-width for the positive electrode will result in a battery of low height. Because the cell terminals are nearly as wide as the electrodes inthe cell design selected for this model, the current collector structure adds very little to the total cell impedance even for electrodes with length-to-width ratios as high as 3.0. If the cell terminals were both brought out of the same end of the cell and, therefore had to be narrow, the resistance of the terminals and of the current collector foil in the vicinity of the terminals would be high, especially for long, narrow cells. Further discussion of the means of adjusting the shapes of the modules and the pack is provided in section 7.

2.3.1 Batteries Using Air Thermal Management
The air thermal management battery format is similar to the liquid thermal management format in that the cells are the same and the modules casings are held together by steel sheets at the ends of the row of modules and compressed by steel straps. The battery pack for air thermal management differs, however, in that much more space must be allotted for air flow than for liquid flow (Fig. 2.8).
Figure 2.8 Battery pack utilizing air thermal management approach.
A
A
Section A-A
Air Flow Passages between Cells
Duct to Fan Inlet

11
Air is admitted along the entire length of the bottom of the pack to minimize the thickness of the flow passages above and beneath the modules. The air leaving the module is ducked to the inlet side of the fan, which can be located nearby to suit the vehicle design. The pack-long entrance and exit passages are insulated for thermal efficiency. These additions and the air passages between the cells and the wide passages required above and below the modules add considerable volume to air thermal management packs over that required by liquid thermal management packs. The thermal calculations described in section 4 indicate that cabin air-cooling is sufficient for HEV battery packs and for some larger battery packs, but it may limit the driving profiles that are feasible.
12

13
3. Modeling of Battery Design and Performance
The design portion of the model calculates the physical properties of a battery based on user defined performance requirements and minimal experimental data. An illustration of the model is shown in Figure 3.1. The user is asked to enter a number of design parameters such as the battery power, number of cells and modules, and target voltage at maximum power, etc. In addition, the user must enter one of the following three measures of energy: battery pack energy, cell capacity, or vehicle electric range. Defining one of these values will determine the value of the other two. An iterative procedure then solves for the user defined energy parameter (energy, capacity, or range) and remaining battery properties by varying the cell capacity and electrode thickness. The result is the dimensions, mass, volume, and materials requirements for the cells, modules, and battery pack.
The model has been designed to allow the user to enter as many customized values as desired. In this way, the model allows flexibility in the battery chemistries studied and some of the cell, module, and battery design aspects. Hence, the focus of this report is on the method of calculation and not the exact values chosen for a specific capacity or cell thickness. However, the default cell design parameters as well as experimental data measured at Argonne National Laboratory, for a number of different battery chemistries both commercial and developed at Argonne, are available for use within the model. There are five governing equations for battery performance that calculate the current density, battery energy, electrode area, electrode thickness, and resistance. The voltage at maximum power and the area specific impedance (ASI) are two important parameters in the design model for calculating the battery performance. Most of the discussion will be spent on these two properties.
3.1 Criteria for Power, Energy, and Life
In order to fully specify a battery design, the user of BatPaC must supply criteria for power, energy, and life. These criteria will depend on the application for which the battery will be used. While the users may change some of the settings as they prefer, we list our suggestions in Table 3.1. The battery type is defined by the end-use application. Hybrid electric vehicles (HEVs), plug-in hybrid electric vehicles (PHEVs), and electric vehicles (EVs) have increasing levels of electrical energy storage for use by the vehicle drivetrain. The model will use Table 3.1 or the user’s explicit inputs to size the battery correctly for the chosen application.
Table 3.1 Criteria for designing batteries for a specific end-use application
Battery Type microHEV HEV-HP PHEV EV
SOC for Rated Power, % 50 50 20 20
Power Duration, sec 2 10 10 10
SOC Range for Useable Energy, % 40-65 40-65 20-90 10-95
Cell Thickness, mm 6 6 8 12
The microHEV is a micro or mild-hybrid that provides a moderate power level, ~25 kW, for two seconds. This design is best suited for cell chemistries capable of very high power-to-energy (P/E) ratios. The HEV-HP is a power-assist hybrid that provides the rated power for a full 10 second pulse. The power for both HEV applications is rated at 50 % state-of-charge (SOC). The energy available for discharge and charging is 25 % of the total energy to ensure long cycle life. As the capacity of the HEV cells is typically small, a cell thickness of 6 mm is used. The PHEV utilizes a much larger portion of the total energy, 70 %. At the end of discharge, the PHEV battery is operated in a charge sustaining mode. Therefore, the power rating for the battery is determined at 20 % SOC. PHEV cells should be much larger than HEV cells and thus a cell thickness of 8 mm is assumed. Finally, EV batteries use 85 % of their total energy with their power rated near the end of discharge. EV cell thicknesses are set to 12 mm.
14
Figure 3.1 Summary flow of the design model

15
As noted later in the report, selecting a parallel arrangement of cells automatically assumes a cell thickness of 6 mm regardless of the end-use application. Additionally, the use of negative electrodes operating at potentials high above the lithium metal potential may extend the upper end of the available SOC range from 95 to 100 %. The lithium titanate spinel, Li4Ti5O12 (LTO), negative electrode is an example of an intercalation electrode with almost no risk of plating lithium metal during a charge pulse. On this basis, the available energy for LTO-based Li-ion cell is increased by 5 % to be 75 % for PHEVs and 90 % for EVs. In an established factory, the fixed design parameter is most likely the electrode area for a single layer rather than a set cell thickness. To make higher capacity cells, more layers of the predetermined footprint are stacked, thus increasing the cell thickness. In our model, the plant is constructed for the sole purpose of building the battery being designed. Flexibility to produce other products is not taken into account. Most importantly, the model calculates very little difference in cost whether the cell has large-area layers that are few in number as compared to a high number of layers smaller in area. For ease of calculation, we use a set cell thickness to determine the number of layers. The area of each layer is set by the cell capacity requirement.
Accounting for capacity and power fade in the battery requires the user to design the battery with the appropriate excess energy and power at the beginning-of-life (BOL). Achieving rated end-of life (EOL) power at a high fraction of the open-circuit voltage at BOL is one way to set the allowable power fade over the life of the battery. This is discussed in detail in the following section. Capacity or energy fade may be managed in multiple ways. The BOL SOC range for useable energy in Table 3.1 may be considered one approach to oversizing. As the battery capacity is reduced resulting from fade mechanisms, the loss in total capacity and energy is notas obvious when only cycling in the reduced SOC range. In addition, the SOC window may shift to different defined pack voltages to obtain a near constant useable energy value. Current practices by the OEMs suggest that the customer will accept some degree of capacity fade from the battery over the life of the vehicle. The Chevrolet Volt battery warranty states the capacity may fade by 10 – 30 % over the warranty period. Certainly, the customers’ previous experience with consumer electronics devices has prepared them for a reduction in battery capacity with the life of the product. However, we do not hold the same opinion on power fade. We have allotted or significant power fade by designing EOL power to be achieved at a high fraction of the open circuit voltage at BOL. The design model does not attempt to predict fade rates or even suggest an allowable fade for a specific application, other than the SOC window for useable energy. It is ur view that many aspects of materials chemistry, cell design, and battery use directly affect the decay rate of the battery pack. Hence, we allow the user to make any additional accommodations for decay believed to be necessary by entering larger total energy content than what is calculated from the useable SOC windows.
3.2 Voltage at Rated Power
The voltage at which a cell reaches the rated power is one of the most important factors in the design of a battery. However, this specification is one of the least discussed aspects of battery design. Our design approach assumes the drivetrain will never draw a power level greater than the rated power over the entire life of the battery. The voltage at rated power is a measure of the largest polarization the cell will undergo during operation at the BOL. This initial value has a direct effect on round-trip battery efficiency, heat removal requirements, cold-cranking power, and allowable power fade. A basic calculation demonstrates the maximum achievable power for a battery at BOL is at 50 % of the open-circuit voltage (OCV). Operating at these conditions would result in an inefficient battery and require a significant cooling system to reject heat. More importantly, the battery will never be able to reach this power level after any increase in impedance occurs. With all certainty, the impedance of a battery will rise with time and the power rating of the battery will no longer be accurate.

16
We design the battery to achieve EOL power capabilities (rated power) at a specified fraction of the open-circuit voltage, [V/U], at BOL. This approach is unique when compared to current design practice of OEMs and cell manufacturers. However, a characteristic value of [V/U] exists for all batteries regardless of the battery design process. One may determine this value for an existing system in a straightforward manner. The voltage at rated power is measured at the end of a 10 s pulse at the EOL power rating and the SOC used for the power rating of a specific battery type (HEV, PHEV, EV). The designed [V/U] value is the measured potential at the end of the pulse divided by the open-circuit potential reached long after the pulse. This design point then captures the degree to which the battery has been oversized to enable long-life, cold-start, and efficient operation. The remainder of this section presents a discussion for setting the BOL voltage at rated power at no less than 80 % of the open-circuit voltage, [V/U] = 0.8. Defining the voltage as a fraction of the OCV, allows for direct calculation of all the necessary battery properties (see for example Eq. 3.6 or 3.8 in the section 3.3). 
The allowable increase in battery resistance over the life of the battery is a function of the designed voltage for rated power. In general, designing the battery to achieve rated power at a higher [V/U] allows for larger resistance or impedance increases over the lifetime of the battery. Figure 3.2 created from Eq 3.1 displays how the voltage at rated power will change to meet the designed power as the internal resistance of the battery increases. Clearly, achieving BOL power at a high fraction of the OCV allows for greater degradation within the usable lifetime of a battery. R1 is the initial resistance of the battery at BOL while R2 is the resistance as the battery ages. If the minimum voltage is 55 % of the OCV, the allowable increase in resistance for batteries designed for BOL rated power at 70, 80, and 90 % OCV is 18, 55, and 175 %. The consequence of achieving the power at lower and lower fractions of the open-circuit voltage is that both electric current and heat generation will increase over the lifetime of the battery, Figure 3.2b and Figure 3.3. The proper design of a battery will account for the changes over the entire lifetime and not just desired behavior at BOL.
The level of heat production is significantly different at BOL for batteries designed to meet rated power at differing fractions of the open-circuit voltage. We may compare the differences in designed [V/U] by assuming the resistive heating (joule heating) is the most significant factor in determining the heat generation, Eq. 3.2. This assumption is true for moderate to high rate applications. We also reasonably assume the ASI will not change significantly in the range of current densities and electrode thicknesses we vary in the comparisons. We can analyze the difference in heat generation for different [V/U] values, Eq 3.3. 
17
Figure 3.2 a) Required change in [V/U] to maintain rated power with increases in internal resistance over the life of the battery. b) Increase in current due to lowered [V/U].
50
55
60
65
70
75
80
85
90
95
0 25 50 75 100 125 150 175 200
Fraction of OCV at Ratedl Power, %
Increase in Resistance, %
90%
80%
70%
Designed
BOL [V/U] at
Rated Power
0
10
20
30
40
50
60
70
80
0 25 50 75 100 125 150 175 200
Increase in Current, %
Increase in Resistance, %
90%
80%
70%
Designed
BOL [V/U] at
Rated Power




  U V    2  1 2 1 1 4 R R1 2   U V   1   1   U V   1     (3.1)
 
j
j
j
j pos j total
R
V U
U
V U
q A I R I U
2
2
2
1
1





  
 



   (3.2)
2
1
2
2
2
1
2 1
1 1
              
              

V U
R
V U
R
q q
(3.3)
0
50
100
150
200
250
300
350
400
450
500
0 25 50 75 100 125 150 175 200
Increase in Heat Generation, %
Increase in Resistance, %
90%
80%
70%
Designed
BOL [V/U] at
Rated Power

Figure 3.3 Change in heat rejection requirement from increases in resistance for batteries with different designed voltages at rated power.
18
The ratio of resistances may be found by equating the power for the two cases. Then the resistances, and areas if the ASIs are equivalent, are determined solely by the fraction of the open-circuit voltage at which they achieve rated power, Eq 3.4. Then substitution will give the Increase in Resistance, % ratio of heat production at rated power for the two cases, Eq. 3.5. A battery that achieves rated power at 80 % of OCV will have a heat production at rated power that is 2.3 times higher than one designed at [V/U] = 90 %. A battery producing power at 70 % of the OCV will have 3.9 time higher heat generation than at [V/U] = 90 %.
             
             
 
2 2
1 1
2 1
1 2
1 2
1 1
V U
V U
V U
V U
ASI A
ASI A
R R
power pos
power pos (3.4)
             
               

2 1
1 2
2 1
1 1
V U
V U
V U
V U
q q
(3.5)

19
Two different design changes would enable operating a battery at 90 % of OCV compared to 80 % while maintaining the same power output. First, a second identical battery may be connected in parallel to the original battery. This will lower the resistance of the battery pack by one half but will also double the energy and cost of the battery. A more cost-effective approach is to reduce the electrode thickness by coating a larger separator area with the same amount of active material. The capacity of the cell is maintained while minimizing increases in cost from a larger separator, current collector and packaging area. This approach is feasible as long as the reduced electrode thickness is above that at which the ASI begins to increase, which is around 20 microns for typical Li-ion electrode systems as discussed in detail below. 
The efficiency of a battery defines the heat rejection requirements and may be measured or calculated. Measurement of round-trip efficiency of a battery is best performed by using a calorimeter to measure the heat given off during the cycling of the battery. The calorimeter removes the requirement of knowing the exact SOC of a battery during the entire drive cycle. Calculation of the round-trip efficiency of a battery requires a detailed transient battery model within a vehicle simulation program to exercise the battery over the many acceleration and deceleration periods that occur during a drive cycle. The interesting result is that the same battery will have different power ratings depending on what level of round-trip efficiency the user is willing to accept.
Figure 3.4 shows the efficiency of a battery as a function of the designed potential at which the battery reaches rated power. The figure is created using Equations 3.1 and 3.4 above. Each line may be considered a different drive cycle, or duty load, for a battery with the same energy but different impedance (changing separator area). The straight, solid black line represents the efficiency of the battery operated only at rated power, P/Pmax = 1. In example, a battery designed at [V/U] = 0.8 will have 80 % efficiency for a single discharge pulse at rated power. Likewise, a battery designed at 0.9 will be 90 % efficient at rated power. Batteries are normally operated in the area above the line of the rated power. Therefore, the other curves represent the efficiency of discharging a battery at power levels below rated power (typical driving conditions). Consider two batteries each designed for a rated power of 100 kW although one achieves this power at a [V/U] = 0.9 and the other at 0.7. If the two batteries are discharged at 45 kW, P/Pmax = 0.45, the battery designed at [V/U] = 0.9 will be 6.4 % more efficient. This is significantly less than the 20 % efficiency improvement realized when operated at rated power. The efficiency penalty is reduced as the battery operates less and less near the rated power.

20
Figure 3.4 Efficiencies for batteries designed to achieve rated power at different fractions of their open-circuit voltage. Comparative efficiency lines are shown for equivalent power demands over a period of battery operation.
50%
60%
70%
80%
90%
100%
0.5 0.6 0.7 0.8 0.9 1
Efficiency During Discharge
Designed [V/U] at Rated Power
0.10
0.20
0.30
0.45
0.60
0.80
1.00


21
3.3 Governing Equations
The five coupled, algebraic equations that govern the battery design are presented in this section. While these equations are perhaps the most important, many other equations are used to fully define the battery mass and volume. These other equations will be specified where necessary in the following subsections.
The user of the model specifies the required maximum rated power, Pbatt, of the battery. This power is translated to a current density, I, in Eq 3.6 using the area of the positive electrode, Apos, the number of cells, Ncell, the open-circuit voltage at the SOC for power, Uocv,P, and the fraction of the open-circuit voltage at which the designed power is achieved, [V/U].



V U
A N U
P
I
pos cell ocv P
batt
,
(3.6)
The relationship between capacity and battery energy is described by Equation 3.7. Formally, the energy of a battery is the product of the capacity and the average voltage at which the energy is obtained. The average cell voltage is approximated in Eq. 3.7 by subtracting the polarization from discharging the battery at a C/3 rate from the open-circuit voltage at the SOC for energy, Uocv,E. The energy for all batteries designed by the model is calculated at a C/3 rate and the average open-circuit voltage at 50 % SOC. The remaining necessary values are the capacity of the cell, C, ASI for energy, ASIenergy, number of cells, and area of positive electrode. Either the battery energy or capacity may be specified. The energy may alternatively be determined from a stated range, fraction of total energy available, and energy usage rate for the vehicle (Wh/mile).


 
pos
energy
cell ocv E
A
C ASI
E N C U
, 3
(3.7)
The area of the positive electrode in Eq. 3.8 is determined largely by the area specific impedance for power, ASIpower, and resulting voltage drop. The voltage of cell at rated power, Vcell,P, is found from the product [V/U]Uocv,P, where Uocv,P is the open circuit voltage at the SOC for max power. In general, the area of the electrodes will increase if the ASI for power increases. The areas of the negative electrode and separator are determined from the area of the positive electrode. The negative electrode is taken to be 1 mm larger than the positive electrode in both height and width to alleviate concerns of lithium plating during charge pulses. The separator area is slightly larger than the negative electrode to prevent the electrical shorting of the two electrodes.
   
 
 N U U V        U V   
ASI P
A
cell ocv P
power batt
pos
2 1
,
(3.8)
The positive electrode thickness, Lpos, in Eq. 3.9 is determined from the capacity of the cell, C, specific capacity of the electrode material, Q, volume fraction of active material, εact, bulk density of the active material, ρ, and the positive electrode area. The negative electrode thickness is determined by its specific reversible-capacity and the designed excess-capacity to prevent lithium plating during charging. We have chosen a ratio of 1.25 negative to positive reversible capacity (N/P ratio) for the default value for the cells with graphite negative electrodes. LTO negative electrode based cells are designed at a 1.1 N/P ratio because of the previously mentioned minimal possibility of lithium deposition. The maximum allowable electrode thickness is a user defined value. The calculation for the electrode area changes when the designed thickness is greater than the maximum allowed (Section 3.6.1).

22
act pos
pos Q A
C
L

 (3.9)
Finally, the ASI for power (and for energy to a lesser extent) is calculated using an expression that is based on the electrode thicknesses, the current density, and the C-rate. The exact expression will be discussed in the next session. The ASI in Eq 3.10 shows the basic dependencies with α and β being constant valued parameters.
 
   
Lpos
f I
ASI (3.10)
3.4 Calculation of the ASI
In most battery design scenarios, the ASI and [V/U] directly determine the electrode thickness and area to meet a specified power-to-energy (P/E) ratio and capacity requirement. Clearly, the ASI plays a significant role in the design of a battery and particularly in the case of the P/E ratios required by automotive applications. However, the ASI is not an inherent constant of a specific battery chemistry or cell design. The measured value of the ASI is a complex combination of resistances within the battery resulting from the physical processes occurring at different length and time scales. Consequently, the measured value is a function of many factors (state of charge, pulse length, current density, C-rate, particle size, transport and kinetic parameters, etc). The calculation used for the ASI in this battery design model has been discussed in detail and validated against experiments elsewhere.20 The physical meaning of the equation will be discussed but those interested in the derivation are directed to the separate publication. We note that the ASI described here is slightly different than the one addressed in the paper. The thermodynamic component is removed that originated from the change in open-circuit potential with concentration for the intercalation materials. Equation 3.11 contains the definition of the ASI used in this document. It1 is a positive valued current density for a discharge pulse. It2 is equal to zero as it is during the relaxation period after the pulse. The subscripts are as follows: time 0, t0, is the time just before a current pulse begins, time 1, t1, is the time just before the current pulse ends, and time 2, t2, is the time long after the current pulse when the cell is at open circuit and the concentration gradients have relaxed. Therefore, this ASI measurement is not troubled by accounting for a change in open-circuit voltage with the passage of current. In general, the ASI measured with this definition is similar, although smaller, in value to those produced using the more standard definition used elsewhere.

23
1 2
2 1
t t
t t
I I
V V
ASI
 
 (3.11)
The ASI for the electrochemical charge and discharge process is referred here-in as ASIechem. Our calculation approach for both the ASI for power and for energy involves adding three components together to reach the ASIechem, Eq. 3.12. The first two factors include impedance that arises from the interfacial charge transfer and transport. The third factor is a lumped parameter used to capture the remaining impedance.
ASI echem  ASI intf pos  ASI intf neg  ASI const (3.12)
The interfacial impedance for positive and negative electrodes both contain the charge transfer resistance component R T/(ioaLF) as shown in Eq. 3.13 and 3.14. Here, io is the exchange current density related to the interfacial area and a is the ratio of interfacial area to electrode volume. An approximation often used for a relates the parameter to the volume fraction of the active material and the particle radius, a = 3εact/rp. The variables io and a should be specified to relate to the same area as they are often not independently determined. R and T correspond to the universal gas constant and absolute temperature respectively. F is Faraday’s constant. The influence of the interfacial impedance is that the ASIechem increases as the electrode thickness is reduced. This behavior is typically observed at electrode thicknesses less than 30 microns for common Li-ion battery materials.
i aL F
RT
ASI
o neg

neg
intf (3.13)
–0.5
2
lim ,lim
pos
intf 1 1






  
 
ASI  ioaL RT posF      I ionic I rCrC (3.14)
The positive electrode interfacial impedance also includes two factors that account for the physical limitations that occur from depleting the concentration of the reactants within the porous electrode. The I lim ionic term is the limiting ionic current for lithium cation transport through the porous separator. The rC,lim term is the limiting C-rate for solid state diffusion of lithium in the active materials. The C-rate may be related to the current density with Eq. 3.15. Here, the specific capacity, Q, the active material density, ρ, active material volume fraction, εact, and the electrode thickness, L, are used. If either the limiting C-rate or limiting ionic current are approached, the ASI will begin to approach an infinite value. This approach assumes the cell and material design is such that the transport limitations all occur on the positive electrode. The parameters required for the ASI expression are fit to experimental measurements. The ASI values are corrected for the interfacial contributions present during measurement so that the correct ASI may be determined at different electrode thicknesses. This is termed “ASI correction factor” on the System Selection worksheet of the spreadsheet model.

24
I  rCQ actLpos (3.15)
The cell ASI for energy, ASIenergy, and power, ASIpower, are determined by adding the ASIechem to that of the current collectors, ASIcc, as discussed in the next subsection. The difference between ASI energy and ASIpower is that the limiting currents are not important during the C/3 discharge for energy and the ASIconst is a different value for two cases. ASIenergy will always be higher than ASI power if a battery is operated far from the limiting current. The higher impedance is due to the formation of significant concentration polarizations during the longer time scale of the energy discharge. A reasonable rule-of-thumb is that the ASIconst for energy is 2.2 times the value for power in layered oxide materials such as LiNi0.80Co0.15Al0.05O2.
3.4.1 Current Collection Resistance
The resistance from the conductors used to collect the current must be accounted for as they can contribute significant ohmic drop to the battery. The ASI used to calculate the required cell separator area, ASIpower, is larger than the ASI for the electrochemical charge and discharge processes, ASIechem,P, as shown in Equation 3.16. The ASIechem value is typically measured from experiments and must be added to the external resistances that arise from the materials used to conduct the electric current. These resistances come from current collection in the cell and also those on the module and battery pack level.
cells
cell cnct pos
power echem,P cc term
N
R A
ASI  ASI  ASI  ASI  (3.16)
The current collector foil impedance, ASIcc, is determined from an analytical expression, Eq. 3.17, which accounts for the coated and uncoated region of the foil, labeled act for active and tab respectively. The resistance factor, Rf, and the resistance of the current collector foils, Rcc, are also shown for clarity in Eq 3.18 and 3.19. The factor of 2 in the Rf term is due to assuming half of the foil thickness carries the current produced on one side of the foil. While all of the current passes through the tab region, the magnitude of the current varies along the height of the coated foil as the reaction area continually contributes current to the foil. An equivalent length for the resistance calculation may be determined so that multiplication by the total current for a cell will give the correct ohmic drop. This equivalent length is H/3 if the current density is relatively constant over the entire area. The derivation of this equivalent length as well as an in-depth discussion of the voltage and current distribution in the foils may be found in subsection 3.4.2. Also in the later subsection, the assumption of constant current density is verified with numerical modeling.
 


  
act tab
act
cc act act cc f H H
H
ASI H W R R
3
2
(3.17)


 
foil neg foil neg foil pos foil pos
Rf L L
, , , ,
2 2
 
(3.18)


25
Rcc  R f     3 H W act act  H W tab     (3.19)
The cell terminals are ultrasonically welded to the ends of the current collector foil tabs. While the welding removes this contact resistance, the ASI of the terminal must be included in the total cell resistance. The ASI of the cell terminals, ASI term cell , is the summation of the positive and negative cell terminals as shown in Eq 3.20. The dimensions for these terminals are set by the calculated width of the cell and the user defined terminal thickness and height.
pos
term term
term
term neg term pos
A
W L
H
ASI  
 

 
, ,
cell
term
1 1
 
(3.20)
The ASI for connection losses is the last term in the ASI summation stated in Eq. 3.16. This ASI value is calculated by multiplying the ratio of cell positive electrode area to number of cells by the summation of the resistances, Rcnct, for cell terminals, module terminals, module interconnects, and batteries terminals. In this way, each cell shares in the burden of overcoming the system losses from carrying the electric current. The calculation of Rcnct is detailed in Eq. 3.21 with the individual sources of connection losses shown. The voltage drop resulting from cell-to-cell contact resistance, Rcntct cell , is taken to be 10-4Uocv,E in Eq. 3.22, a small fraction of the open-circuit voltage. A battery manufacturer would only tolerate a minimal voltage drop from cell-to-cell contact. One connection method is to physically press the two cell terminals together. This resistance could be lowered by increasing the physical pressure and contact area, or by laser welding the terminals together. Regardless, the value used in the model is left to the choice of the user to leave as is or to change to a different value.
Rcnct  Ncell Rcntct cell  NmodRterm mod  Nmod 1Rincnt mod  Rterm batt (3.21)
pos
cell cell ocv E
cnct
IA
N U
R  104 , (3.22)
The module terminal resistance, Rterm mod , calculation in Eq. 3.23 is shown as an example of how the terminal and interconnect resistances are calculated for the module and battery pack. The size of the terminals and thus their resistance are determined from a calculation based on a pre determined allowable rate of temperature rise for the conductor. This approach is explained in more detail in subsection 3.4.3.
 
mod
2
mod
term term
term term
term N
r
H
R
 
 (3.23)

26
3.4.2 Potential and Current Distribution in the Current Collection Foils
The designed current collection system was evaluated using a numerical simulation package. Equations 3.24-3.26 were solved for a steady state, isothermal, and 1-D simulation. Here, the conductivity, σj, is the effective conductivity of ½ of the foil (the other half carries the current from the opposite side). The bulk conductivity value, σj0, is multiplied by the thickness of the conductor, Lj/2, to lower the dimension of transport.
    
echem
ocv pos neg
n ASI
U x x
I   1,  1, (3.24)
 pos1, pos  In (3.25)
 neg1,neg  In (3.26)
The boundary conditions were set for both ends of each foil. The tab ends of the foils were set to a specified voltage and the opposite ends of the foils were restricted to a no flux condition. The simulation was performed using the foils defined in our battery design: 12 micron thick copper foil and 20 micron thick aluminum. The cell length was 20 cm, the ASIechem was 30 ohm cm2, and the Uocv and Vcell were set to 3.72 and 3.57 V respectively. Figure 3.5 shows the current and potential distribution in the foils and in the cell resulting from the simulation. The cell potential along the length of the foil varies only by 1.5 mV from maximum to minimum difference. The 0.04 % variation in voltage results in a 0.9 % variation in current density. This verifies the current density is uniform along the length of the foil. This is also obvious from the linear relationship of current with foil height in Fig. 3.5. The assumption of constant current density was tested in cell heights up to 100 cm and found to be satisfactory. The assumption should be reasonable as long as the ASIechem is at least twice the value of ASIcc. The simulated resistance of the foils is found to raise the ASIechem by 0.7 for an ASIpower of 30.7 ohm cm2. Additionally, the numerical result verified that H/3 is the correct equivalent length to represent the ASIcc for the cell. This may also be found analytically, Eq. 3.27-3.29, if you assume an even current distribution. We have shown that to be a reasonable assumption.
1,  2 2
2
V I H x
pos
n
 pos  cell  

(3.27)
1,neg  Ineg n     x 2 2  xL    (3.28)


  
  
  
pos neg
cell
H
n
pos neg
echem cc
H
I
V
dx
H I
ASI ASI
 
1 1
3
1 2
0
1, 1, (3.29)


27
Figure 3.5 The change in current and potential within the positive and negative foils. The current collection design results in a uniform current distribution along the length of the foil.
3.5690
3.5700
3.5710
3.5720
3.5730
3.5740
3.5750
0 0.2 0.4 0.6 0.8 1
x/H
Positive foil and cell potential, V
-0.0060
-0.0050
-0.0040
-0.0030
-0.0020
-0.0010
0.0000
Negative foil potential, V
Cell
Positive foil
Negative foil
0.00
0.02
0.04
0.06
0.08
0.10
0.12
0 0.2 0.4 0.6 0.8 1
x/H
Foil current per width, A/cm
0.00486
0.00487
0.00488
0.00489
0.00490
0.00491
0.00492
Current density, A/cm2
Negative foil
Positive foil
current density


28
An analogous problem has been solved by Euler and Nonnemacher and then communicated repeatedly by Newman et al.24, 25 The analytical solution they presented may be used after a slight alteration to dimensionalize the current density to the geometry of our concern, Eq. 3.30 and 3.31. This solution was reached assuming linear polarization behavior and is valid for cases where the current density varies along the height of the current collector foil. Thus, this approach is a more general solution than the one we use in the design model.
 




 



   
 
v v
v
H
I
U
neg
pos
pos
neg
neg pos
ocv pos neg
echem cc
sinh
2 cosh
ASI ASI 1
2
1, 1, 



 
(3.30)


 
ASI echem pos neg
H
v
 
2 2 1 1
(3.31)
3.4.3 Determination of Module Terminal, Battery Terminal, and Module Inter-connect Size An important factor for setting the resistances of a module terminal, battery terminal, or module interconnect is the allowable rate of temperature rise in the conductor at full power. We set the acceptable rate of temperature rise, dT/dt, at 0.2 °C/sec or a 2 °C rise for a 10-sec power burst under adiabatic conditions. The heating rate, q, is then used to determine the mass, m, of the terminal required for the designed battery in Eq. 3.32. Since the heating rate may also be determined by Eq. 3.33, we may determine the cylindrical terminal radius and mass by assuming a length, Hterm. In this way, the size of the module terminal is redesigned during each simulation to meet the specified power requirements and allowable temperature rise, Eq. 3.34. The mass of the conductor is found to be inversely proportional to the allowable temperature rise.
dt
dT
q  mC p (3.32)
 pos2
term term
term IA
A
H
q

 (3.33)
1/ 2



dt
dT
A IA C
term pos term term p (3.34)
A copper busbar must also be sized for batteries using a single row of modules. We have somewhat arbitrarily assumed a ∆Vbb = 30 mV drop across the busbar to be allowable at maximum current. This value maybe easily changed by the user. Equation 3.35 is used to calculate the mass of the busbar, mbb. The complicated expression for the volume of the busbar is derived from the voltage drop, conductivity, busbar width, wbb, and required busbar cross sectional area.

29
 
bb bb
tot bb
bb bb
w V
I
m




2
(3.35)
3.5 Calculation of Battery Dimensions
The goal of the model is to quantify how the various components of a specific battery design sum to make the mass and volume of the battery pack. In this way, a true energy and power density can be calculated as well as the exact materials requirement to meet this design. Summing the mass of the components is relatively straight forward. Determining the total volume that contains the components and required free volume is not as obvious. The exact calculations used in the design model are detailed below for the cell, module, and battery pack. 
3.5.1 Cell Dimensions
The number of layers in each cell is approximated in Eq. 3.36 by accounting for the compression factor, Xcomp, and the individual thicknesses of the current collector foils, Lfoil, electrodes, Lpos and L neg, separator, Lsep, and container, Lcont. Xcomp is usually taken to be 0.97. The Li-ion battery chemistries this model was designed for are assumed to undergo negligible volume change on the cell level. Slight volume changes can be accommodated as mentioned in Section 2.3.
2( )
2
sep neg pos
pos
foil
neg
foil
neg
cell cont foil
layers comp
L L L L L
L L L
N X
   
 
 (3.36)
The Nlayers approximation is necessary as the cell thickness is a user defined parameter. The aspect ratio of the cell is also user defined; therefore, solving for the width also determines the height of the cell as seen in Eq. 3.37. The width is calculated from the number of layers and the aspect ratio, H/W. The factor of 2 enters the denominator as both sides of the foil are assumed to be coated.
layers
pos
pos
N
A H W
W
2
 (3.37)
Having determined the width and height of the electrode, the rest of the cell dimensions are relatively straightforward, Eq. 3.38 and 3.39. The width of the cell, Wcell, is 2 mm wider than the positive electrode to allow for the larger separator area and pouch seals. The thickness of the folded edge, Le, is also included in the width dimension. The pouch seals are folded up, pressing along the inside wall of the module casing. The height of the cell, Hcell, is the height of the positive electrode in addition to the distance for the terminals and connections to the foil tab, Lterm,cnt. Our assumed design requires 15 mm for this distance at each end of the cell for a total of 30 mm. The volume of the cell is the product of the three dimensions.

30
Wcell  Wpos  2  2Le (3.38)
H cell  H pos  2Lterm,cnt (3.39)
3.5.2 Module Dimensions
The module dimensions are defined by Eq. 3.40-3.42. The height and length of the module are both just 2 mm wider than the cell dimension. The width of the module is related to the total thickness from all of the cells with allowance for a SOC controller at one end.
2
H mod  Wcell  (3.40)
2
Lmod  H cell  (3.41)
Wmod  Lcell Ncell / mod 11 (3.42)
3.5.3 Battery Pack Dimensions
The battery pack volume includes all of the modules, spacing for connections between modules, channel for the cooling air to flow, Hair, thickness of the module compression plates, Lcomp, and the battery pack jacket, Ljack (Eq. 3.43-3.45). Ljack includes a 10 mm thick insulation layer sandwiched between two aluminum walls for the container. The thickness of the aluminum wall increases from 1 to 1.5 to 2 mm as the battery volume increases from < 20 L to < 40 L to larger dimensions. The layout of the modules, number per row, Nmod/row, and number of rows, Nrow, is also included. The final volume of the battery is the product of the three dimensions. The space left for connections between modules, Lgap, is a function of the number of rows of modules. Lgap is equal to 8, 10, or 20 depending if there is one, two, or four rows of modules. Three rows of modules are not allowed as the positive and negative terminal for the battery would be on opposite ends and thus not very practical. A number greater than four rows of modules is deemed unnecessary.
Hbatt  H mod  2H air  2L jack (3.43)
Lbatt  Nmod/rowWmod  H air  2Lcomp  2L jack (3.44)
Wbatt  NrowLmod L gap2L jack (3.45)
3.6 Maximum Electrode Thickness
A practical limitation exists for the maximum achievable electrode thickness. This limitation may be set by manufacturing capabilities, ionic and electronic current transport within the porous electrode, susceptibility to plating lithium on the negative electrode, or aging characteristics related to adhesion to the current collector. Some of these challenges are discussed in great detail in the following subsection. When the maximum electrode thickness, Lmax, has been reached on either the positive or negative electrode, the electrode area equation is modified as shown in Eq 3.46. The electrode thickness, Ltgt, is the largest electrode thickness, negative or positive, calculated at the targeted fraction of the OCV [V/U].
31
pos
L tgt
pos A
L L
A
max
max
 (3.46)
The area of the electrode is now determined by the cell capacity requirement to meet the battery energy demands and not the target voltage at rated power. As a consequence, the battery pack will operate at a higher [V/U] than originally selected by the battery designer. The new [V/U] may then be calculated from Eq. 3.47 which is the solution to the quadratic found in Eq. 3.48.
 


    


cells pos
batt power
cell cell
cell N A
P ASI
U U
U U
V
4
2
1 2
(3.47)
cell cells pos
batt power
cell cell
V N A
P ASI
V  U  (3.48)
The maximum electrode thickness may have a large impact on the energy density and cost of cells designed for high energy and range. Nelson et al. demonstrated this concept in 2009 assuming a 100 micron maximum electrode thickness.12,19 In 2010, Santini et al. relaxed this assumption to 300 micons; although, the thickest electrode discussed in the paper was a 225 micron graphite electrode in the LMO-Gr EV with 100 mile range.13 In conversations with manufactures, 100 microns appears to be the general electrode thickness used for EV type cells at the present time. However, Santini et al. has shown substantial increases in energy density and decreases in cost if larger electrode thicknesses may be utilized. The challenges to achieving thick electrodes, in addition to those already mentioned, relate to fast charging while avoiding lithium metal deposition, utilizing all of the materials reversible capacity, removing gases formed during formation cycling, wetting the full porosity of the electrode, achieving defect free coatings, and drying the thick electrode at high rates. Our opinion is that the successful cell manufacturers will engineer ways to overcome these challenges to increase energy density and lower cost.
Dependent upon the battery chemistry and designed P/E ratio, the maximum achievable electrode thickness (loading) may have a significant effect on the end cost and energy density of a battery pack. For batteries designed at low P/E ratios or for cell chemistries with low volumetric capacities, the designed electrode thickness based on the target efficiency is often larger than what is feasible during operation in a transportation environment. This subsection explores some of the challenges that arise in the electrochemistry when larger electrode thicknesses are utilized.
Argonne gained a wealth of experience in the NCA-Gr in 1.2 M LiPF6 3:7 EC:EMC cell during the Advanced Technology Development program sponsored by the US Department of Energy (DOE). Dees and coworkers developed a world-leading parameter set for a numerical model through exhaustive electrochemical measurements, ex-situ characterization techniques, and multi-scale modeling activities.26-35 The resulting phenomenological cell model founded on the methodology originating from John Newman (UC Berkeley) will be used to evaluate the electrochemical behavior of cells using thick electrodes.36 The coupled, non-linear partial differential equations are solved with the finite element method using FlexPDE.
Simulated discharge capacity for the C/1 and C/3 discharge rate is shown in Figure 3.6 as a function of electrode thickness. For reference, the target positive electrode thicknesses for this cell operating at a 5C-rate and a [V/U] = 0.8 is 142 microns. The line of 100 % capacity utilization is also shown as a means to judge the deviation from theoretical capacity. As expected, the C/1 rate deviates more strongly than the C/3 rate with increasing electrode thickness. The loss in capacity is a result of the cell hitting the discharge voltage cut-off, 3.3 V,before all of the lithium has been transported from the negative to the positive electrode.
Figure 3.7 displays the normalized concentration profile of the electrolyte salt, LiPF6, at the end of a C/1 and C/3 discharge for an electrode thickness of 245 microns. The C/1 discharge results in a positive electrode starved of electrolyte salt. This transport limitation results in the cell prematurely reaching the voltage cutoff. In order to overcome this limitation, the electrode would need to be engineered with significantly reduced tortuosity37 or utilize an electrolyte with better mass transfer characteristics. This behavior is exacerbated by lower temperatures, such as those experienced during winter driving conditions. The fraction of theoretical discharge capacity begins to lower significantly at thicknesses greater than 100 microns, 3.4 mAh/cm2, at the C/1 rate and 175 microns, 6.4 mAh/cm2, at the C/3 rate. The electronic transport properties of the cathode material also play an important role in determining the current distribution within the electrode. While the NCA material has a reasonably high conductivity, other cathode materials have lower valued electronic conductivities and, depending on the conductive additive properties, may have different current distributions and limitations within the electrode.

Figure 3.6 Cell capacity simulated at the C/1 and C/3 rate as a function of electrode thickness (loading) for NCA-Gr.
Figure 3.7 Normalized electrolyte salt concentration at the end of discharge at the C/1 and C/3 discharge rates. The second half of the positive electrode next to the current collector is starved of the LiPF6 salt resulting in a lower utilization of the inherent cell capacity.
8 6 4 2 0
10
0 50 100 150 200 250 300 350
Electrode Thickness, microns
Discharge Capacity, mAh/cm2
3-Hour Discharge Capacity
1-Hour Discharge Capacity
100 % of capacity
0.0
0.5
1.0
1.5
2.0
2.5
0 100 200 300 400 500
Cell Coordinate, microns
c/cavg
1C Discharge
C/3 Discharge
Negative
Positive
Separator

34
The simulated ASI for a 5C, 10-s discharge pulse at 60 % SOC is shown in Figure 3.8 as a function of electrode thickness. The initial decrease in the ASI is a mathematical result of diminishing significance of the interfacial impedance as more current is passed in the same geometric area. The ASI then remains constant from 75 microns to nearly 400 microns. The constant ASI results from ohmic losses that behavior linearly with applied current. The dramatic increase in the ASI at the largest electrode thicknesses results from limitations in electrolyte transport within the porosity of the positive electrode. This is similar to what is displayed in Fig 3.7 above during the constant discharge at the C/1 rate for an electrode thickness of 245 microns.
The most significant issue for pulse power operation with thick electrodes occurs on the negative electrode during a charge or regen pulse, Figure 3.9. The potential of the negative electrode may drop below that of a hypothetical lithium reference electrode during a charge pulse, inferring an undesirable side reaction of lithium plating on graphite.38 This behavior is exacerbated by increasing electrode thickness. Operation at higher SOC and lower temperatures will also increase the probability of lithium plating. The lithium reference electrode is taken to be in the center of the separator layer. The two times shown in the graph, 1-s and 10-s, represent different polarization measurements for the electrode. The 1-s value includes all of the interfacial impedance and minor contributions from concentration polarization. The longer time value includes additional changes in potential due to the concentration gradient in the electrolyte. The 1-s time is the more accurate valuation of the tendency of the electrode to plate lithium. 
Figure 3.8 Calculated ASI from a simulated 10-s, 5C discharge pulse for the NCA-Gr cell couple at 60% SOC. Positive and negative electrode thicknesses are similar in value for this cell design. Transport within the electrolyte is not limiting until the electrode thickness approaches 450 microns for these simulation conditions.
0
10
20
30
40
50
0 100 200 300 400 500
Electrode Thickness, microns
ASI10s, ohm cm2
Full Cell
Positive Electrode
Negative Electrode

35
Figure 3.9 The potential of the negative electrode versus a hypothetical lithium reference electrode located in the center of separator during a 5C charge pulse for the NCA-Gr couple.
The tendency for lithium plating appears to be significant at electrode loadings greater than 3.4 mAh/cm2 under these specific conditions. Lower continuous and pulse charge rates are most likely necessary to ensure the safe operation and long life of this battery. Fast charging of PHEV and EV batteries is an oft discussed value-added characteristic necessary to increase the attractiveness of electric vehicles to the consumer. However, this fast charge requirement may require a lower loading design to prevent lithium plating from occurring. This would not be true for batteries based on LTO negative electrodes, or possibly even non-graphitic carbon electrodes (e.g. hard carbon). The consequence of a lower loading design is that higher quantities of inactive materials are used resulting in a more expensive and less energy dense battery.
A limit of 100 microns has been chosen for the default maximum electrode thickness. This thickness represents a graphite electrode balanced to a positive loading of 3.5 mAh/cm2 and is the largest thickness that ASI measurements have been validated at Argonne. However, a low volumetric capacity electrode, such as LMO, will result in a lower area-specific capacity as the limit will be determined by the positive electrode thickness. One domestic OEM has suggested that at the time of this publication, state of the art electrode loadings for PHEV applications are less than 2 mAh/cm2. This low loading level was selected based on cold-start performance, life testing, and rate capability studies. We note that different electrolytes will likely have the most significant effect on the transport limitations and result in different optimum electrode loadings. Gel-based electrolytes or standard carbonate electrolytes mixed with low molecular weight polymers are often utilized in pouch cell based batteries. While the ionic conductivity of these systems may approach standard carbonate electrolytes used, diffusion of the salt is restricted.
-0.4
-0.3
-0.2
-0.1
0.0
0.1
0 50 100 150 200 250 300 350
Electrode Thickness, microns
VNegative vs. VLithium, volts
1s Pulse Time
10s Pulse Time

36
This decrease in mass transport will result in large increases in impedance during longer discharges (constant speed highway driving). Hence, companies using an electrolyte with sluggish mass transport will require thinner electrodes than what the model would normally calculate based on pulse power applications. Greater electrode thicknesses may be achievable in the future as manufacturers expend significant engineering efforts to minimize the inactive material that lowers energy density and raises cost. The concerns over lithium plating may remain unless new, less susceptible negative electrodes are developed that still enable high energy density.
Table 3.2 displays a calculated sensitivity analysis for designing the battery at different target electrode loadings to achieve 17 kWh of total energy for the NCA-Gr cell couple for two power levels, 120 kW and 60 kW of power. The consequence of varying electrode loading at constant power and energy is to change the fraction of open circuit voltage at which rated power is achieved at BOL. This quantitative comparison of electrode thickness with [V/U] is only valid for the specific battery and cell chemistry designed in the table, while the qualitative results would hold for all systems. An alternate but equivalent way to create Table 3.2 is to maintain a constant value of [V/U], but vary the designed power level. As mentioned previously, private communications suggest that current electrode thicknesses used in PHEV applications are near 50 microns or 2 mAh/cm2; however, the exact details of that cell configuration are unknown and thus direct comparison should be conducted with caution. For the cell chemistry shown in the table, a loading of 1.9 mAh/cm2 with 120 kW of power correlates to achieving the rated power at BOL at [V/U] = 0.84. Our default suggestion of using 80% of OCV results in a moderately less expensive battery, albeit similar in value. If a battery of lower P/E ratio were designed, then the electrode thickness (loading) would be much larger for the same designed fraction of open circuit voltage. The sensitivity to [V/U] decreases with lower [V/U] values owing to the inverse proportionality of electrode loading to the P/E ratio. The calculated designed electrode loadings for lower P/E ratios will differ the most significantly from those used in industrial practice today. This is in part the motivation to limit electrode thicknesses to 100 microns as well as the transport limitations discussed earlier. While the standard practices of today are important, the goal of the calculations is to evaluate the potential cost of Li-ion batteries in the future years after improvements have been made resulting from the competitive marketplace. Therefore, calculating a range of values will be the most instructive approach to determining where future battery costs may fall. Additional variation studies may be found in Appendix A.
Table 3.2 The effect of electrode loading on the price of a 17 kWh NCA-Gr PHEV40 battery with 96 cells
17 kWh Loading Thickness Battery cost Loading Thickness Battery cost
[V/U] mAh/cm2 m US$ mAh/cm2 m US$
68 7.0 180 4218 3.2 82 4664
72 6.5 166 4244 3.0 76 4726
76 5.8 149 4284 2.7 68 4822
80 5.1 129 4345 2.3 58 4969
84 4.2 107 4445 1.9 48 5210
88 3.2 81 4647 1.4 35 5653
92 2.1 54 5039 0.9 22 6699
60 kW 120 kW


37
4. Thermal Management
The power and life of Li-ion batteries are more drastically affected by temperature than most other batteries including those based on lead-acid, nickel-cadmium, and nickel metal-hydride systems. It is important that the temperature of a Li-ion battery be controlled at all times, even when the battery is at rest. Developing schemes for effectively controlling the pack temperature at minimum cost will certainly be important in the success of this technology. The most difficult problem is the removal of heat generated within the battery, principally by ohmic heating. Avoiding excessive temperature rise during idle periods in hot ambient conditions is also a problem. Either of these conditions might raise the temperature to well above 40oC, which enhances degradation reactions and shortens the battery life. In fact, maintaining the battery near the minimum temperature for adequate power will prolong battery life by retarding degradation reactions. Because the battery has poor power at low temperatures, heating the battery from a very cold condition is necessary and especially difficult for large EV battery packs for which no assistance is available from the engine. For electric-drive vehicles to be competitive in the market with conventional vehicles, these thermal control problems must be solved at moderate costs by means that do not compromise the safety of the vehicle or battery system. 
The BatPaC model has a separate worksheet for designing the thermal management system. The results are transferred to the Battery Design worksheet to calculate the mass, volume and materials requirements for the battery pack.
4.1 Heat Generation Rates in the Battery Pack during Driving
During driving, the heat generation rate depends on the drive cycle and the power of the battery relative to the demands of the cycle for the vehicle being driven. As discussed below in section 4.2, fluctuations in the temperature of the pack are smoothed out by the battery heat capacity. The rate that the cooling system must handle is the average rate for the most difficult sustained driving conditions to which the battery pack will be subjected.
There are two types of driving profiles that will generate high heating rates in the battery pack. One is a drive cycle such as the US06 that has rapid acceleration and deceleration, including periods at high speeds. The average heat generation rate for such driving profiles is difficult to evaluate and is best done by vehicle simulation studies. These studies require a battery impedance algorithm that makes possible accurate estimates of internal battery heating during vigorous driving patterns. The results of vehicle simulation studies of battery heating can be entered on line 37 in the Thermal worksheet to override the estimated default values. A second driving profile that causes a high rate of battery heating is driving at a high, constant speed for a prolonged period (i.e. >5 minutes). Battery heating is easier to estimate for this condition because the battery power requirement is a direct function of the vehicle speed and the battery impedance approaches a constant value after a few minutes of driving.
Vehicle simulations were completed by Argonne’s Advanced Powertrain Research Facility with the Autonomie model. The battery energy required to support all-electric driving was compared for the US06 driving cycle and a constant speed of 70 mph based on a vehicle similar to the Chevrolet Volt. In that study the impedance of the LMO-G battery was determined with a model that had been derived from HPPC data. The model has an ohmic resistance and two polarization resistances with time constants of 15 and 270 seconds, respectively. The model is useful for calculating the changing impedance during a complex driving cycle such as the US06 cycle and it reproduces the impedance values entered in the “Chem” worksheet for the stated conditions. Table 4.1 shows the results of this study including the parameters derived to enable calculation of the heat generated in the battery operated at constant speed.
38
The first column of values shows the results of the study for the Autonomie model for both the US06 cycle and constant speed driving at 70 mph. The sum of the power for accessories, rolling friction and aerodynamic drag was divided by the total power determined in the Autonomie model to obtain a vehicle efficiency factor. This factor accounts for power losses in the power converter, the motor and the gears. This vehicle efficiency factor is assumed to be sufficiently constant over the vehicle speeds of interest for the purpose of establishing battery cooling requirements and the associated cost.
The energy demand per mile of travel for the vehicle of Table 4.1 was calculated to be 250  Wh/mile from the useable battery energy of 10 kWh for 40 miles of travel on the Urban Dynamometer Driving Schedule (UDDS). As shown at the bottom of the first column of figures, the estimated constant speed at which this energy demand would result is 57.85 mph. The second column of figures shows how the key parameters from the first column have been adjusted to round numbers that are suitable for the approximations required in BatPaC, and these values are highlighted in yellow. BatPaC then calculates the remaining parameters in close agreement to Autonomie.
The electric energy consumptions (Wh/mile) for the two types of driving are almost the same, but the higher average speed at 70 mph indicates a higher energy consumption per unit time (higher power) for this constant speed than for the US06 cycle (average speed of 48.4 mph). More importantly, a high heating rate results because constant rate discharge of the battery pack causes high battery impedance, which reaches more than twice the impedance of the battery when operated for short power bursts. The US06 cycle has long periods of high speeds resulting in elevated battery impedance, but this increase in impedance is mitigated by periods of low power demand during which the impedance decreases. Thus, driving at a constant high speed for an extended time results in the maximum heat generation rate in the battery and justifies our emphasis on this source of battery heating, which fortunately is the easiest to calculate.
For microHEV battery packs, heat generation is intermittent and substantial periods of little or no heat generation exist in the load profile. The model estimates the heat generation rate for 25-kW microHEV batteries at 100 W, which is entered on line 36 in the Thermal worksheet. For the larger battery packs (HEV-HP, PHEV and EV), the BatPaC model calculates the vehicle constant speed at which the centerline of the hottest cells in the battery will reach the maximum allowed temperature with steady state cooling, which is set at 35oC in the sample calculation on line 18 of the Thermal worksheet. That speed is deemed to be the maximum speed that the vehicle can be driven without damaging the battery by overheating. The battery control system should be designed to limit the battery output as this condition is approached.

Table 4.1 Energy Requirements for EREV Midsize 40AER similar to Chevrolet Volt. Highlighted values are the parameters required by BatPaC to estimate heat generation.
Autonomie
Values
Adjusted for
BatPaC
Vehicle Parameters
Mass, kg
Power for accessories, kW
Rolling resistance, kg/kg
Factor for rolling resistance power, kW/mph
Coefficient of drag, CD
Frontal area, m2
Factor for aerodynamic drag, kW/(mph)3
1850
0.472
0.008
0.0647
0.311
2.372
4.060E-05
0.5
0.065
4.0E-05
Parameters for LMO-G Battery
Battery power, kW
Battery energy, kWh
Usable battery energy, kWh
Designated electric range, miles
Standard energy demand, Wh/mile
100
15.0
10.0
40.0
250
100
15.0
10.0
40.0
250
Autonomie Results
US06 Cycle
Electric energy consumption, Wh/mile
Average power (excluding stopping and regeneration), kW
Maximum power, kW
70 mph Constant Speed
Power, kW
Electric energy consumption, Wh/mile
327.3
25.2
126.4
22.67
323.8
Constant Speed Results from Vehicle Parameters
70 mph
Power for accessories, kW
Power for rolling friction, kW
Power for aerodynamic drag, kW
Vehicle efficiency factor*
Total power, kW
Electric energy consumption, Wh/mile
Speed for 250 Wh/mile Energy Demand
Estimated Speed (So), mph
Power for accessories (Pa), kW
Power for rolling friction (Pf), kW
Power for aerodynamic drag (Pd), kW
Vehicle efficiency factor (e)*
Total power (Po), kW
Electric energy consumption, Wh/mile
0.472
4.53
13.93
0.835
22.67
323.8
57.85
0.472
3.74
7.86
0.835
14.46
250
0.5
4.55
13.72
0.833
22.53
321.9
58.0
0.5
3.77
7.80
0.833
14.49
250
*Determined by dividing the sum of the power for accessories, rolling friction and aerodynamic drag by the total power determined in the Autonomie model.

40
This maximum speed will depend on vehicle design parameters, the type of electric drive (HEV HP, PHEV or EV), the battery maximum power, the type of cooling system, (cabin air or liquid) and the battery design as it affects the efficiency of cooling. Under some conditions, it might be desirable to set a lower speed than that limited by battery heating to reduce the required capability and cost of the cooling system. This can be done by entering the maximum constant speed at which the vehicle will be operated on line 20 and BatPaC will calculate the maximum steady-state temperature at the center of the cells on line 19. 
Since it has been established that the maximum battery heating will occur when the vehicle is driven at a high, constant speed, it is necessary to estimate the power needed to drive the vehicle at any desired speed and the resultant battery heating. For this purpose, approximate equations are needed for vehicle parameters including accessory power, rolling friction and aerodynamic drag. A starting point for deriving these equations is the battery power calculated from the energy requirement per mile, E  (Wh/mile) entered on the Battery Design worksheet, line 172. The battery power, Ps0 (kW), will sustain a vehicle speed of S0 at the designated value of E  .
Ps0 = S0 E  /1000 (4.1)
The total battery power for maintaining the designated speed for the energy requirement is the summation of power demands for accessory power (Pa), rolling friction power (Pf), aerodynamic drag power (Pd) and power losses resulting from inefficiencies in the electrical and mechanical components of the powertrain system. From the calculations described in Table 4.1 we estimate the efficiency (e) from the battery to the wheels and accessories to be approximately constant at 0.833. The accessory power is estimated to be constant at 0.5 kW, but the model user may wish to increase this value to allow for air conditioning in warm climates and battery cooling. Estimates of the power to the system for cooling the battery (based on a coefficient of performance of 2.5 for the refrigeration cycle) are calculated on line 39 of the Thermal worksheet.
For midsized sedans, the power to drive the vehicle can be estimated with the energy requirement per mile, (Wh/mile) as the starting point. A reduction in the future from the default value of 250 Wh/mile will result primarily from reduction in the vehicle weight, which will reduce rolling friction. Thus, for the rolling friction factor, fPf (kW/mph), we propose:
fPf = 0.065· E  /250 (4.2)
And, the power for rolling friction, Pf (kW) is:
Pf = fPf ·S (4.3)
Aerodynamic drag is more difficult to reduce than vehicle weight. However, the interaction between the speed and the total power (a function of both Pf and Pd ) affects the drag factor, fPd, which is the product of the drag coefficient and the vehicle frontal area. The drag factor is estimated here from the default value of 0.00004 kW/(mph)3.
fPd = 0.00004·( E  /250)0.3 (4.4)
41
The value of Pd at any vehicle speed, S, may be calculated with the expression:
Pd = fPd·(S)3 (4.5)
The battery power, Ps, at any specified sustained vehicle speed can then be calculated from:
Ps = (Pa + Pf + Pd)/e (4.6)
Eq. (4.1) and (4.6) are solved simultaneously for S0 by iteration on lines 8 and 9 of the Thermal worksheet. S0 is used to calculate fPf and fPd by means of Eq. (4.2) and (4.4).
For battery packs other than microHEV battery packs, the BatPaC model calculates the heat generation rate, q (W), from the battery current, Itotal (A), and the battery resistance for a sustained constant discharge, Rbs (ohms).
= ( ) (4.7)
The value of Rbs for PHEV and EV batteries is calculated from the total ASI for the energy of the cell (taken at the C/3 rate and an average resistance assumed to be the same as that at 50% SOC), and entered on line 28 of the Thermal worksheet. This value is equivalent to the sum of the ohmic and polarization resistances for the impedance model used in the Autonomie vehicle simulation study described above. For HEV-HP applications, the battery is operated for an estimated 30 to 60 seconds and the value of Rbs is estimated to be 20% more than for the battery resistance at maximum power. Also the average battery heat generation rate is conservatively estimated as 60% of q as defined by Eq. (4.7) because only about 60% of the power for the vehicle is delivered from the battery; the balance of the power for the vehicle comes from the engine by direct coupling to the drivetrain or through a generator and motor. For PHEV and EV batteries, the heat generated in the battery pack is calculated directly from Eq. (4.7). Battery current and voltage, V, are calculated as follows:
Itotal = 1000·Ps/V (4.8)
� =
−�
��� ,� + ���� ,� 2 − 4 ∗ 1000 ∗ � � ∗ ��
2 (4.9)
The heat generation rate in the battery is selected on line 38 in the Thermal worksheet from three possible values: (1) for microHEV batteries it is 100 W (line 36), (2) for batteries that have been modeled in a vehicle simulation program to determine maximum sustained heat generation and the result entered on line 37, and (3) for all other battery packs, the heat generation rate calculated on line 34 (based upon Eq. 4.7 and modified as discussed above for HEV-HP batteries) is selected.
As a check on the practicality of estimating the heat generation in the battery by the method described above, another calculation was done by Argonne’s Advanced Powertrain Research Facility with the Autonomie model. In that calculation, the vehicle was an advanced sedan with an energy demand of only 201.8 Wh/mile on the UDDS cycle resulting from a vehicle weight of only 1625 kg, rather than 1850 kg as in the initial study (Table 4.1). The drag factor was only lightly lower than previously (i.e. 3.7x10-5 vs. 4.0x10-5). A comparison of the results of calculations on Autonomie and BatPaC are shown in Table 4.2.
42
Table 4.2 Comparison for calculated heat generation by Autonomie and BatPaC 
Autonomie BatPaC
Energy demand ( E  ),Wh/mile 201.8 201.8
Constant speed at E  , mph 53.4 53.2
Battery power at 75 mph, kW 24.4 24.3
Heat loss in battery at 75 mph 50% SOC, W 1343 1516
Average heat loss on 2nd US06 cycle, W 1062
Average heat loss on 3rd US06 cycle, W 1082
It is noted that BatPaC accurately reproduced the Autonomie results for constant vehicle speed, for the standard energy demand, and for battery power at 75 mph. BatPaC slightly over estimates the heating at 50% SOC because it calculates the impedance for the parameters at that SOC. TheAutonomie calculations take into account the lower values of the parameters at lower SOC and the time delay in adjusting to the ever increasing parameters with increasing SOC. The calculations in Autonomie illustrate, again, the higher rate of heat generation for high speed continuous driving than on the US06 driving cycle.
With the determination of the heat generated in the battery as a function of vehicle speed, as described above, the vehicle speed and the associated maximum temperature at the cell center are determined by the model in the following iterative procedure. The desired maximum battery temperature at steady-state is entered on line 18 and the model calculates the maximum sustained battery power, line 30, the internal battery heat generation rate, line 34, and the maximum sustained vehicle speed associated with those values, line 21. In this process, the heat generation value is transferred to the liquid cooling section beginning on line 69 or the cabin-air cooling section beginning on line 114, as determined by the type of cooling entered on line 68. In carrying out this calculation, if the temperature calculated is different from the temperature target on line 18, the vehicle speed is automatically adjusted by the program and the process is repeated until agreement is reached between the calculated temperature on line 19 and the target on line 18. The maximum temperature at the center of the cells is calculated at the end of the heat transfer calculations for the liquid-based and the cabin-air based thermal management approaches (lines 113 and 174, respectfully). As noted above, an alternative to dictating maximum cell temperature is to enter the maximum continuous vehicle speed under electric power on line 19 of the Thermal worksheet. Then the model program will override the process above and calculate the maximum cell temperature from the selected continuous vehicle speed.

43
The overall adequacy of the cooling is estimated on line 41 as a function of the maximum temperature of the battery at steady-state cooling as follows:
Maximum Cell Temperature Cooling Adequacy
35 oC or less Excellent
Over 35 oC to 40 oC Good
Over 40 oC to 45 oC Fair
Over 45 oC Poor
4.2 Heating under Adiabatic Conditions
A factor to be considered in thermal management is the substantial heat capacity of the battery pack. The thermal mass of the battery evens out temperature fluctuations resulting from power bursts so that the heat dissipation system need only handle the average heat generation rate for the most extreme driving profiles the battery is likely to encounter. For large PHEV and EV batteries the heat capacity of the battery will limit the temperature rise of the centerline of the cells by distributing the heat throughout the battery. For a large EV battery with power of 120 kW and energy of 50 kWh, the temperature rise under adiabatic conditions may be only 10oC or less for a complete discharge and certainly less with a cooling system even if that system is only moderately effective. For HEV batteries, which have high power-to-energy ratios, the main effect of the heat capacity will be to smooth out temperature fluctuations.
4.3 Active Thermal Management Systems
Several heat transfer fluid types have been considered for battery pack thermal management including air from the cabin, which may be heated or cooled, ethylene-glycol/water (EG/W) solutions and dielectric liquids such as transformer fluids. Additionally, cooling plates in contact with surfaces on the cells or the modules may be cooled directly with refrigerant. Air is the least expensive, but it is less effective than the liquid coolants because of its poor conductivity, the need for large flow passages and high pumping power. Dielectric liquids are expensive, but have the advantage of being compatible with terminals and other parts at electrical potential. A 50/50 EG/W solution is inexpensive and has better properties as a coolant (thermal conductivity, heat capacity, and viscosity) than typical transformer fluids. Cooling directly with a refrigerant would eliminate the need for an intermediate heat transfer fluid and may be the most efficiency of the systems, but it is more technically complex to access, which was not attempted here. In this study we consider both thermal management approaches with heat transfer fluids of cabin air and EG/W solution. To evaluate cooling with a dielectric fluid, it would only be necessary to substitute the properties of the dielectric fluid for those of EG/W solution (lines 84-87) and to increase the cost of the thermal management system to allow for the higher cost of the heat transfer fluid. Cooling and thermal management will be used interchangeably in this report. However, we emphasize the need of the thermal management approach to allow for both cooling and heating of the battery.
For both the liquid-based and the cabin-air based thermal management approaches, we selected a general cell design that can be adapted to all of the electric-drive batteries from micro-HEVs packs to EV packs (section 2). For all types of batteries, the liquid-based design incorporates a hermetically sealed module closure. This design can be effectively cooled by liquids and requires that only the module terminals and connectors be protected from contact with a conducting coolant, thus accommodating EG/W coolant. Aluminum heat sinks in contact with the broad surfaces of the cells transfer heat to and from the module surface (Fig. 2.4) that is in contact with the heat transfer fluid.
44
The enclosure does not have sufficient surface area to be cooled effectively by air. For cabin air based thermal management, heat transfers fluid flow passages are included between the cells, which add considerably to the pack volume. That design feature permits air cooling for microHEV and HEV-HP batteries. Air based approaches might also be used for some combinations of vehicle parameters and PHEV and EV battery configurations that result in low heat generation rates. However, air cooling is much less effective than liquid cooling and may not be effective in high heat generation applications (e.g. continuous all electric drive at autobahn speeds).
4.3.1 Thermal Management with Ethylene-Glycol/Water Solution
For the assumed format, the battery pack coolant is contained by the battery jacket and thus severely limits the practical pressure drop in the coolant circuit. The pack is on the suction side of the pump so the module structure assists in supporting the walls of the battery jacket. This approach is simple to calculate and appears to result in a workable design of low cost. Alternatively, cooling plates with built-in flow channels and capable of withstanding high pressure may be used with EG/W heat-transfer fluid reducing the likelihood of this electrolyte contacting cell or module terminals. Leaks in any system using an electrolyte fluid are a serious danger. For that reason alone, such fluids may have to be replaced by a dielectric fluid in future batteries.
4.3.1.1 Heat Transfer from Cell to Module Wall
As described in section 2, the cells transfer heat to the cooled walls of a hermetically sealed module with the aid of an aluminum heat conduction channel. Some of the heat is transferred through the sides of the cell to the channel and from there to the module wall. Other heat is transferred directly through the seal edge of the cell to the conduction channel flange which is in contact with the module wall. Calculation of heat transfer in this two-dimensional array through several materials is complex requiring a numerical model. The spreadsheet iterates many times in reaching a solution for the electrical and physical parameters for the battery as discussed in section 2. Each of these iterations results in a slightly different cell design. Thus, it would be impractical to imbed a numerical model directly, which may increase the total calculation time to many minutes. Instead, a software program based on the finite element method, FlexPDE 6.15 by PDE Solutions Inc., was employed to calculate heat transfer rates for 70 cell configurations. The resulting simulations were empirically correlated so that simple equations occupying a few cells in the spreadsheet could rapidly calculate the heat transfer rate with only a small error.
An important requirement for calculating heat transfer rates within the cell is to estimate the composite conductivities of the cell layers both parallel to the layers and across the layers. The resulting conductivities vary considerably with the relative thicknesses of the layers as shown in Table 4.3, for which the results are consistent with the literature.39-43 These values for conductivities and a range of cell dimensional parameters (Table 4.4) were employed in selected arrangements for calculating heat transfer rates with the FlexPDE model for 70 representative cells that covered a broader range of variables than is needed for practical cells.

45
Table 4.3 Sample calculations of composite thermal conductivities of cell structures across layer and parallel to layers
Cell 1 Cell 2 Cell 3 Cell 4
Layer Thicknesses, microns
Positive foil
Negative foil
Positive coating
Negative coating
Separator
Total bicell structure
20
12
30
40
20
212
20
12
75
100
20
422
20
12
150
200
20
772
20
12
220
300
20
1112
Thermal Conductivities, W/cm-K
Aluminum
Copper
Positive coating
Negative coating
Separator
Across layers, kx
Parallel to layers, ky
2.0
3.8
0.013
0.013
0.0020
0.00689
0.4127
0. 2.0
3.8
0.13
0.13
0.0020
0.00689
0.4127
0. 2.0
3.8
0.13
0.13
0.0020
0.01045
0.1228
0. 2.0
3.8
0.13
0.13
0.0020
0.0.01112
0.0892
Table 4.4 Range of parameter values for calculating heat transfer rates in FlexPDE model Parameter Levels Evaluated
1 2 3 4
Conductivities, W/cm-K
Across layers, kx (a)
Parallel to layers, ky
Cell edge, ke
0.00689
0.4127
0.10
0.00689
0.4127
0.01045
0.1228
0.0.01112
0.0892
Cell Dimensions, cm
Cell thickness, Lcell
Cell width, W
Cell edge thickness, Le
Aluminum conductor thickness, LAl (b)
0.6
8
0.1
0.03
1.0
12
0.06
1.4
18
0.10
(a)The kx and ky values are calculated as in Table 4.3 and were, thus, paired together in the Flex PDE model calculations.
(b)The total conductor thickness consists of the conductor thickness itself plus twice the thickness of the aluminum layer within the pouch material.
For each of these cells, the FlexPDE model calculated the temperature difference between the cell center and the module housing per unit of heat generation, T/q (oC/W), and the fraction of the total heat that was transferred through the edge of the cell, qe/q. The balance was transferred through the side of the cell to the aluminum conductor, qs. The division of the heat transfer into two routes is represented by the equation:
46
q/T = qe/T + qs/T (4.10)
Estimated values for qe/T and qs/T were determined by empirical correlation of the results obtained for the calculation of the 70 cells by the FlexPDE model with the result shown in Fig.
4.1. Empirical values of these estimated values resulted in the equations:
qe/T = 3.917ky0.58kx-0.19Lcell1.2W-0.75 (4.11)
qS/T = 1628ky0.55kx0.58Lcell-0.21W-0.7LAl0.72 (4.12)
Figure 4.1 Plot comparing the estimated resistance to heat transfer from the cell center to the cooled surface of the module to that calculated by the FlexPDE model.
The average error in the estimated T/q compared to the values calculated by the FlexPDE model for the 70 cases studied was 6.0% and the maximum error was 13.0%. This accuracy was deemed to be satisfactory in that for all practical battery designs, the error in estimating the difference in temperature between the cell center and the module housing, T, will be only a fraction of a Celsius degree.

47
4.3.1.2 Heat Transfer from Module Wall to Flowing Coolant
The model directly calculates the temperature drop between the module wall and the heat transfer fluid for a set pressure drop, fluid (coolant) temperature rise, and fluid physical properties. A 50/50 ethylene glycol, deionized water (EG/W) mixture was selected based on the low cost and contemporary use in coolant systems. The default pressure drop was taken to be 10 millibar, but may be changed by the user if desired. The gap in which fluid flows is sized to maintain the target pressure drop without going below a minimum gap height of 3 mm. A coolant temperature rise of 1 °C was selected to establish a mass flow rate, but also may be changed by the user.
Calculation of the heat transfer coefficient allowed for determination of the temperature difference between the module and average coolant temperature. A schematic of the flow passageway and change in temperature profile with distance is shown below in Fig. 4.2. The outer wall of the flow passage is assumed to be perfectly insulated. The inner wall (module casing) is assumed to have a constant heat flux perpendicular to the wall. Laminar flow was assumed to simplify the calculation of the velocity profile (parabolic). 
Figure 4.2 Heat transfer from the module wall to the laminar flow heat transfer fluid. The temperature profile of the fluid is shown at different lengths down the flow path.
Frequent use of dimensionless numbers was necessary to adequately correlate the numerical results into a generally useable form. We define the Reynolds, Prandlt, Graetzl, and Nusselt numbers here for completeness44. The Reynolds number, Re, is the ratio of inertial to viscous forces. The Reynolds numbers were always less than 1000 confirming laminar flow. The Prandlt number, Pr, is the ratio of the momentum diffusivity to thermal diffusivity. The Prandlt number for the EG/W mixture is approximately 38. The Graetz number, Gz, is directly proportional to the product of the Reynolds and the Prandlt numbers. Moreover, the Gz value is inversely proportional to the distance down the fluid flow path, l, resulting in higher values near the start of the flow path. Finally, the Nusselt number, Nu, is the ratio of the convective to conductive heat transfer. Here uave is the average fluid velocity, dH is the hydraulic radius (twice the flow gap), and μ is the viscosity. The heat capacity, cp, thermal conductivity, k, and heat transfer coefficient, h, are the critical heat transfer values. The mass flow rate, G, and the width of the channel, W, are the remaining parameters.

u aved H
Re  (4.13)
48
k
c
p
Pr  (4.14)
Gz 2 2 Re Pr
l
d
kWl
Gc d
p H H
  (4.15)
k
hd
H
Nu  (4.16)
Coupled momentum and heat transfer has been solved previously by determining a number of the eigenvalues of an analytical series solution for a vast number of various geometrical configurations related to pipe, duct, and parallel plate flow45,46. We have chosen to reach the solution numerically and then fit a correlation between the Graetz number and the mean Nusselt number. The empirical form provided by Nickolay and Martin provides an accurate means of correlating the results over many orders of magnitude47. The correlation, shown in Eq. (4.17), relates the Graetz number and the limiting solution, Nu∞ = 5.385, to the mean Nusselt number. Then, the mean heat transfer coefficient may be directly calculated from Nu. Here n and C1 are fitting parameters.
Nu  Nun  C1Gz1/3n1 n (4.17)
The numerical model was solved with the finite element method using FlexPDE software. We note that the bulk or “cup mixing” fluid temperature in Eq. (4.18), the average temperature of the fluid normalized by the fluid velocity profile, was necessary to reach the proper values.
  T y u y y
u
T
avg
avg ( ) ( )
2
1
(4.18)
The following important assumptions were used to reach a solution.
1. Flow of incompressible heat transfer fluid is laminar
2. Thermal diffusion is allowed up and down stream of the heat transfer (for convergence)
3. Boundary conditions: dT/dy = 0 at insulation; q = constant at module casing
4. Negligible radiative energy transfer
5. Steady state conditions reached
Figure 4.3 displays the temperature profile between the module casing and the insulated wall for various distances along the flow channel. The average temperature of the fluid has risen 1 °C at the end of the flow path even though the maximum and minimum temperature is separated by nearly 5 °C. The simulated change in average temperature down the length of the flow channel allows the calculation of the average heat transfer coefficient and thus Nusselt number. The correlation, Eq. (4.17), determined from various simulations conditions is shown in Fig. 4.4. An excellent fit is obtained allowing for implementation of the correlation into the design and cost model. This correlation now enables efficient and accurate calculations of the heat transfer coefficient to be made in the spreadsheet informing the user of the effectiveness of the thermal management in the design.
49
Figure 4.3 Temperature profile in the heat transfer fluid for various fractions of the
dimensionless path length.
Figure 4.4 Correlation of model simulation results relating the Graetz number and mean Nusselt number for laminar flow between an insulated surface and the module casing.
24.5
25.0
25.5
26.0
26.5
27.0
27.5
28.0
28.5
29.0
29.5
-1 -0.5 0 0.5 1
Dimensionless distance from centerline Fluid temperature, C
0.00
0.02
0.24
0.46
0.68
0.90
Dimensionless distance
down fluid path
1
10
100
0.1 1.0 10.0 100.0 1000.0
Graetz number, Gz
Mean Nusselt number, Num
Calculations
Correlation
Nu
∞ = 5.385
n = 3.592
C1 = 2.255

50
In general, the heat transfer from the module is improved by increasing the contact area and increasing the fluid flow rate. The contact area may be increased by using cells with a higher aspect ratio. This also results in a smaller temperature gradient within the cell as discussed previously in section 4.3.1.1. Increasing the fluid flow rate is accomplished by using a lower temperature rise and/or a larger target pressure drop. The gap height may prevent a change in a single parameter from having a significant effect on the temperature drop. Physical limitations of implementing a cooling system should be considered when moving to higher flow rates and pressure drops. The user should note that raising both of these parameters will increase the cost of the battery design in ways that the model does not consider (e.g. more expensive pump, increasing structural integrity, etc).
For high speed driving or very aggressive driving cycles, the temperature difference between the surface of the cooled module surface and the bulk of the coolant may become fairly large (>10oC). This coupled with the temperature rise within the cells could result in too high cell centerline temperatures. This result can be avoided by controlling the inlet coolant temperature as a variable that is adjusted in a classic cascade automatic control system to control the module wall temperature at the desired value. Thus, the temperature rise at the center of the cells will be essentially held to that resulting from conduction within the cell and will not be greatly influenced by the temperature rise in the coolant. The use of the vehicle air-conditioning system to cool the liquid coolant allows a standard coolant temperature of 15oC, or even lower if necessary.
4.3.2 Thermal Management with Cabin Air
Air-based thermal management requires a much larger heat transfer surface area than that of liquid thermal management approach discussed in section 4.3.1. In this study the extra surface area was gained by flowing air past the faces of the individual cells as shown in Fig. 2.5. This approach greatly simplifies the calculation of heat transfer from the interior of the cells, which can be solved as a one-dimensional calculation as contrasted with the more complex two dimensional calculation done for liquid thermal management of the outside of the module (section 4.3.1.1). The air flows in at the bottom of the long side of the battery pack, splits into many flow steams as it flows up the passages between the cells and then recombines and flows out the top of the battery pack.
4.3.2.1 Temperature Drop from Cell Center to Cell Wall at Steady State
The composite conductivity across the cell layers was calculated by dividing the total cell thickness by the sum for all layers of the conductivity of each layer divided by its thickness as illustrated in Tables 4.1 and 4.2. The temperature drop from the center of the cell to the cell wall, ∆Tcell, was calculated as follows:
∗
∗ ∗
(4.19)

51
4.3.2.2 Heat Transfer from Aluminum Cell Sleeve to Flowing Air
The length of the cooled section of the cell is taken to be the same as the length of the positive electrode. The number of air flow channels is essentially calculated by dividing this length by the target width of an air flow channel plus that of one web and rounding down to an integral number. The target width was taken to be 1.0 cm, but any width between 1.0 and 2.0 cm will provide similar results for cooling. The exact width of the channels is calculated from the electrode length and the number of channels. The thickness of the channel is calculated to meet the pressure drop for the required flow rate. The required flow is that which will carry off the heat generated by the cell divided by the number of cooling channels per cell. 
Because of the difficulty in moving sufficient air through the pack to carry out the heat generated in the cells, the air must be allowed to rise in temperature by about 5oC, whereas a 1oC temperature rise is sufficient for liquid-cooled packs. We also used a higher pressure drop to force the air through the pack, 0.02 bar versus 0.01 bar for liquid-cooled packs. The pressure drop for air cooling is divided between that through the channels between the cells (90%) and that in the large passages across the bottom of the pack where the air enters and across the top of the pack where the air leaves (10%). This distribution of the available pressure drop, which is achieved by sizing the thickness of the channels between the cells and those at the top and bottom of the pack, provides an even supply of air to all channels between the cells. All of the parameters discussed for managing the air flow are adjustable by the model user, but large deviations from the suggested values may adversely affect the feasibility of the design. 
The heat transfer flux to establish the temperature drop from the cell sleeve wall to the bulk air stream is calculated in much the same way as described for the liquid-cooled battery packs (section 4.3.1.2). However, for the air-cooled packs, heat is transferred from both sides of the channel rather than from only one side as for the liquid-cooled modules, which have insulated jacket walls on the opposite side of the cooling channel. For transferring heat from both sides, the value of is 8.235 rather than 5.385 for use in Eq. (4.17).
4.4 Cooling and Heating Required to Maintain Pack Temperature
When parked in the sun for several hours, the internal vehicle temperature and, thus, that of the battery may become so hot that the life of the battery is reduced. To avoid this with liquid-cooled systems, the vehicle air conditioning system may be actuated intermittently to cool the battery. By allowing the temperature of the battery to fluctuate by several degrees, it is only necessary to actuate the cooling system about once per hour for a few minutes. For a set of target temperatures with a difference of 25oC and with the default insulation thickness (10 mm) and default thermal conductivity (0.00027 W/cm-K), BatPaC calculates the average cooling requirement to be about 60 W for PHEV-40 batteries. The performance coefficient of the vehicle air-conditioning system might reduce the actual energy draw to less than half that, but heating of the system outside of the battery during the hour-long downtime periods would be a counter acting factor. The BatPaC calculates the energy required for cooling of all types of electric-drive vehicle batteries. However, most HEVs, even if cooled by liquids, may not have electrically driven air-conditioning units and some other method might be needed to avoid very high battery temperatures during parking such as thicker insulation and fan cooling during parking. Batteries for any type of electric vehicle that are cooled by air would require similar measures or some method of connecting the air cooling to an electrically-driven air-conditioning system or dedicated refrigeration system. The additional cost for any special system to deal with high ambient temperature that is not a part of the system to remove heat generated within the battery has not been provided in the BatPaC model.
If the battery is to deliver full power at startup, it must be at a temperature of at least 5oC. This minimum temperature can be maintained by heaters and circulation of the coolant, whether air or liquid. The BatPaC calculates the amount of power required to maintain the battery temperature for any set of battery and ambient temperatures. PHEV-40 batteries would require about 50 W of heat to maintain the battery temperature at 20oC above that of the ambient under steady-state conditions. During recharging this should be easily done for 20 hours at a cost of $0.10 with an energy cost of $0.10 per kWh. If the vehicle is not at a source of power for recharging, limited energy (say 1-2 kWh) can be drawn from the battery (if not blocked by a switch actuated by the driver) and then automatically shut off after maintaining the battery temperature for one to three days, depending on the ambient temperature.
4.5 Heat-up from Cold Ambient Conditions
All of the batteries for the various types of electric-drive vehicles will occasionally be exposed to very cold temperatures, which will require special heat-up procedures. All but the EV batteries can be heated with the aid of the engine. This can be done with electric heaters operated from power taken from the generator or from glycol solution from the engine cooling system. If the latter, it might be prudent to isolate the engine coolant from the battery coolant by means of a plastic heat exchanger.
Another method of heating the battery is by means of the electric heaters that should be available for maintaining the battery temperature (section 4.4). BatPaC calculates the amount of heat needed and the time required with suitable heater power. For PHEV-40 batteries, about 15 minutes is required with 2-kW heaters. This method of heating will be slower than with the engine coolant and even the latter would result in some delay before the battery is capable of full power.
To avoid delay in starting vehicles from a cold startup, the driver could initiate heating by means of a remote device, even a telephone. By this means, heating could be initiated either from heat drawn from the engine or electric heaters. Remote initiation of heat-up would be especially important for an EV away from a charging station in that no engine is available to assist heating and the large size of the battery would result in a long heating period with electric heaters. The BatPaC estimates the time under these conditions.

53
5. Modeling of Battery Pack Manufacturing Cost
5.1 Approach
The manufactured cost of a battery pack is calculated with input from the design information generated in modeling the cell and battery pack performance. The design modeling determines the annual materials and purchased items requirements. The manufacturing cost is then added to these materials costs, along with a warranty cost, to reach the unit cost of a single battery pack. The manufacturing costs for the designed battery are scaled from a baseline plant. The baseline plant was designed for a battery of intermediate size and production scale so as to establish a center-point for other designs. The baseline plant accounts for the size, speed, number of units, direct labor, and depreciation of the capital cost for each processing step. These costs are adjusted to meet the requirements for a plant producing the battery under study. The process expenses are summed with the additional costs of operating the manufacturing facility. These costs include launch costs, working capital, variable overhead, general, sales, administration (GSA), research and development, depreciation, and profit. Additionally, the costs for the thermal management, battery management system, and disconnects have been estimated to provide the total cost to the OEM for the integrated battery pack.
In this analysis, all costs are evaluated for 2020 when large battery manufacturing plants are built. All dollar values are brought back to 2010 with allowance for inflation. In other words, all costs and prices are in 2010 dollars. Some materials and battery manufacturing costs are lower than recent values, where we judged that processing improvements for high volume production of materials would reduce costs.
The baseline manufacturing plant was calculated for an annual production rate of 100,000 batteries. The cost model accounts for different scales of manufacture by recalculating the costs of each individual step in the manufacturing process. The changes in capital and operating costs will change the calculated unit cost of the battery pack. The parameters were determined to provide reasonable estimates for manufacturing rates of 20-500 % of the baseline rate. Thus, for a plant that is far different in size from the baseline plant, for instance a pilot plant having an annual production of only 5,000 battery packs per year, the estimate from this study would be expected to be less accurate than if determined in a study dedicated to that purpose.
To simplify the cost calculations, it was assumed that all hardware items for the cells, modules and battery will be purchased from a vendor specializing in similar products. The costs for these items were estimated to be a fixed value plus an additional value proportional to the weight of the item, which is calculated during the battery design. In mature manufacturing plants in 2020, toward which this study is directed, some items which are assumed to be purchased in this study might actually be internally manufactured from raw materials. This would increase the number of processing steps needed in our manufacturing simulation and thus complicate the cost calculations. Assuming that some parts would be purchased if they would actually be produced from raw materials would tend to underestimate capital and labor costs and overestimate purchased items expenses. However, the net effect would be a very small change to the overall unit cost of the battery pack.

54
5.2 Materials Costs, Purchased Items, and Pack Integration
The end battery pack cost depends significantly on the cost of both the active and inactive materials that compose the design. In this subsection, the assumed material costs and the rationale behind them are presented. We provide for means to scale the materials cost with production volume using the same method used for processing rates as discussed in section 5.4. In general, the materials costs will be largely insensitive to production volume since we have assumed a high volume market already exists. Only the negative and positive electrode active materials are assumed to have a minor benefit for larger scales of production. While we state suggested materials costs and sensitivity to production scale, the users of the cost model may enter any value that they desire.
5.2.1 Battery Specific Materials Cost
The largest contributions to the materials cost of the battery are from the following components: positive and negative electrode active material, separator, electrolyte, and current collector foils. The choice of the materials often defines the size and performance of the battery as well as the cost. Many different variations of materials are possible in the Li-ion family of chemistries. However, we have chosen to focus on the different available positive electrode materials with less attention on the negative electrode. This reflects the current research and manufacturing activities. The separator and the electrolyte are also both active areas of development. However, the following battery designs are based on a single electrolyte and separator combination. Including the cost and effect of additives and enhanced separators is beyond the scope of this work. The user is always able to modify the dimensions, cost, and ASI that may be required to account for changes in these materials.
The price of specific battery materials is of some debate. The values presented in Table 5.1 compare our suggested costs to those reported recently in the open literature. Our values, as well as the others in the table, are derived from conversations with material, cell, and original equipment manufacturers. The sources are commonly anonymous and the accuracy of the values is generally unknown. We present the comparison of published values so that the user of the cost model may appreciate the accepted range of values for commonly used materials.
5.2.1.2 Positive Electrode Active Materials
The cost of positive electrode materials is driven to a large extent by the cost of the raw materials from which it is made. The archetype Li-ion positive electrode material, lithium cobalt oxide (LCO), was the original material commercialized in Li-ion batteries for consumer electronics. LCO has many excellent characteristics but is not considered a viable choice for use in Li-ion batteries for automotive applications. One of the largest drawbacks of LCO, other than safety concerns, is the high and volatile cost of the cobalt. While tolerable in the consumer electronics market, the cost is too high for use in an automobile battery. Many other materials are in a commercially viable state of development and are currently utilized in Li-ion batteries produced today (Table 5.1) such as lithium manganese spinel oxide (LMO) and lithium nickel manganese cobalt oxide (NMC).3,6 The relative advantages and disadvantages of each material will not be discussed here.

55
Table 5.1 Details of stated costs for cathodes, anodes, electrolyte, and separator.3,6
ANL TIAX** CARB
Material Chemistry Abbreviation unit 2010 2010 2007
Manganese spinel cathode Li1.06Mn1.94-xM'xO4 LMO $/kg 10 12 - 16 - 20 8 - 10
5V spinel cathode* LiNi0.5Mn1.5O4 LNMO $/kg 21 - -
Phospholivine cathode LiFePO4 LFP $/kg 20 15 - 20 - 25 16 - 20
Layered oxide cathode* LiNi0.80Co0.15Al0.05O2 NCA $/kg 33 // 37 34 - 40 - 54 28 - 30
Layered oxide cathode* Li1.05(Ni1/3Mn1/3Co1/3)0.95O2 NMC-333 $/kg 31 // 38 40 - 45 -53 22 - 25
Layered oxide cathode* Li1.05(Ni4/9Mn4/9Co1/9)0.95O2 NMC-441 $/kg 26 // 29 - -
Li & Mn rich layered cathode* xLi2MnO3·(1-x)LiNiyMnzCo1-y-zO2 LMR-NMC $/kg 22-25 // 22-29 24 - 31 - 39 -
Layered oxide cathode* LiCoO2 LCO $/kg 36 // 59 - 30 - 40
Synthetic graphite anode C6 Gr $/kg 19 17 - 20 - 23 -
Natural graphite anode C6 Gr-Nat $/kg 10 - -
Titanate spinel anode Li4Ti5O12 LTO $/kg 12 9 - 10 - 12 -
Electrolyte 1.2 M LiPF6 in EC:EMC $/kg 18 18.5 - 21.5 - 24.5 -
Separator PP/PE/PP $/m2 2 1 - 2.5 - 2.9 -
Current collector foil Copper $/m2 1.80 - -
Current collector foil Aluminum $/m2 0.80 - -
* The cost of cathode materials using co-precipitation of Ni, Mn, and/or Co is based off of a correlation. Cobalt $44/kg vs. $81/kg separated by "//"
** Cost represent range of values possible

56
The amount of cobalt and nickel, as well as ease of manufacture, controls the end price for a positive electrode material. For example, the NMC-441 is less expensive than the NMC-333 as the cobalt quantity is significantly reduced. The market prices for cobalt and nickel metals vary dramatically from year to year. Reducing the quantities of these materials in the positive electrode will reduce the total price and price volatility. Researchers at TIAX LLC have treated this variation and shown the significant effect on end battery cost.10 The average traded metal prices and the 95% confidence intervals for the last 25 years is 44.4±18.3 $/kg and 14.9±7.6 $/kg for cobalt and nickel respectively. These numbers are based on historical prices for the metals as collected by the United States Geological Survey (USGS).48 The metal prices are indicators for how the intercalation material cost will relate when compared to one another. The fact these materials are not earth abundant means they will not benefit as much as other materials from increased scales of production.
We employ the relationship in Equation 5.1 to systematically calculate the cost of the transition metal based spinel and layered compounds. The final cost, C, of the lithiated oxide depends on the baseline cost, C0, and the contributions of the lithium and transition metal raw materials, Ci. The molar stoichiometry, xi, is transformed to a mass basis with the molecular weight of the raw material, MWi, and the final product, MW. The baseline cost is the sum of the cost for processing, additional raw materials, and profit margin associated with the manufacture of the materials. We assume a baseline cost of $7/kg for single metal containing oxides (LMO and LCO) and $16/kg for the co-precipitated metal oxides such as NMC-333 and NMC-441. NCA is known to have a slightly lower yield and requires additional raw materials resulting in an assumed C0 = $20/kg. The costs for Li, Ni, Mn, and Co are taken to be 0.22, 0.87, 0.15, and 2.6 $/mol respectively. The historical average metal prices for Ni and Co are used recognizing that these values will fluctuate over time. Aluminum is assumed to be similar in cost to manganese for these calculations. One may directly translate these numbers to raw materials costs resulting in $6/kg for Li2CO3, $5.6/kg for NiSO4, $16.9/kg for CoSO4, and $1/kg for MnSO4. Calculations are also shown in Table 5.1 using $4.8/mol ($81/kg) for cobalt as a demonstration of the upper 95% confidence interval cobalt price on the end material cost.
   
 
C    kg $ C0 MW 1 i xiCiMWi (5.1)
In general, earth abundant elements should be the dominate transition metals used if a low cost positive electrode is desired. Both iron and manganese are abundant and inexpensive transition metals for intercalation materials. Comparison of the iron phosphate, LFP, to manganese spinel, LMO, reveals how processing costs contribute to the end price of a material. LMO is relatively easy to manufacture. In contrast, LFP requires a reducing atmosphere and a carbon coating step to reach the end product. The increased complexity in the manufacturing process is realized in the price. However, one could argue that the manufacturing cost will decrease with increased knowledge from larger scales of production.
5.2.1.2 Negative Electrode Active Materials
While several negative electrode materials exist for Li-ion batteries, carbon materials in the form of graphite and/or hard carbon are still used in the vast majority of commercial cells. Graphite 57 offers the greatest energy density while hard carbon is said to enable high rate capability with decreased risk of lithium plating (an undesired side reaction) during high charge rates. We have chosen synthetic graphite as a generic carbon electrode in our model. Significant differences in cost and performance will exist between synthetic, natural, and coated-natural graphite. The method of production and necessary heat-treatment will control the end cost. Many manufacturers use a proprietary blend of natural and synthetic graphite and/or hard carbon in the negative electrode of their cells. The user of the model may feel free to vary the price depending on the application of interest.
The lithium titanate electrode, LTO, offers an interesting option compared to graphite. Unlike graphite, LTO operates within the stability window of the electrolyte. The higher electrode potential, 1.5 V vs Li, dramatically reduces or eliminates the formation of the solid electrolyte interphase (SEI). As a result, nanoparticle-based LTO may be implemented without concerns of increased side reactions with the electrolyte. The reduced nanoparticle dimensions increase the available surface area for reaction while simultaneously shortening the diffusion length. Both of these factors combined with the lack of SEI dramatically reduce the impedance of the electrode.
5.2.1.3 Electrolyte and Separator
The electrolyte used in this model is based on a lithium hexafluorophosphate salt, LiPF6, dissolved in a carbonate based solvent system. The carbonate solvent system is a blend of ethylene carbonate, EC, and a linear carbonate such as ethyl methyl carbonate, EMC, or dimethyl carbonate, DMC. Other chemical additives may be used to limit the capacity and power fade of the battery over time. Polymers may be added to the electrolyte as either a minor or major component. This is not discussed in any further detail in this work. The price of 18 $/kg, about 22 $/L, is only for the base electrolyte (i.e. no additional additives).
The separator is typically a porous membrane based on polypropylene (PP) and sometimes includes a polyethylene (PE) middle layer. PP and PE are very inexpensive raw materials and thus the suggested cost of $2/m2 is in large part due to the manufacturing process required to form the porous network in the membrane. As competition and scale of manufacture increase, the prices of the separator may fall closer to $1/m2. However, the cost of improved technology may offset some of this cost reduction, so we have retained our cost estimate of $2/m2. As safety is a major concern for Li-ion batteries, the separator plays a key role in isolating the oxidant from the fuel. If the two charged electrodes contact each other (short), then a run-away reaction is possible. Separators have been designed to “shut-down” or melt at key temperatures. The middle PE layer is the shut-down feature in our proposed separator. Ceramic coatings have also been used to ensure structural integrity. Many other approaches are being developed to increase the safety of Li-ion batteries. The user of the cost model should account for the specific separator technology in the price and dimensions (thickness and porosity) of the separator as needed.
5.2.1.3 Current Collector Foils
The current collector foils are based on copper metal for the negative electrode and aluminum for the positive electrode. However, the LTO anode material, because of its high voltage relative to lithium, enables the use of aluminum as the negative electrode current collector. The price of these foils is based on raw materials and manufacturing costs. The aluminum foil is produced by rolling of thicker stock foils into thinner and thinner sheets. On the other hand, copper foil is more likely to be produced through an electrodeposition process. The foils are 12 microns and 20 microns thick for the copper and aluminum current collectors respectively. The foils used in batteries have additional requirements beyond the cheapest product available. Surface treatments are often necessary to promote adhesion of the composite electrode to the foil surface. In addition, alloying of the foil may be necessary to achieve the required material properties for long life.


58
The raw material contributions to the foil price will vary with the volatility of the market price for the metals. Figure 5.1 displays the metal ingot price contribution on a $/m2 basis. These numbers are based on historical prices for the metals as collected by the USGS.48 The values for both aluminum and copper tend to vary significantly over the time period examined. The price for copper is more volatile and always more expensive than aluminum. Analysis of Figure 5.1 reminds the user of the cost model that cost quotes are only valid for a short period. As the market price for raw materials changes, so will the price for the finished product. 
Conversations with manufacturers and suppliers lead us to take a price of 1.80 and 0.80 $/m2 for battery grade copper and aluminum foil respectively. We point out that the current metal ingot price is only a small contribution to the end foil price being about 16 % of the aluminum foil price and 23 % of the copper foil price. Thus, a doubling of the ingot prices would only moderately increase the foil prices. 
Figure 5.1 Metal ingot cost contribution to the current collector foils over a 20 year period. The average for that period is also shown. All costs are in 2010 US$.
0.00
0.10
0.20
0.30
0.40
0.50
0.60
0.70
0.80
0.90
1985 1990 1995 2000 2005 2010
Year
Metal Ingot Cost in 2010 $/m2
Copper
Copper 20 yr avg
Aluminum
Aluminum 20 yr avg

59
5.2.1.4 Additional Electrode Components
The binder and conductive additive in the positive and negative electrodes add a small but real cost to the battery. The conductive additive, more common for the positive electrode, was priced at 6.80 $/kg for a high purity and moderate surface area carbon black material. The binder, perhaps PVDF or CMC based, is assumed to be 10 $/kg. The N-Methyl-2-pyrrolidone (NMP) solvent for the PVDF binder is estimated to be 3.20 $/kg. Most of the NMP is recovered after evaporation and recycled as discussed in section 5.3.3. Only the small amount lost in processing need be replaced. No cost is assumed for water used in the electrode slurry processing.
5.2.2 Purchased Items Cost
Table 5.2 lists the purchased items for the cell module and battery jacket. The cost of a SOC controller for each cell, or group of parallel cells, is $2.50 plus a small factor for the cell capacity (Ah), which allows for higher cell balancing currents for larger cells. The other component costs include a fixed amount plus an additional factor, which is proportional to their mass, mi. The cell negative terminal and parallel cell group connection are both made from nickel plated copper sheet and thus have the same cost equation. The costs shown for the terminals include an allotment for isolation tape that is necessary to protect the electrical connection. The bus bar is a fixed cost and is only charged if a single row of modules is used. A single row of modules requires a bus bar in order to locate the positive and negative terminals at the same end of the battery.
Table 5.2 Cost equations for purchased items
Component, i Cost Equation, $/unit Cost per unit
SOC controller 2.50 + 0.01C cell or parallel cell group
Cell positive terminal 0.25 + 4mi cell
Cell negative terminal 0.25 + 6mi cell
Cell container 0.20 + 3mi cell
Aluminum heat conductor 0.10 + 4mi cell
Parallel cell group connection 0.25 + 6mi parallel cell group
Module terminals 0.75 + 5mi module
Balance of module (casing) 1.00 + 3mi module
Module interconnect 1.00 + 5mi module
Battery terminals 15.00 + 0.02Itotal battery pack
Bus bar for one module row 20.00 battery pack
Battery jacket 30.00 + 7mi battery pack
5.2.3 Pack Integration Cost
Various additional components and thus cost are necessary to integrate the battery into the electric drive system, which adds cost. While it is not clear what should and should not constitute the cost of the “battery pack,” we present these additional items in Table 5.3 in an attempt to be complete. After all, the cost of the entire system is of interest to the final consumer of the product. The calculated total battery cost to the OEM may be directly compared to battery pack level goals as set by the U.S. Advanced Battery Consortium. This category in BatPaC includes the battery pack as well as the battery management system and disconnects. However, thermal management additions outside of the pack are only included in the total system cost to the OEM. The general conclusion is that the pack integration costs have the largest consequence for the smallest batteries. The worst case is perhaps that of a small PHEV10 battery. The integration costs of a PHEV10 battery carry the burden of charging from the grid, but provide only a modest electric drive benefit. The fixed cost of pack integration may amount to 25 % of the battery pack total even without considering the costs of additional powertrain components. Clearly, understanding the entire cost of the electric drive system is of importance to evaluating the true value of the electrified vehicle to a consumer.

60
Table 5.3 Costs to integrate battery pack into vehicle drivetrain. $/kW numbers reflect maximum kW of cooling or heating required.
5.2.3.1 Battery Management System
The battery management system (BMS), in our assumed battery design, integrates the modules and battery into the overall electric drive system. The BMS includes measurement and control features such as the following:
* Measurement of battery pack current and voltage
* Balancing of the module voltages (cell balancing done within module)
* Estimation of battery pack state-of-charge (SOC) and state-of-health (SOH)
* Estimation of module SOC and SOH
* Monitoring and signaling of battery thermal management

The cost of the BMS will scale with magnitude of battery current and with the need to charge from the electrical grid. Therefore the PHEV and EV batteries will have a higher burden from the BMS. The micro-HEV is assumed to have less complicated management and thus less cost than the HEV-HP.
Battery Pack Integration System PHEV
MicroHEV HEV-HP and EV
Current and voltage sensing, $ 40 70 100
Module controls, $/module 10 10 20
Auto. battery disconnect, $ 50 70 200
Manual disconnect per pack, $ 15 15 15
Additional for parallel modules and packs, $ per string 100
Thermal Controls PHEV
MicroHEV HEV-HP and EV
Baseline thermal system*, $ 30 80 120
Additions to AC system**, $/kW 40 40 40
Heating system**, $/kW/pack 20 20 20
Additional for multiple packs, $/additional pack 100
*$60 additional for each added pack
**No charge for cabin air cooling

61
5.2.3.2 Manual and Automatic Disconnects
The manual and automatic disconnects integrate a high-level of safety and electrical management into the electric drive system. The manual disconnect breaks the current flow pathway from the high-voltage terminals to the outer system allowing for the safe service of the vehicle and battery pack. This disconnect is designed to be operated when the electrical system is de-energized. The automatic disconnect is much more complex. This unit contains the connections for the high voltage system to the rest of the vehicle’s electrical system: drivetrain, grid charging (if applicable) and accessories (high and low voltage). Fuses are present as a hard-wired safety device to prevent unusually large current spikes from damaging the battery or drivetrain. Multiple contactors are used to appropriately channel electrical current depending upon normal operation or grid-charging. Engaging the contactors requires that multiple safety interlocks are established including isolation of the high voltage bus from the vehicle chassis and an inertia based sensor (crash protection). Finally, a small circuit is provided to prevent arcing of the current across the high-voltage contactor when the high-voltage circuit is closed.
The relative cost of the automatic disconnect amongst the various battery designs is driven by the pack voltage, maximum battery current, and the need for charging from the grid. The voltage of the pack has a significant effect if a 42 V micro-HEV pack is considered. For this system, electrical safety regulations allow a less complicated system to be used. Requiring higher battery currents generally increases the cost of electronics and conductors. The additional complications arising from grid-charging adds a significant additional cost to the PHEV and EV systems. It is unclear to the authors at this time what other factors may enable a lower burden of external safety controls. These additional costs in the automatic disconnect unit have the most pronounced effect on the cost of smaller batteries, as the burden amounts to a significant fraction of the total cost.
5.2.3.3 Balance of Thermal Management System
The thermal management of the battery is crucial to meeting the life and safety requirements of transportation applications. The complexity of this system must be minimized to reduce the cost and size burden on the vehicle. A single refrigerant compressor is used for both the cabin air and the battery cooling applications. Likewise, the same radiator and fan as the cabin cooling will also be used for the battery cooling refrigerant. Most OEMs appear to use an electric compressor for all full-HEVs (HEV-HP) and PHEVs/EVs that are liquid cooled. The incremental cost for an electric compressor at high volume in year 2020 will likely be $200-300 more than the commonly used $100 belt driven compressor. We do not include this incremental cost in our thermal management system cost; however, we state it here for completeness. The additional cost to the compressor for the battery cooling capacity is insignificant compared to burden of transitioning to the electric compressor. Experts in the field have informed us that the electric motor and high-voltage invertor are the largest contribution to the incremental cost of the electric compressor.
An expansion valve on the refrigerant line and a heat exchanger (chiller) transfers the thermal energy from the heat transfer fluid to the refrigerant loop. A 50/50 DI-water/ethylene-glycol solution is selected as the heat transfer fluid. The assumed battery design has the heat transfer fluid pumped over the module casing to transfer heat from and to the cells. The battery may be heated by either a positive thermal coefficient (PTC) or flexible mat heater. The PTC heater would directly raise the temperature of the heat transfer fluid in a reservoir while the matt heater would be placed under the battery jacket insulation.

62
The PHEV and EV batteries will likely have both active and passive thermal management modes requiring some additional monitoring and an electrically actuated valve. We have assumed decreasing cooling costs for the HEV-HP and microHEV systems without explicitly dictating where the savings originate. In general, one would expect smaller batteries to have a less complicated control system, lower flow rates and possibly even direct cooling of the cells with the evaporator.
5.3 Baseline Manufacturing Plant
The model’s baseline plant is designed to produce 100,000 NCA-Gr baseline battery packs per year. The baseline battery pack produced by the plant has sixty, 40-Ah capacity cells, providing a total pack power of 50 kW and total energy of 8.7 kWh. The battery will power 24 miles of vehicle travel at 70% of the pack energy and 250 Wh/mile. The schematic diagram of the plant (Fig. 5.2) is designed to illustrate the flow of materials through the plant and the relative floor areas for the processing steps rather than representing a realistic plant layout. The overall manufacturing rate of 100,000 battery packs per year is achieved by operating for three shifts at the equivalent of 300 days per year of fully effective production. There will be more than 300 days of operation, but all days will have less than 100% effectiveness. The exceptions to three shift operation are the Receiving and Shipping sections, which are active for only two shifts per day. The cost factors for the individual manufacturing steps in the baseline plant are summarized in Table 5.4 and discussed in detail in the sections that follow. Most of the operations are carried out with normal factory atmosphere, but the cell assembly process steps are completed in a dry room atmosphere.

63
Figure 5.2 Baseline lithium-ion battery manufacturing plant schematic diagram. Manufacturing rate: 100,000 NCA-Gr battery packs per year, 50-kW pack power, 40-Ah capacity, 60 cells per battery. Operating year: 300 days with three 8-h shifts (two shifts for receiving and shipping)
5.3.1 Receiving and Shipping
These operations incorporate the moving equipment and storage facilities common to any such factory facilities. The Receiving section handles slightly less than 6,000,000 kg of materials per year and also has facilities to handle and store some of the electrode materials in a dry atmosphere. The Shipping section is required to enclose the battery packs in crates, which requires some automated equipment and more labor than is required for Receiving. Shipping also handles about 400,000 kg of scrap each year, which is broken down and prepared for shipping in the Rejected Cell and Scrap Recycle section. The estimated resources needed for the Receiving and Shipping sections are shown in the table below.
Rate Factor Direct Labor Capital Equip.* Plant Area, m2
Receiving
Off-loading
Moving
Storage
870,000 kWh/y 3 per shift 3.60 mil$ total
0.60
1.20
1.80
900
Shipping 870,000 kWh/y 6 per shift 5.0 mil$ total 900
*Total cost including installation
The areas in this diagram for each processing step are approximately proportional to the estimated plant areas in the baseline plant.
Shipping
Cell and Scrap Recycling
Receiving
Control Laboratory
Assembly Route
Battery Pack Assembly and Testing
Module Assembly
Formation Cycling
Current Collector Welding
Enclosing Cell in Container
Electrolyte Filling and Cell Closing
Cell Stacking
Solvent Evaporation
Positive
Negative
Electrode Coating
Positive
Negative
Electrode Slitting
Vacuum Drying
Electrode Materials Preparation
Positive
Negative 
Calendering
Solvent Recovery
Air Locks
Charge Retention Testing
Final Cell Sealing
Dry Room
Materials Handling
Outdoor dry-room air processing equipment

64
Workers/ Baseline Scale Baseline Scale Baseline Scale
Shift Hours/yr Factor, p $millions Factor, p Area, m2 Factor, p
Receiving (two-shift operation) 869,416 kWh energy 3 14,400 0.4 3.60 0.6 900 0.5
Materials preparation
Positive electrode 1,712,524 kg active material 2 14,400 0.5 2.00 0.7 600 0.6
Negative electrode 1,060,374 kg active material 2 14,400 0.5 2.00 0.7 600 0.6
Electrode coating -
Positive electrode 8,209,039 m2 cell area 4 28,800 0.5 8.00 0.8 (0.2)* 750 0.8
Negative electrode 8,209,039 m2 cell area 4 28,800 0.5 8.00 0.8 (0.2)* 750 0.8
Solvent recovery 2,309,021 kg NMP 2 14,400 0.4 3.00 0.6 225 0.6
Calendering -
Positive electrode 8,209,039 m2 cell area 2 14,400 0.5 1.00 0.7 225 0.6
Negative electrode 8,209,039 m2 cell area 1 7,200 0.5 1.00 0.7 225 0.6
Materials handling# 8,209,039 m2 cell area 4 28,800 0.7 1.50 0.7 900 0.6
Electrode slitting 8,209,039 m2 cell area 4 28,800 0.5 2.00 0.7 300 0.6
Vacuum drying 8,209,039 m2 cell area 2 14,400 0.5 1.60 0.7 300 0.6
Control laboratory 869,416 kWh energy 4 28,800 0.5 1.50 0.7 300 0.6
Cell Assembly in Dry Room -
Cell stacking 6,315,789 total cells 5 36,000 0.7 4.00 0.8 (0.3)** 600 0.8
Current collector welding 6,315,789 total cells 5 36,000 0.7 4.00 0.8 600 0.8
Enclosing cell in container 6,315,789 total cells 3 21,600 0.5 3.00 0.7 600 0.6
Electrolyte filling, and cell sealing 6,315,789 total cells 5 36,000 0.5 5.00 0.7 900 0.6
Dry room control and air locks 2,000 m2 operating area# 2 14,400 0.4 20.00 0.6 100 0.4
Formation cycling 6,315,789 total cells 8 57,600 0.7 30.00 0.8 (0.3)** 2,200 0.8
Final cell sealing 6,315,789 total cells 2 14,400 0.5 2.00 0.7 450 0.6
Charge retention testing 6,315,789 total cells 3 21,600 0.4 4.75 0.7 900 0.6
Module assembly 6,000,000 finished cells 6 43,200 0.5 6.00 0.7 600 0.6
Battery pack assembly and testing 100,000 battery packs 6 43,200 0.5 6.00 0.7 (0.3)*** 900 0.6
Rejected cell and scrap recycle 6,315,789 total cells 5 36,000 0.7 2.50 0.7 600 0.6
Shipping (two-shift operation) 869,416 kWh energy 6 28,800 0.5 5.00 0.7 900 0.6
Total 90 626,400 127.45 15,425
#One-third of the space for materials handling is within the dry room.
*The baseline cost for capital equipment for electrode coating, Co, is based on the evaporation of the baseline annual solvent weight (Rso) of 2,309,000 kg for
the positive electrode and 1,527,000 kg for the negative electrode. For batteries requiring different solvent evaporation rates Rs, the cost is multiplied by
(annual solvent rate (Rs)/baseline rate (Rso)) raised to the 0.2 power. Thus, Cost = Co*(R/Ro)^0.8*(Rs/Rso)^0.2.
**The baseline costs of the capital equipment for cell stacking and formation cycling is for 40-Ah cells. To correct the baseline cost (C o) for cells of different
capacity, the cost is multiplied by the capacity ratio, (Cap)/ 40 Ah, raised to the 0.3 power. Thus, Cost = Co*(R/Ro)^0.8*(Cap/40)^0.3.
***The baseline cost of the capital equipment for battery assembly is for a battery with four modules. To correct the baseline cost to a battery with a different
number of modules (Mod), the cost is multiplied by the ratio of the number of modules, (Mod)/4 raised to the 0.3 power. Cost = C o*(R/Ro)^0.7*(Mod/4)^0.3.
Annual Baseline Rate (Ro)
100,000 Battery Packs per Year, 50-kW Battery Power, 40-Ah Capacity, 60 Cells per Battery
Operating year: 300 days with three 8-hour shifts (two shifts per day for receiving and shipping)
Direct Labor Cap. Equipment Plant Area
Table 5.4 Summary table of the baseline plant

65
5.3.2 Electrode Materials Preparation and Delivery to Coating
The electrode materials, which consist of active material, carbon (if necessary), binder and binder solvent, are well mixed in small batches in portable tanks. At the design production rate in the baseline plant, each shift requires three tanks each holding about 1000 liters of positive electrode material mix and three tanks each holding about 900 liters of negative electrode material mix. The section must be capable of exceeding this design rate of production by at least 25% to catch up in case of unscheduled downtime in Materials Preparation or in some of the section immediately following that section. The tanks of prepared materials are moved to the Coating section and pressurized to push the coating paste into the coating mechanism. The estimated resources needed are the following:
Materials Prep. Rate Factor Direct Labor Capital Equip.* Plant Area, m2
Positive
Materials
Storage tanks
Mixing tanks
Moving equip.
1,710,000 kg/y
active material
2 per shift 2.0 mil$ total
1.00 mil$
0.50
0.50
600
Negative
Materials
1,210,000 kg/y
active material
2 per shift 2.0 mil$ total 600
*Total cost including installation
5.3.3 Electrode Coating on Current-Collector Foil
The positive and negative electrode structures are formed by coating both sides of the current collector foil. In the baseline plant, the coating lines are 1.5 meter wide continuous roll-to-roll coating processes carried out at a line speed of 10 m/min. The first set of coating and drying stations coats one side of the current collector foil, drives off the solvent in a heated oven, and turns the foil over while transferring it to a second set of stations. The second set of coating and drying stations applies and dries the remaining coating before the coated foil is wound into a large roll at the end of the line. An advanced alternative would be to run the foil directly into the calendering process. The negative and positive coating lines are very similar. However, some of the negative material is coated only on one side to provide the electrodes at the end of the cell stacks. For the baseline plant, a total of 8,170,000 m2/y of coating (annual cell area) is required for the positive electrode (slightly more for the negative electrode), which allows for the 5% loss of cells expected to fail testing and inspection. A larger area of foil than the coated area must be fed to the coaters to allow for the part of the foil that is not coated so as to provide tabs for welding to the terminals (about 10%) and to allow for trimming losses during electrode slitting (8%). Also, about 30% excess coating capacity must be provided to allow for unscheduled downtime. Only one coating line is needed for each electrode type to meet these needs. If one coating line breaks down, the other coating line may change over temporarily to coat the other electrode material.
The oven sections of the coating line are designed to dry coatings about 100 microns thick at the coating speed of 10 m/min. A thicker coating will require longer ovens at additional capital cost which is provided in the adjustment of costs discussed in section 5.4. For the same annual area throughput, a coating line that coats both sides with a 300-micron coating would cost $9,500,000 rather than the $8,000,000 cost for the 100-micron coater. The binder solvent for the positive electrode in the baseline plant is NMP, which must be recovered by condensation and recycled. About 0.5% of the binder solvent is combusted with a thermal oxidizer and must be replaced. For the negative electrode the binder is water, which need not be recovered. The estimated resources to meet these needs are the following:

66
Electrode Coating Rate Factor Direct Labor Capital Equip.* Plant Area, m2
Positive Electrode
Uncoated area
Width of coater
Coating speed
Number of coaters
Maximum rate
Excess capacity
8,170,000
m2/y cell area
4 per shift 8.0 mil$ total
18%
1.5 m
10 m/min
One
13,000,000 m2/y
30%
750
Negative Electrode 8,170,000
m2/y cell area
4 per shift 8.0 mil$ total 750
Solvent Recovery &
Oxidation
1,527,000 kg
NMP/y
2 per shift 3.0 mil$ total 225
*Total cost including installation
5.3.4 Calendering
The materials leaving the coating lines may be stored on large rolls (see next section). However, typically the materials leaving the coaters would go directly to the calendering process in which the coatings are compressed by rolling to meet the specified void volume fraction, which will later be filled with electrolyte. The calendering equipment must match the output of the coating equipment producing 8,170,000 m2/y of cell area with a maximum rate of 13,000,000 m2 of foil per year to meet contingencies as in coating. We estimate three workers are necessary to collectively operate the two pieces of equipment. The estimated resources to meet these needs are the following:
Calendering Rate Factor Direct Labor Capital Equip.* Plant Area, m2
Positive Electrode 8,170,000
m2/y cell area
2 per shift 1.0 mil$ total 225
Negative Electrode 8,170,000
m
2/y cell area
1 per shift 1.0 mil$ total 225
*Total cost including installation
5.3.5 Inter-Process Materials Handling
For all processes (Fig. 5.2), work in progress must be transported and occasionally stored to permit nearly-continuous operation of the equipment. Storage areas must be provided both inside and outside of the dry room. Raw materials must also be moved to the processing sites, which for those in the dry room means through a separate air lock for materials transfer. One-third of the total space for Inter-Process Materials Handling is within the dry-room for the baseline plant and also for all other plants. The estimated resources to meet these needs are the following:
67
Materials Handling Rate Factor Direct Labor Capital Equip.* Plant Area, m2
8,170,000
m2/y cell area
4 per shift 1.5 mil$ total 900
*Total cost including installation
5.3.6 Electrode Slitting
The coated electrode foils are slit into strips between the coated sections and then into individual electrodes as shown in Fig. 2.3. The estimated scrap loss of foil for this process is about 8%. The estimated resources to meet these needs are the following: Electrode Slitting Rate Factor Direct Labor Capital Equip.* Plant Area, m2
8,170,000
m2/y cell area
4 per shift 2.0 mil$ total 300
*Total cost including installation
5.3.7 Final Electrode Drying
In the absence of electrolyte, no harm is done by exposing the electrodes to normal factory air; however, the electrodes must be dried by heating under vacuum prior to cell assembly. Maintaining extremely low moisture conditions during cell assembly is believed to be very important in achieving long battery life. The final drying step coupled with dry room conditions ensures minimal moisture content in the final product. The pertinent processing rate in determining the resources necessary for drying is the total amount of active materials processed per year (other electrode materials are approximately proportional), which for the baseline plant is 2,950,000 kg/y or 3,275 kg/shift. The individual electrodes exiting from the electrode slitting process are separated into stacks by polarity, loaded into vacuum drying ovens, dried for several hours, and unloaded directly into the dry room. The estimated resources to meet these needs are the following:
Electrode Drying Rate Factor Direct Labor Capital Equip.* Plant Area, m2
Dryer capacity
Number of dryers
Maximum rate
2,950,000 kg/y
active material
2 per shift 1.6 mil$ total
600 kg/shift
8
4,320,000 kg/y
300
*Total cost including installation
5.3.8 Control Laboratory
The purpose of the control laboratory is to ensure that the raw materials and the electrodes being fabricated meet specifications. Laboratory personnel collect or supervise collection of samples and carry out analyses. The estimated resources to meet these needs are the following:


68
Rate Factor Direct Labor Capital Equip.* Plant Area, m2
Control Lab 869,000 kWh/y 4 per shift 1.5 mil$ total 300
*Total cost including installation
5.3.9 Cell Stacking
The cells are assembled in four steps, which are carried out in a dry room. The first of these steps is cell stacking. The primary rate factor that determines the cost for all steps in cell assembly is the number of cells assembled per year. For cell stacking an additional cost factor is the capacity of the cells; large cells usually require more electrodes of larger area and thus a more capable, faster cell stacking machine. The method used to determine the extra costs of stacking equipment is detailed in Table 5.4. The capacity of the cells is deemed to have only a minor effect on the other steps in cell assembly and is not taken into account for those steps. The electrodes are inserted in a folded separator sheet, the positive electrodes tabs protrude on one side and the negative electrodes tabs on the other. As in other parts of the plant, excess capacity is provided to allow catching up after unscheduled downtime. The estimated resources to meet these needs for the baseline plant are the following:
Cell Stacking Rate Factor Direct Labor Capital Equip.* Plant Area, m2
Stacking rate
Number of units
Maximum rate
6,320,000 cells/y 5 per shift 4.0 mil$ total
5 cells/min
4
8,640,000 cells/y
600
*Total cost including installation
5.3.10 Current Collector Welding
The current collector tabs for the negative and positive electrodes are welded to their respective terminals by ultrasonic welding. This procedure achieves a connection of near-zero resistance and avoids overheating the electrodes during the welding process. The estimated resources to meet these needs are the following: 
Tab Welding Rate Factor Direct Labor Capital Equip.* Plant Area, m2
Cell rate
Number of units
Maximum rate
6,320,000 cells/y 5 per shift 4.0 mil$ total
5 cells/min
4
8,640,000 cells/y
600
*Total cost including installation
5.3.11 Enclosing Cell in Container
The aluminum foil layer in the pouch container is sufficiently thick (100 microns default thickness) to permit the use of stiff, pre-shaped pouch halves. The pouches are assumed to be purchased as finished parts. Each cell is enclosed in these containers, which are then partially sealed prior to injecting electrolyte. The estimated resources to meet these needs are the following:

69
Enclosing cells Rate Factor Direct Labor Capital Equip.* Plant Area, m2
Cell rate
Number of units
Maximum rate
6,320,000 cells/y 3 per shift 3.0 mil$ total
5 cells/min
4
8,640,000 cells/y
600
*Total cost including installation
5.3.12 Electrolyte Filling and Cell Sealing
At this station, the cells are evacuated, filled with electrolyte and temporarily sealed. The estimated resources to meet these needs are the following:
Filling & 1st Seal Rate Factor Direct Labor Capital Equip.* Plant Area, m2
Cell rate
Number of units
Maximum rate
6,320,000 cells/y 5 per shift 5.0 mil$ total
5 cells/min
4
8,640,000 cells/y
900
*Total cost including installation
5.3.13 Dry Room Management
Excellent dry-room atmosphere is required for lithium-ion cell assembly. A maximum dew point temperature of –40 °C is maintained in the room. The load on the dry-room drying apparatus is determined by diffusion of water vapor through the walls, entry of air through the air locks, the number of workers in the room, and the need to admit some fresh air to limit the build up of contaminants such as electrolyte solvent vapor. These load factors are approximately a function of the room area. Because of the importance of the proper functioning of the dry room, two workers are on duty at all times to monitor its performance. The equipment for circulation and purification of the dry air will be located outside of the plant building, adjacent to the dry room. The estimated resources to meet these needs are the following:
Operating Area
Direct Labor Capital Equip.* Air Locks, m2
Dry Room 3,000 m2 2 per shift 20.0 mil$ total 100
*Total cost including installation
5.3.14 Formation Cycling, Final Cell Sealing and Charge Retention Testing
Formation cycling is expensive because it takes considerable time and each cell must be monitored separately. For plants to be operated in 2020, we expect some improvements from present day operations because of the urgency to improve and thus save cost. We project that the entire formation cycling and testing can be done in two shifts. These operations consist of charging the cell, discharging to full depth to measure capacity and impedance, followed by fully recharging the cells. These tests will be carried out in large temperature controlled cycling units that test 500 cells simultaneously, monitor each cell and automatically identify failed cells. The capital cost of the cycling equipment is primarily a function of the annual number of cells to be tested, but to a lesser extent on the capacity of the cells.

70
The short-term testing described above does not detect cells that have self-discharge rates that are slightly above normal, which could lead to catastrophic failures later. To detect such defects, the cell charge is topped off and the cells are stored for two weeks and then checked for loss of charge. Most of the test period is spent in large racks in compact arrays, without electronic monitoring. Incidentally, the two-week long self-discharge testing requires less floor space than for formation cycling, which lasts only two shifts. 
The final cell sealing occurs between the formation cycling and charge-retention storage test. Gas generated during formation cycling may accumulate in the reservoir space that was created during the temporary sealing step. This gas is removed by creating the final seal below the reservoir and trimming off the unwanted portion.
The estimated resources to meet these needs are the following:
Rate Factor Direct
Labor
Capital Equip.* Plant Area,
m2
Formation Cycling
Cell capacity
Number of cyclers
Cells per cycler
Length of test
Testing capacity
6,320,000 cells/y 8 per shift 30.0 mil$ total
40 Ah
35
500
2 shifts
7,875,000 cells/y
2200
Final Cell Sealing 6,320,000 cells/y 2 per shift 2.0 mil$ total 450
Charge Retention
Testing rack capacity
Racks per stack
Number of racks
Length of test
Testing capacity
6,320,000 cells/y 3 per shift 4.75 mil$ total
500 cells
5
750
14 days
8,040,000
900
*Total cost including installation
5.3.15 Module and Battery Assembly
Approximately 5% of the cells are expected to fail the formation cycling and charge-retention tests and these are sent to the Rejected Cell and Scrap Recycle section. The accepted cells (6,000,000 finished cells per year) are assembled into modules by attaching the terminals through laser welding or mechanical joining with spring loaded devices. Electronic circuit packsare attached that occupy about the same volume as a cell. An aluminum heat conductor is placed around every cell. These operations are carried out at four automated stations each capable of handling about 280 cells per hour. For the module design being cost estimated in this model, the module is enclosed in an air-tight aluminum container by double seaming. The processing rate that determines the cost of module assembly is the number of finished cells that must be handled per year.

71
The finished modules are assembled into battery packs with the aid of automated stations. The total cost of these stations is dependant mainly on the number of battery packs to be assembled per year (100,000 for the baseline plant), but to a lesser extent on the number of modules per pack. After assembly, the packs are moved to testing stations where they are discharged as a final check of impedance and to lower the state of charge to a level suitable for shipping. The estimated resources to meet these needs are the following:
Rate Factor Direct
Labor
Capital Equip.* Plant Area,
m2
Module Assembly
Number of stations
Cells/h/station
Capacity
6,000,000 cells/y 6 per shift 6.0 mil$ total
4
280
8,060,000 cells/y
600
Battery Pack Assembly
Modules/pack
Number of stations
Packs/h/station
Capacity
100,000 packs/y 3 per shift 3.0 mil$ total
4 3 6
130,000 packs
450
Battery Pack Testing 100,000 packs/y 3 per shift 3.0 mil$ total 450
5.3.16 Rejected Cell and Scrap Recycle
Scrap is generated in preparing the electrodes and by the rejection of 5% of the cells that go through formation cycling and charge-retention tests. This scrap is gathered and packaged for shipment for recycling of the materials having value. No credit is taken for the value of the scrap in this model except that the costs of gathering, sorting, packaging and shipping are understated by about that value. The main factor in determining the cost of scrap recycle is the number of cells rejected, which have to be disassembled to recover the scrap, a labor intensive process. The yields of materials in the various processing steps are shown in Table 5.5.
Table 5.5 Materials yields during electrode and cell fabrication
Material Material
Mixing
Coating Electrode
Slitting
Cell
Stacking
Electrolyte
Filling
Total
Positive Electrode 99 95 99 99 92.2
Negative Electrode 99 95 99 99 92.2
Positive Current Coll. 99 92 99 90.2
Negative Current Coll. 99 92 99 90.2
Separator 98 98.0
Electrolyte 94 94.0


72
The estimated resources needed for scrap recycle are the following:
Rate Factor Direct
Labor
Capital Equip.* Plant Area, m2
Scrap Recycle
Scrap rate
6,320,000 cells/y 5 per shift 2.5 mil$ total
441 kg/shift
600
5.3.17 Baseline Plant Summary
The processing rates and the primary cost factors for the baseline plant are summarized in Table 5.4. The main processing rate for each step is shown in the second column. The requirements for direct labor, capital equipment and plant area, which are shown in detail in the subsections above, are summarized in the table. It is seen that the plant requires a total of 90 workers per shift, $127,450,000 worth of capital equipment, and 15,425 square meters of plant area to manufacture the baseline battery at a rate of 100,000 battery packs per year. 
5.4 Adjustment of Costs for Varying Production Volumes
Production volume may affect the end price of the battery in two distinct ways. First, the user of the model may change the annual production volume and every processing step will be affected. Somewhat differently, as the performance requirement and thus design is changed, the production of individual steps will change in non-uniform ways. As noted in Table 5.4, there are many processing rates that must be considered in addition to the overall number of battery packs manufactured per year. Each of these rates affects the costs of one or more steps in the process and may have no effect upon the costs of other steps in the process. For instance, when the user of the model increases the power of the battery packs without increasing the number of cells or their capacity, the model increases the area of the cells and decreases the electrode coating thicknesses. Such changes would result in an increase in the cost of the coating equipment, the floor area occupied by the equipment, and in the direct labor for that step in the process. It would have no effect on the cost of mixing the materials to be coated because the amounts of these materials per battery back are unchanged under the assumed conditions.
The general approach to cost estimation of multiplying a known cost by the ratio of processing rates raised to a power has also been applied to the capital cost of individual items of equipment.49
C = Co(R/Ro)p (5.2)
Here, Co is the capital cost of an installed equipment item designed for the baseline processing rate, Ro. The power factor, p, relates the capital investment cost and the processing rate for the manufacturing step.
If the value of p were 1.0, it would imply that the cost of the equipment item, or the equipment items if there are several in parallel, would be directly proportional to the processing rate. However, the value of p for the cost of equipment is frequently about 0.6 to 0.7 for many manufacturing process steps because the equipment is larger for the higher processing rates and its cost is less than if it were directly proportional to the processing rate. For process steps requiring the addition of many identical pieces of equipment for scale up, such as may be true for formation cycling of battery cells, the value of p may be as high as 0.9. The value of p is unlikely to reach 1.0 because the equipment cost includes installation, for which there is some savings even in installing multiple units of the same processing capacity. The relationships between cost and processing rate for two-fold and three-fold rate changes are illustrated in Table 5.6.

73
Table 5.6 The effect of processing rate (R) on cost for various scale factors
C/Co = (R/Ro)p
Cost Ratio, C/Co
Scale Factor, p R/Ro = 2 R/Ro = 3
0.25 1.19 1.32
0.3 1.23 1.39
0.4 1.32 1.55
0.5 1.41 1.73
0.6 1.52 1.93
0.7 1.62 2.16
0.8 1.74 2.41
0.95 1.93 2.84
1.0 2.00 3.00
Similar equations have been applied for determining the effect of processing rate on the annual hours of labor and the plant area required for a manufacturing step. In general, the value of p is low for the labor equation, usually only 0.4 to 0.5, because only a relatively small addition to the labor crew permits operation of larger equipment or of operating several more units of the same processing capacity.24 The value of p for the plant area required for a processing step is slightly less than that for equipment. The floor area required for larger equipment or for more equipment items of the same size is proportionately less than the increase in the processing rate because of the more efficient use of the space occupied by the equipment and the savings in aisle area. 
The value of the scale factors (i.e. p factors) for labor, capital equipment, and floor area were estimated for each of the processing steps (Table 5.4). The scale factors selected for the direct labor requirement are usually only 0.4 to 0.5, which indicates considerable unit cost reduction for increasing the plant throughput.
For most processing steps, increasing the processing rate beyond that in the baseline plant would result in a decision to increase automation or use faster equipment to mitigate the costs of higher levels of throughput. Decreasing the processing rate would have the opposite effect. Some steps in the process such as cell stacking, welding of current collectors, and formation cycling do not appear to be easily automated beyond the level intended in the baseline plant and, thus require a higher value for the scale factor of 0.8. This higher scale factor results in achieving fewer reductions in the cost per battery pack with increasing production volume. Additionally, a higher p factor results in a less severe penalty for lower production scale for an individual step in the
process.
There are five steps for which the cost of the capital equipment is affected by factors other than the main processing rate for the process step. These are discussed in the footnotes at the bottom of Table 5.4. For these steps, the costs that have been adjusted for the changes in the processing rate from the baseline rate are further adjusted to take into account the other cost factors. The cost of the coating equipment is adjusted for the amount of solvent to be driven off the positive and negative electrodes; thicker coatings need longer, more expensive ovens to drive off the additional binder solvent or the coater most be operated at lower speeds. The costs of the cell stacking equipment and the formation cycling equipment, for which the main cost factor in both cases is the number of cells to be fabricated annually, are also adjusted for the capacity of the cells; larger cells require more expensive equipment. The cost of the capital equipment for battery assembly is primarily a function of the number of cells in the battery, but it is also a function of the number of modules that must be interconnected. This dependence is accounted for in the model with an additional multiplying factor.
A breakdown of the baseline plant capital equipment costs listed in Table 5.4 is illustrated in Fig. 5.3. The largest costs for capital equipment are for formation cycling and testing, cell assembly (in the dry room) and electrode coating. These capital costs are likely to be dominant in any lithium-ion battery plant in the near future.
74
Figure 5.3 Breakdown of installed capital equipment costs for the baseline plant
7%
3%
15%
2%
1%
2%
1%
1%
28%
29%
9%
2%
Receiving and shipping
Materials preparation
Electrode coating
Calendering
Materials handling
Electrode slitting
Vacuum drying
Control laboratory
Cell assembly in dry room
Formation cycling and testing
Module and pack assembly
Rejected cell and scrap recycle

75
5.5 Plant Investment Costs
In this model, the calculated investment costs are defined as those directly related with building and operating the plant (Table 5.7). Other costs that may require investment, such as research and development, are added separately to the unit cost of the battery. The largest investment cost is for the installed capital equipment. Each cost item for the battery under design is adjusted from the estimate of the baseline plant. The plant cost is done in a similar way with a cost of $3,000 per square meter ($280/sq. ft) including land and utilities. The high cost for land and utilities accounts for both the area of the manufacturing facility as well as other land requirements such as office buildings and waste water treatment requirements. Launch costs include plant start-up, employee training and materials that are lost or recycled in early stages of production, beyond the normal amounts. Launch costs are estimated to be 5 % of annual materials costs plus 10 % of annual direct labor and variable overhead (Section 5.6). Working capital is needed to cover the costs of payroll, receivables, and the inventories of raw materials, work in progress and finished product. These working capital costs are partially offset by bills that are payable. We estimate the working capital to be 15 % of the annual variable costs. 
Table 5.7 Battery pack manufacturing investment costs
Investment Costs Description Method of Calculation
Capital Equipment Equipment costs including
installation
Estimates of costs for each
processing step at baseline rates
adjusted for actual rates.
Plant Floor Space Space includes aisles and space
for unfinished processing
inventory plus land and utility
costs.
Estimates of costs for each
processing step at baseline rates
adjusted for actual rates.
Launch Costs Plant start-up, training, out-of
spec product.
5% of annual materials cost,
10% of direct labor plus
variable overhead.
Working Capital Cash to meet payroll,
receivables, inventories of raw
materials and of unfinished and
finished product, minus
payables.
15% of annual variable costs.
5.6 Unit Costs for Battery Pack
The unit costs of the battery pack are calculated as summarized in Table 5.8.
5.6.1 Variable Costs
The costs of the materials and purchased items are based on the costs discussed in section 5.2, and the annual amounts of materials are adjusted for the yields of materials (section 5.3) and yield of cells. The direct labor is the sum of the labor cost for each step in the process, which are each calculated for the baseline plant and adjusted for the rate associated with the battery under study. Variable overhead is the cost of indirect materials and labor, utilities, and plant maintenance. It is estimated to cost 40 % of direct labor costs and 20 % of total depreciation.

76
5.6.2 Fixed Expenses
Fixed expenses include General, Sales, and Administration (GSA), research and development, and depreciation. The cost of GSA includes the plant office, taxes on income and property, cost of sales and insurance. It is estimated by the model as 25 % of direct overhead and depreciation. Research and development (R&D) must be carried out to ensure that the battery packs that are produced in the plant and the means of production continue to be competitive in the world market with respect to performance and price. The greater the investment in the plant and its equipment, the greater is the need to be successful in the R&D effort. Thus, the expenditure has been set at 40 % of the depreciation expense. Depreciation expense provides funding available for future investment in this plant or another venture to replace deteriorating plant and equipment. The equipment and plant are depreciated at straight-line rates for 6-year life (16.7 % per year) and 20-year life (5 % per year).

Table 5.8 Unit cost of battery pack
Variable Costs Description Method of Calculation
Materials and Purchased
Items
All materials and purchased items in finished product and lost in processing. 
Based on prices of materials, cost equations for purchased items and yields.
Direct Labor Labor costs for operations and immediate supervision.
Estimates of costs for each processing step at baseline rates adjusted for actual rates.
Variable Overhead Indirect materials, labor, utilities, plant maintenance
40% of direct labor cost plus 20% of depreciation 
Fixed Expenses
General, Sales, and
Administration (GSA)
Plant office, taxes on income and property, cost of sales and insurance expenses.
25% of direct labor and variable overhead plus 25% of depreciation.
Research and Development On-going research needed to upgrade product and maintain competitive position.
40% of depreciation
Depreciation Provides funds for new investments to replace those in current equipment and plant.
16.7% of capital equipment cost plus 5% of plant floor space cost.
Profit Return on invested capital after taxes.
5% of total investment costs.
Warranty Funds set aside for reimbursing customers for battery pack failures.
5.6% added to price based on present worth of projected payments.

77
5.6.3 Profits
The profit goal for this type of venture varies with the financial structure of the company, especially regarding long-term debt. For the model, the profit is set to provide a 5 % return on the total investment, which is an approximate average for mature manufacturing as vehicle battery production is expected to be in 2020. In general, the chosen cost structure and the resulting margin are similar to a Tier 1 supplier in the automotive industry. 
5.6.4 Battery Pack Warranty Costs
If a battery module or an entire pack fails, the replacement will cost much more than the original price paid by the OEM. It is important that such events are rare, but provision must be made to reimburse the vehicle owner, especially in the early years of the projected battery life. The extra costs of replacing the battery will result from labor for testing and replacing the battery, inventory costs for stocking replacement batteries, and servicing the battery controller if the new battery is slightly different than the old battery. It is likely that the battery manufacturer will be responsible for the cost of the new battery, which we assume will be equal to the cost of the original battery. The other costs of replacing the battery, to the extent that they are covered by the warranty, are assumed here to be covered by the automobile manufacturer and the dealer. The goal for average battery life is 15 years and a warranted life of 10 years, with full replacement in the first five years and shared cost of replacement for the last five years seems appropriate. The vehicle owner would pay an increasing share of the cost from between 0 % at 5 years to 100 % at 10 or more years. With these assumptions, the cost to the battery manufacturer will be equal to the present worth of the future costs of the new battery or modules as provided in the warranty. The rate of battery failure will vary over the life of the battery with a slightly higher rate early in life, then a low failure rate followed by a gradually increasing failure rate. For purposes of calculation we assume a failure rate of 1.0 % per year throughout the warranty  eriod. With an internal rate of return of 8 % and calculated on a monthly basis, the present value of the future costs would be about 5.6 % of the price of the battery before adding the warranty cost.
5.7 Summary of Baseline Battery Cost
The spreadsheet version of the model, which is discussed in more detail in sections 6 and 7, provides a summary sheet which is illustrated in Table 5.9 for the cost of the baseline battery and that of three others. This breakdown of the battery costs, with a brief summary of the design values, illustrates the effects of the cost factors. The second battery has twice the power of the baseline battery and the third battery has the same power as the baseline battery, but twice the capacity. The number of cells is the same for each battery. The energy storage is slightly higher for the battery with double power because the voltage would be slightly higher during the discharge to determine capacity. The battery with double the capacity has about the same number of electrodes; although, the electrodes are longer and wider in dimension, because the cell thickness is maintained. This results in a slightly higher resistance in the current-collector structure. The higher impedance lowers the voltage during the discharge capacity measurements and results in slightly less than twice the energy storage of the baseline battery.

78
Table 5.9. Summary of results for cost of baseline battery and that of similar batteries with
double the power and double the capacity of the baseline battery
Calculated Battery Parameters Baseline Double Power Double Capacity Double Modules
Vehicle electric range, miles 24.4 24.6 48.5 48.6
Number of battery packs 1 1 1 1
Packs in series or parallel
Number of cells per pack 60 60 60 120
Battery system total energy storage, kWh 8.7 8.8 17.3 17.3
Cell capacity, Ah 40.0 40.0 80.0 40.0
Cell group capacity, Ah 40.0 40.0 80.0 40.0
Module capacity, Ah 40.0 40.0 80.0 40.0
Pack capacity, Ah 40.0 40.0 80.0 40.0
Battery system capacity, Ah 40.0 40.0 80.0 40.0
Nominal battery system voltage (OCV at 50% SOC),V 221 221 221 442
Battery system power at target % OCV, kW 50.0 100.0 81.0 85.9
Required battery system power, kW 50.0 100.0 50.0 50.0
Target % OCV at full power 80.0 80.0 80.0 80.0
% OCV at full power adjusted for thickness limit 80.0 80.0 88.9 89.6
Battery system volume (all packs), L 37.4 43.2 61.3 66.2
Battery system mass (all packs), kg 63.3 78.1 112.3 117.7
Cooling system power requirement, W 616 251 348 335
Investment Costs
Capital equipment cost including installation, mil$ 128 146 158 205
Building, Land and Utilities
Area, m2 15,478 18,401 19,204 23,791
Cost, $/m2 3,000 3,000 3,000 3,000
Building investment, mil$ 46.4 55.2 57.6 71.4
Launch Costs
Rate: 5% of direct annual materials + 10% of other annual costs
Total, million$ 10.26 13.02 16.46 18.09
Working capital (15% of annual variable costs), mil$ 27.71 35.52 45.76 49.74
Total investment, mil$ 212.10 249.45 277.97 344.20
Summary of Unit Costs, $
Materials 1,245 1,706 2,329 2,342
Purchased Items 397 426 481 671
Direct Labor 113 130 130 162
Variable Overhead 92 106 111 140
General, Sales, Administration 110 127 133 170
Research and Development 94 108 117 151
Depreciation 236 270 292 377
Profit 106 125 139 172
Warranty 134 168 209 234
Price to OEM for battery pack, $ 2,528 3,166 3,941 4,421
Pack integration (BMS & Disconnects), $/pack 395 395 395 475
Total battery cost to OEM, $ 2,923 3,561 4,336 4,896
Additions to AC for thermal management, $ 240 200 200 200
Total cost to OEM for complete system, $ 3,163 3,761 4,536 5,096
Price to OEM for modules for one pack, $ 2,364 2,977 3,734 4,204
Error bars on price to OEM for battery pack, %
Potential positive error, % 21 10 31 26
Potential negative error, % 10 10 16 15

Doubling the power does not add as much cost to the materials and purchased parts as doubling the cell capacity. Most of the labor costs for the first three batteries are similar with the major difference being for the labor cost for electrode processing. The double power battery requires greater labor costs principally for coating the larger electrode area. Capital equipment and depreciation costs are higher for both the high power and high capacity battery packs. The increases in capital equipment cost for the high-power battery are for coating, calendering, materials handling and vacuum drying equipment. For the high-capacity battery, the main additional capital equipment costs are for the materials mixing, binder solvent recovery, cell stacking and formation cycling steps in the process. 
Overall, doubling the power of the battery increases the price of the battery pack by only 25 %. Doubling the capacity of the cells increases the cost by 56 %, considerably more than for doubling the power. Alternatively, doubling the number of baseline cells and modules within a larger battery jacket (two rows of modules instead of one, twice the voltage, energy, and power) would increase the cost by 75 %.
The summary of unit costs for the baseline battery pack, which is shown at the bottom of Table 5.9, is illustrated in Fig. 5.4. The materials and purchased items are the largest costs for the battery. For larger levels of production, these costs are even more dominant because the scale factors for these items are close to one.
Figure 5.4 Breakdown of unit costs for baseline battery with total price to OEM of $2528. The total battery cost to the OEM, including pack integration components but excluding thermal management external to the pack, is $2,923.
49%
16%
5%
4%
4%
4%
9%
4%
5%
Overall Cost Breakdown
Materials
Purchased Items
Direct Labor
Variable Overhead
General, Sales, Administration
Research and Development
Depreciation
Profit
Warranty

80
5.8 Uncertainties in Price Estimates
The potential uncertainty in estimating the price of future Li-ion batteries depends upon many factors. In BatPaC, the error bars for the 95% confidence intervals for the price charged to an OEM for the battery pack are automatically calculated. The uncertainty ranges are specific for the performance requirements of the battery. The three major categories of uncertainty in the default calculation of battery price are:
* Input costs of materials and capital equipment
* The maximum allowable thicknesses of the electrode coatings
* The maximum capacity of single cells
An in-depth variation study analyzing the contribution of these categories to the battery price to the OEM has been completed. The details and methodology used in that study may be found in the Appendix.
5.8.1 Materials and Capital Equipment
A variation study was made of the cost inputs for the top eight contributors to total battery price including the active materials, copper current-collector foil, electrolyte, separator, and SOC controllers (see Appendix). The costs of capital for electrode coating and formation cycling were also varied. Both of these are subject to considerable variation due to unforeseen quality difficulties or advances in process throughput. The high, median, and low costs were considered for each of the factors, sometimes over 100% higher in value. Normal or log-normal random distributions of these values were used to calculate a population of batteries with differing price. Analyzing the resulting uncertainty in end battery price, a range of +/- 10% was found to capture the 95% confidence interval of the total price for several different cell chemistries and for HEV, PHEV, and EV battery packs.
5.8.2 Electrode Thickness
Most of the current transportation Li-ion batteries have electrode coatings of about 20-60 micron thickness; whereas, some consumer electronic applications may have 120-micron thick electrodes. As batteries are sought for vehicles with useful electric ranges (low power-to-energy requirement), there is a strong incentive to save cost by increasing the thickness of the electrode coatings as discussed previously in section 3.6.1. In BatPaC, a 100-micron default electrode thickness limitation is assumed. If the calculated optimal thickness is less than 100 microns, then the optimal calculated thickness is used. If the optimal thickness is greater than 100 microns, BatPaC increases the area of the cell to meet the energy requirement while maintaining an electrode thickness of 100 microns. After continued engineering development, the appropriate thickness limitation may be greater or less than the default assumption. The model estimates this uncertainty by calculating the total costs for batteries having electrode thicknesses limits at the 95% confidence limits, namely 50 and 150 microns for PHEV cells and 70 and 200 microns for EV cells. EV cells typically operate at lower P/E ratios than PHEVs and thus are more likely to successfully utilize electrodes of larger thicknesses. The costs so calculated determine negative and positive percentage uncertainty added to the base value of 10 % discussed in section 5.7.1.

81
5.8.3 Cell Capacity
Vehicle designs requiring batteries with large energy storage (e.g. EVs) commonly rely on high capacity cells or cell groups, exceeding 50 Ah. Cells of this size and larger (e.g. 200 Ah) exist today for some applications and cell chemistries. However, an OEM may choose to use smaller cells grouped by parallel connection. These smaller cells may have already been demonstrated to meet the performance, life, and safety requirements for a particular application and thus are a more attractive choice for the OEM. It is difficult at this time to predict the largest cells that will be practical for a particular application in the near future and, thus, BatPaC does not limit the cell capacity. However, as the cell capacity calculated to meet the energy requirement increases, the likelihood of the designers using parallel connected cells in a group also increases. This uncertainty in additional cost is taken into account by increasing the size of the positive error bar. Additional parallel cells increase the cost because of the increased number of cell terminals, interconnects, and formation cycling units in the manufacturing facility. Details on these costs are discussed in section 7.3.
To calculate the cost uncertainty from lowering the capacity of individual cells, BatPaC sets a capacity of 50 Ah below which there is no addition to the error bar. At 100 Ah or above the error bar is that for the additional cost of using half the cell capacity and doubling the number of cells with two cells in parallel. Between 50 and 100 Ah the error bar is calculated as 2% of the additional cost for the smaller capacity cells in parallel for each Ah above 50 Ah. 
5.8.4 Example of Contribution to Calculated Uncertainty
The uncertainties in the cost estimates are calculated in the worksheet “Error Bars”, in which, BatPaC recalculates the cost of the battery pack with the maximum electrode thicknesses and the capacity set at what we estimate to be the 95% limits and compares the results with that for the default values, resulting in contributions to both positive and negative error bars. An example is illustrated in Fig. 5.4 for a 120 kW 360V EV battery based on the NMC441-Gr chemistry having a vehicle range of 80 to 200 miles. As the range is increased, both the thickness of the electrodes and the capacity of the cells increase. No uncertainty from the electrode thickness limitation is added for calculated electrode thickness less than 70-micron. As the thickness increases, the positive uncertainty increases. Above 100 microns in thickness (default assumption), a negative uncertainty is added on the assumption that the actual thickness limit may be as high as 200 microns. Similarly, the effect of the uncertainty derived from the cell capacity is not a factor for capacities less than 50 Ah. A contribution to the positive uncertainty is accounted for as the capacity increases above that level. In summary, for this example, the battery price uncertainty ranges are plus 10% and minus 10% for the vehicle with 80-mile range, and plus 26% and minus 18% for the vehicle with 200-mile range.


Figure 5.5 Effects of electric-vehicle range on price and error bars for battery pack with
NMC441–Gr cell chemistry, 120-kW 360 V.

82
5.9 Breakdown of Costs
BatPaC assists in showing the relative importance of cost items by providing cost breakdowns from several perspectives as detailed in the Cost Breakdown worksheet. The costs are distributed in several ways and then graphed with pie charts to illustrate the relative importance of the cost items. This is a useful way of judging the importance of cost items. 
This worksheet is illustrated below with the sample cases provided in BatPaC v2.0 as distributed. The sample batteries are PHEV batteries all with 60 LMO-G cells and power of 60 kW. They range in energy from 4 to 16 kWh and provide an electric range of about 10 to 42 miles for vehicles requiring energy of 250 Wh/mile.
The first set of graphs for Battery 1 (4.0 kWh) and Battery 7 (16.0 kWh) shows the overall distribution of costs as calculated in the “Summary of Results” worksheet. (The modeler may change the selection of battery on the chart by selecting the pie image on the chart and then changing the Excel column for the cost values.)

29%
24%
7%
5%
6%
5%
13%
6%
5%
Overall Cost Breakdown
Battery 1
Materials
Purchased Items
Direct Labor
Variable Overhead
General, Sales, Administration
Research and Development
Depreciation
Profit
Warranty (includes battery pack(s) only)
49%
16%
4%
4%
4%
4%
10%
4%
5%
Overall Cost Breakdown
Battery 7
Materials
Purchased Items
Direct Labor
Variable Overhead
General, Sales, Administration
Research and Development
Depreciation
Profit
Warranty (includes battery pack(s) only)


83
Figure 5.6 Overall distribution of costs of manufacturing battery packs, not including pack integration system.
These graphs illustrate that materials and purchased items compose a large fraction of the total battery pack price for a mature battery plant producing 100,000 packs per year. This effect is stronger for the 16-kWh battery (Battery 7), which has a large fraction of expensive cell materials, than for the smaller 4-kWh battery.
The second set of graphs illustrates the breakdown of costs for the materials and purchased items only. For the 16-kWh battery (Battery 7), the costs of active materials and electrolyte are substantial. It should also be noted that the cost of separator material is greater than the total costs of the current collection foils. The fraction of cost required for active materials is larger for the 16-kWh battery than for the 4-kWh battery because the cell capacity is larger and the electrodes are thicker.

.
12%
8%
1%
3%
8%
15%
8%
7%
27%
11%
Materials and Purchased Items Cost Breakdown
Battery 1
Positive Active Material
Negative Active Material
Carbon and Binders
Positive Current Collector
Negative Current Collector
Separators
Electrolyte
Cell Hardware
Module Hardware
Battery Jacket
18%
13%
2%
17% 9% 4%
12%
4%
13%
8%
Materials and Purchased Items Cost Breakdown
Battery 7
Positive Active Material
Negative Active Material
Carbon and Binders
Positive Current Collector
Negative Current Collector
Separators
Electrolyte
Cell Hardware
Module Hardware
Battery Jacket


84
.
Figure 5.7 Distribution of materials and purchased items for the battery pack.
Sections 5.5 and 5.6 discuss the derivation of fixed and variable overhead costs by the use of multiplying factors on the costs of (1) materials and purchased items, (2) direct labor, (3) capital equipment, and (4) building, land and utilities. These overhead costs can be redistributed back to their origins by applying the constant multipliers shown in Table 5.10 which is a reproduction from the “Cost Input” worksheet.
The next set of charts (Fig 5.7) in the printout of the Cost Breakdown worksheet, shows the distribution of the price of the battery pack to materials, purchased items, and the individual manufacturing processes and operations.


Table 5.10 Table for converting overhead costs back to their origins
Multipliers for Overhead to Basic Costs
Multiplier
Materials and purchased items, $/pack 1.0666
Direct labor, $/pack 1.8665
Capital equipment (100K packs/yr*) 3.8764
Building, land, utilities (100K packs/yr*) 1.5325
*For other production rates multiply by 100,000/rate
Basic Cost Factors
31%
9% 26%
13%
11%
6%
2%
2% 0%
Cost Breakdown with Overhead Distributed to Processes
Battery 1
Materials, $
Purchased items, $
Manufacturing, $
Electrode processing
Cell assembly
Formation cycling, testing and sealing
Module and battery assembly
Cell and materials rejection and recycling
Receiving and shipping
Control laboratory
52%
17%
10%
7%
7%
3% 1% 2% 1%
Cost Breakdown with Overhead Distributed to Processes
Battery 7
Materials, $
Purchased items, $
Manufacturing, $
Electrode processing
Cell assembly
Formation cycling, testing and sealing
Module and battery assembly
Cell and materials rejection and recycling
Receiving and shipping
Control laboratory

85
Figure 5.8 Distribution of overhead costs to materials, purchased items, and individual processes.
The materials and purchased item costs have a small effect on overhead cost, namely launch costs and working capital costs. Thus we have distributed back to the materials and purchased items a small amount, which accounts for the fraction of the cost of materials and purchased items being slightly higher in the charts of Fig. 5.7 than in those of Fig. 5.5. The other costs are redistributed to the individual processes and operations. 
The costs of the three major manufacturing operations of (1) electrode processing, (2) cell assembly, and (3) formation cycling, testing and sealing estimated by BatPaC for a Control laboratory manufacturing scale of 100,000 battery packs per year in 2020 is considerably lower than their actual costs at the time this report is in writing. If these projected costs are reached, there can be only small percentage reductions in cost after that by further optimization and automation for even larger scales of production, unless there are substantial reductions in materials costs.
In Fig. 5.8, the costs are distributed to the basic cost factors of (1) materials, (2) purchased items, (3) labor, and (4) capital equipment and building by means of the factors in Table 5.10.

86
Figure 5.9 Redistribution of costs to basic cost factors
The total effects of the direct labor costs are greater than indicated in Fig. 5.5 because of the influence of labor costs on overhead as shown in Fig. 5.8. Foreign battery plants may have lower labor cost than plants in the United States, which may give them an advantage even considering shipping costs. However, the advantage would be small and further automation may overcome such an advantage.
Clearly, the major opportunities for cost reduction are in the area of materials costs. Improvements may be in lower costs per unit weight of material or in higher performance, greater power or greater capacity per unit weight for materials of nearly the same cost as set in BatPaC.
Materials
36%
Purchased items
23%
Labor
12%
Capital Equipment
and Building
29%
Breakdown of Costs to Basic Cost Factors
Battery 1
Materials
52%
Purchased items
17%
Labor
8%
Capital Equipment
and Building
23%
Breakdown of Costs to Basic Cost Factors
Battery 7

87
6 Description of the Spreadsheet Model and Instructions for Use
6.1 Background
Historically, the model has been based on Microsoft® Office Excel spreadsheets. The flexibility afforded by a spreadsheet approach has been extremely useful to the development of the calculations. Until recently, the model had been in a constant state of development. Changes to parameters and equations were made rapidly and frequently. The publication of the BatPaC v1.0 report represented the first time a version of the model was be “frozen” for open distribution to the public. Advances will continue to be made with the model beyond this current v2.1; however, distributions of the revised model will be made in an orderly fashion rather than the continuous improvement approach taken over the last number of years.
6.2 Instructions
The following subsections are a brief explanation of how one may operate the spreadsheet based model. The user is advised to save the original document separately as a back-up copy. Corruption of the calculation is possible and will likely occur during use by someone unfamiliar with the model.
6.2.1 Enabling Calculation
This Microsoft® Office Excel workbook requires the use of iteration. The iterative function may be enabled by going to File > Options > Formulas. Check the box next to “Iteration” and change the maximum number of iterations to 1000 (Figure 6.1). Perhaps most importantly, ensure the calculation is set to automatic and not manual. If the iteration is not turned on, the software will  resent an error complaining about circular references. If the model is opened while a different Excel spreadsheet is in use, the software will also warn of an error. Simply close all Excel windows except for the model; alternatively, one could re-enable the iterative function as discussed above.
6.2.2 Chem Worksheet
The cell chemistry is selected by copying the system designated at the top of a column, for instance NCA-G in cell F4, pasting it into cell E4 (Figure 6.2). Any of the values in column E can be overridden by entering the desired value in column M. For example, the maximum electrode thickness may be overridden by placing a new value in cell M53. The selection of the cell chemistry also includes the associated prices at the bottom of the page. These prices can also be overridden by entering the desired values in column M. A full screen shot of the system selection worksheet is in Figure 6.3.
6.2.3 Battery Design Worksheet
The Battery Design worksheet designs seven or more batteries for any type of electric-drive vehicle (Figure 6.4–6.6). The calculated designs are specific for the end battery requirements specified by the user. From the result, the amounts of materials and the purchased items required for manufacture are easily available to be used in the manufacturing cost calculations found on subsequent worksheets. Although a cell and module format is assumed, the exact format (prismatic, pouch, can, etc) of the battery does not have a dominant effect on the cost for a set cell chemistry system. Our experience teaches us that the amounts of electrode materials and the number, capacity and electrode area of the cells, are the determining cost factors. Nevertheless, a specific design format was selected and is shown on the Cell Design worksheet to provide a basis for calculating the entire cell and battery related costs.
88
Figure 6.1 Automatic iteration must be enabled for the spreadsheet model to function.
Figure 6.2 The specific cell chemistry for the battery design is selected on the Chem worksheet.
89
Figure 6.3 Chem worksheet
90
Figure 6.4 Top portion of Battery Design worksheet.
91
Figure 6.5 Middle portion of Battery Design worksheet

92
The Battery Design worksheet automatically receives input from the Chem worksheet. These values are shown in purple (Figures 6.4 and 6.6) and must not be altered on the Battery Design worksheet. As explained above, cell chemistry values may be adjusted on the Chem worksheet. The operator provides battery design input in the aqua colored cells (Figures 6.4 and 6.6). The battery input parameters on lines 54 to 62 (Figure 6.4) and lines 179 to 181 (Figure 6.6) are the only input values that the operator is required to provide to study a group of batteries. The type of vehicle battery (microHEV, HEV-HP, PHEV, or EV) on line 51 in Figure 6.4, is another important variable to be specified. One performs the selection by typing the name of the vehicle battery type in cell F51. While the correct spelling is important, capitalization is not. This selection automatically determines the state of charge at which full power is designated (thus, the open-circuit voltage and ASI for full power) and the length of the power burst (2 seconds for microHEV and 10 seconds for all others). It is expected that the majority of the remaining default values should serve well for most batteries; however, the user may also change to their exact specifications. The thermal management approach is selected on line 52 in Figure 6.4. One can select between a thermal management approach using liquid (EG-W), cabin air (CA), or conditioned cabin air (CoolA). The different module and battery formats for air and liquid cooling are displayed in later worksheets of BatPaC. 
The cell capacity (lines 179 to 181 in Figure 6.6) can be set in any of three ways: (1) directly specifying the capacity (Ah) on line 179, (2) specifying the total battery energy on line 180 or (3) specifying the electric range of the vehicle (miles). Only one of the three lines should be filled in and the others should be blank. The model will follow the directions of the top-most line with non-zero values.
The number of batteries manufactured per year is selected on line 68 in Figure 6.4. Changing this value from the default value of 100,000, which is the manufacturing rate for the baseline plant, will change the manufacturing cost.
If it is desired to study more than five batteries in the same workbook it is only necessary to add additional columns by copying the battery 7 column to the right as many times as desired. Care should be taken that the appropriate values are maintained when the cells are copied over. The qua colored cells are typically the source of any problems. The same column additions must also be done for all other worksheets containing calculations.
6.2.4 Remaining Worksheets
The cost calculations are done on the Manufacturing Cost worksheet and the results for the model are shown on the Summary of Results worksheet (Figure 6.7). No parameters need to be entered on these worksheets by the operator; all of the input for these worksheets is from the Battery Design and the Cost Input worksheets. Tables for presentations or for preparing graphs of the data can be assembled at the bottom of either the Battery Design or the Summary of Results worksheet. These tables can be transferred to a blank worksheet for more complex studies. For instance, results for different cell chemistries can be copied and pasted (special paste, values and numbers formats) to a blank worksheet. On the last worksheets, the cell, module, and battery design, as well as the baseline plant are sketched.

93
Figure 6.6 Bottom portion of Battery Design worksheet

94
Figure 6.7 Summary of Results worksheet

95
6.3 Battery Design Format Requirements
As the battery design is based off an assumed format (Section 2), certain design requirements are necessary to ensure the modeled battery is physically realistic. The dimensions of the calculated battery pack should be examined. Some final designs may benefit from changing the cell aspect ratio, H/W, to fit the end-use application. One example would be, to reduce the height of the battery pack by increasing the cell H/W ratio. Also, for a set number of cells in the pack, changing the number of rows of modules, allows for adjustment of the pack dimensions.
6.4 Troubleshooting and General Advice
The spreadsheet iterates to find the solution and this sometimes causes error messages to appear after an entry is changed. These errors can usually be removed by first correcting any erroneous entries (non-numeric, two decimal points, etc.). Then the cells may be reset to default values by entering a “0” (i.e. zero) in the restart cell, F188 in Figure 6.6. Finally, entering a “1” in F188 restarts the iteration process leading to a successfully converged answer. 
At some point, a user will ask the model to design a battery that is outside the bounds of what is allowable for the selected cell chemistry. The most common error is when too large of a P/E ratio is requested. Two different physical limitations are approached with increasing P/E ratio. First, the electrode thickness is shrinking. At some point, the value will become unrealistic and eventually approach 0 crashing the calculation. At the same time, the C-rate for the active material is approaching the limiting C-rate defined in the Chem worksheet. As this value is approached, the ASI will increase to larger and larger values, which thus demands smaller and smaller electrode thicknesses. Eventually, the calculation will crash.
A warning has been added to BatPaC in row 72 of the Battery Design worksheet. A red “X” will appear if the capacity is too low to meet the power required by the user. The warning is triggered if the ASI for power is calculated to be more than 50% the default level (see cell E45 on Chem worksheet). Common sense approaches to resolve these issues are to use lower designed power or higher designed energy. The C-rate and electrode thickness are easily viewed in the model output. These are found on the Battery Design worksheet in row 139 for the C-rate and rows 94 and 95 for the electrode thickness. Therefore, the user may try designs of increasing P/E ratios and watch to see how the electrode thickness and C-rate is changing. Different cell chemistries will have different sensitivities to the P/E ratio depending on the defined limiting C-rate, rC,lim, and calculated ASI for power. What is possible with the LMO-G system will not always be possible with the NCA-G system. P/E ratios that satisfy the expression in Eq. 6.1 generally result in successful battery designs. Higher P/E ratios are allowable in some situations. Note that selecting the microHEV design doubles the allowable C-rate since only two second pulses are used. The limiting C-rate, rC,lim, may be found in cell E44 on the Chem worksheet and is carried over to row 77 in the Battery Design worksheet.
1.35
rC,lim
P E
 (6.1)

96
6.5 Suggested Number of Cells, Modules, and Performance Inputs
Table 6.1 presents some suggestions for the required inputs into the design model that might change depending on the type of vehicle battery being designed. These values are only suggestions, but tend to be similar to practices used today or projected to be used in the future by industry. If the calculated cell capacity is higher than 60 Ah, the user should consider the inclusion of parallel cells as an additional parameter to examine. The default energy usage rate in BatPaC is 300 Wh/mi. This rate may be used to size the energy requirement based on a desired electric range for the vehicle by specifying the distance in row 164 on the Battery Design worksheet.
Table 6.1 General suggestions for range of input parameters that change with battery type
battery type modules/battery OCV @ 50% SOC Power (kW) Energy (kWh)
HEV-25 1 - 4 40 - 200 25 0.6 - 1.5
HEV-HP 2 - 4 160 - 260 25 - 80 1 - 2
PHEV 4 - 6 290 - 360 40 - 160 4 - 30
EV 4 - 6 290 - 360 80 - 160 20 - 200

6.6 Entering a New Material Couple
The user of the model may wish to examine an electrochemical couple that is not included as one of the options available in the model. We list below a brief explanation on how to properly enter new materials into BatPaC. Various properties may be calculated, found in literature or measured in the laboratory. The self-consistency of the data used is very important.
Experimentally measured values required:
1. Half cell formation cycling data from positive and negative electrode
2. Half cell cycling data from positive and negative electrode at C/3 rate
3. Full cell open-circuit voltage measurement at 50 % and 20 % SOC
4. Full cell ASI measurement for 5C pulse at 50 % and 20 % SOC
5. Full cell ASI at 50% SOC during a C/3 discharge
6. Electrode void fractions, active material densities, electrode component weight percent
7. Estimated interfacial area from surface area (preferred) or particle size measurements
The ASI calculation includes some additional parameters that become important as the designed P/E ratio increases above 10 h-1 or the electrode thicknesses decrease below 30 microns. The user is referred to section 3.4 and the supporting manuscript from Gallagher et al.20 for the parameter estimation process. An exchange current of 0.15 mA/cm2, normalized to the surface area  alculated using the BET method from nitrogen absorption experiments, is used in the model in row 77 in the Battery Design worksheet. While the exact value of the exchange current will vary from the material to material, the general behavior of the ASI will be preserved with this assumption. If lower P/E ratio designs are desired, the exact valuation of the exchange current, interfacial area, and limiting C-rate are less important. However, the experimental ASI measurement should then come from a cell with similar P/E ratio (electrode loading). Electrode thicknesses 40 microns or larger should be used to minimize the contribution of interfacial impedance to the ASI measurement. Otherwise the “ASI correction factor” may not accurately remove the interfacial component. A reasonable approach for a first approximation of the ASI parameters may be to select the same values for a similar material. For example, if the new material is based on nano-sized primary particles, then the parameters for LFP or LTO may be close enough. The ASI does depend on a large number of factors and a full determination of the parameters is important to capture all of the physical behavior of the cell couple. If the desire of user is to reproduce an existing cell, then many of the parameters may be estimated from the electrochemical characterization of the full cell data. These electrochemical results typically require a teardown of the cell to measure the area of the electrodes and their loadings/thicknesses.

97
The available lithium for cycling in a full cell configuration may be calculated from half cell measurements. The calculation method may be found in the Capacity Calculator worksheet in the spreadsheet model and is detailed below. Alternatively, the reversible capacity of the full cell in the experiment may be normalized to the mass of the positive and negative electrodes while carefully accounting for the negative to positive capacity ratio. The first cycle efficiency of a positive or negative electrode based half-cell may be defined as the ratio of the first discharge capacity divided by the first charge capacity, Equation 6.2. We have assumed the first discharge capacity is equivalent to the reversible capacity when measured against lithium foil (half-cell arrangement).
st
j
rev
st j
j Q
Q
1
1
  (6.2)
The quantity of lithium consumed from the positive electrode in the negative electrode SEI, Qsei, may be calculated from Equation 6.3. Here, [N/P] is the negative to positive capacity ratio.
    N irrev
N P
rev
N
st
rev N
N
rev
sei P Q
m m
Q Q
Q Q
Q  N/P 1   (6.3)
After one full cycle, the remaining lithium in the positive electrode available for cycling, QPact, in a full-cell configuration (positive electrode versus non-prelithiated negative electrode) may be calculated by choosing the minimum value determined in Equation 6.4 below. Here we see the possibility that the positive electrode is unable to accept the full amount of lithium released during the first charge cycle. This so called “irreversible capacity” of the positive electrode results in lithium residing in the negative electrode. While this excess lithium may require additional negative electrode capacity, it also provides some beneficial aspects to cycle and calendar life.50 We have chosen to set the [N/P] = 1.25 for layered oxides positive electrodes (NCA, NMC441, NMC333) due to their tendency to have a lower first cycle efficiency ~ 88%. The lithium manganese spinel and lithium iron phosphate cells have a high first cycle efficency and thus we selected a [N/P] = 1.20. For positive electrodes with a high first cycle efficiency, the reversible capacity of the cell is reduced by the lithium consumed in the graphite electrode SEI during the formation cycle. Conversely, the lithium titanate spinel negative electrode does not form an SEI and is significantly safer than the graphite electrode as discussed in Chapter 5. Thefore the [N/P] ratio is set to 1.1 for the cells based on lithium titanate spinel.

98
 







  
 
QP act  MIN QP rev 1    1  1 Pst1 Pst N/P 1 1 Nst1 Nst ,QP rev (6.4)
6.7 Entering Parallel Cell, Module, or Pack Configurations
The provision for specifying multiple modules and multiple packs was added to the worksheet “Battery Design” and the equations throughout the spreadsheet were altered as necessary. To implement parallel cells, the user must designate the number of cells in parallel and increase the number of cells in a module accordingly. The model program will automatically select a cell thickness of 6 mm, which is half the thickness selected by the model for EV cells if all are connected in series. Because of the larger number of cells, the price of a battery with parallel connected cells is higher than that for the battery of all series connected cells. To select a parallel module configuration, the user of the model must increase the number of modules and select the desired number of modules in parallel. The cost of the parallel modules is more than that of an equivalent battery with parallel cells because of costs for extra module hardware especially for the extra circuits for SOC regulation.
To a parallel battery pack setup, the user must first configure the battery packs, remembering that each pack provided only a part of the energy, and then select the number of packs and designate whether they are in parallel or series connection. The user must also determine the capacity of the pack at the bottom of the “Battery Design” worksheet. The user makes this determination by selecting one of the following: (1) the pack capacity (note: not the cell or total battery system capacity), (2) the pack energy, or (3) the range of the vehicle. For Table 1, we selected a 100 mile range for all five sample battery systems. The battery system with series-connected packs has twice the voltage and half the system capacity than for a parallel pack configuration.

99
7. Illustrated Results
The BatPaC model may be used to study the effects of battery parameters on the performance and the manufactured cost of the designed battery packs. A few examples are given below for the effects of various parameters on battery pack volume, weight and cost.
7.1 Number of Cells in Series
For a set battery pack power, the number of cells in the pack has substantial effects on the price of the pack, the pack voltage and the maximum current. These effects are illustrated (Figure 7.1) for LMO-Gr PHEV20 batteries (providing 20-mile electric range) with 60-kW power at a [V/U] = 0.8. The total battery cost to the OEM increases by 15% in changing the number of series connected cells in the pack from 48 to 96. The integrated cost includes battery management system with disconnects in addition to battery price. The change in the maximum current, resulting from differing pack voltages, would also affect the cost of the motor and the electronic converter and controller, but in the opposite direction. As a result of these offsetting effects on the total cost of the electric drivetrain, a study is required to determine the optimum current at rated power as a function of the total battery pack power and other parameters. 
Figure 7.1 The effect of the number of series-connected cells for LMO-Gr, 60-kW, PHEV20 packs with 8 kWh total energy (70% useable).
Current PHEV and EV battery technology uses battery packs containing 80-96 series connected cells. However, these series connections are often composed of parallel cell groups. For instance, the battery used in the first production model of the Chevrolet Volt is in a 3P-96S configuration.21 Three low capacity cells are connected in parallel forming a parallel cell group. Then 96 parallel cell groups are connected in series. The cost savings from moving to larger format cells with only series connections is discussed later in this section. 
0
100
200
300
400
500
600
700
800
2000
2200
2400
2600
2800
3000
20 40 60 80 100 120
Current (A) or Voltage (V)
Total battery cost to OEM, US$
Number of series connected cells
Cost
Nominal Voltage
Max Current


100
7.2 Cathode Materials
Lithium-ion batteries for high mileage PHEVs and EVs do not require a high P/E ratio or low ASI to meet their goals. The most important material properties for performance are high specific capacity (mAh/g), high cell voltage, and high electrode density. Graphite electrode is near universal in commercial cells as a negative electrode, although not all graphite is the same. Here we consider changes in the positive electrode that result in significantly different calculated batteries. To compare the performance of EV battery packs made from various Li-ion chemistries, we designed the packs to provide 150 kW at 360 V (20% SOC) for a [V/U] = 0.8. Each pack consisted of six modules containing 16, 16, and 18 cells for the cell chemistries LMO Gr, NMC441-Gr, and LFP-Gr, respectively. This calculation assumes that large capacity cells may be reliably produced. Moving to a parallel connection of smaller capacity cells would result in higher cost as discussed later in the section.
The NMC441-Gr system has excellent energy density and low cost (Fig. 7.2 and 7.3). The LMO Gr system is less energy dense than the NMC441-Gr couple, but equivalent in calculated price to the OEM. The LFP-Gr system results in a battery that is larger and more expensive than the other two chemistries. The mass-specific cathode raw material prices are 26, 20, and 10 $/kg for NMC441, LFP and LMO respectively. The differences in cathode materials costs do not directly translate to the end cost of the battery. The performance (exhibited by specific capacity and voltage) affect the quantity of both active and inactive material required. The NMC441 material achieves 175 mAh/g at a good cell voltage and is representative of an advanced, although close to commercialization, layered oxide cathode.51 The combination in voltage and capacity results in a superior energy density compared to the other cathodes. The LMO cathode has similar cell voltage to NMC441 and low raw material cost but also a low specific capacity of 100 mAh/g. This low capacity results in a positive electrode loading limited by the maximum achievable electrode thickness ~100 microns. The LFP electrode has moderate capacity, 150 mAh/g, and raw material cost, but exhibits a lower cell voltage and electrode density. These poor performance characteristics result in a low energy density battery with a high price. 
7.3 Parallel-Connected Cell Groups and Electrode Thickness Limits 
BatPaC also allows the user to create parallel cell groups and to set a maximum electrode thickness. The effect these two unique design factors have on battery price are illustrated below in Figure 7.4 for the LMO-Gr and NMC441-Gr systems. In this illustration, the PHEV battery pack design parameters are 100 kW of power at a [V/U] = 0.8 and 17 kWh of total energy. The nominal battery pack voltage (OCV at 50% SOC) is around 360 V from 96 cell groups connected in series. The number of cells in the parallel cell group is varied from a single cell (no parallel connections) to four. Two maximum electrode thicknesses of 100 and 200 microns are shown for the LMO-Gr chemistry. In contrast to the NMC441-Gr, the LMO-Gr chemistry benefits from allowing larger electrode thicknesses. The thickness of the positive electrode is limiting the LMO-Gr chemistry while the thickness of the negative electrode limits the NMC441-Gr cells.

100
150
200
250
300
350
400
450
500
50 100 150 200 250
Battery pack mass (kg)
Vehicle range (mi)
LFP-Gr
LMO-Gr
NMC441-Gr
0
50
100
150
200
250
300
50 100 150 200 250
Battery pack volume (L)
Vehicle range (mi)
LFP-Gr
LMO-Gr
NMC441-Gr

Figure 7.2 Mass and volume of electric vehicle battery packs with lithium iron phosphate (LFP), lithium manganese-spinel (LMO) and lithium nickel-manganese-cobalt oxide (NMC441) positive electrodes versus graphite designed to deliver 150 kW of power at 360 V (20% SOC).

60006000
7000
8000
9000
10000
11000
12000
13000
14000
15000
50 100 150 200 250
Total battery cost to OEM (US$)
Vehicle range (mi)
LFP-Gr
LMO-Gr
NMC441-Gr
7000
8000
9000
10000
11000
12000
13000
14000
15000
50 100 150 200 250
Total battery cost to OEM (US$)
Vehicle range (mi)
LFP-Gr
LMO-Gr
NMC441-Gr

101
Figure 7.3 Total battery cost to OEM for LFP-Gr, LMO-Gr and NMC441-Gr battery packs for same designs as in Fig. 7.2. NMC441-Gr and LMO-Gr result in nearly the same price.
The calculated value for the NMC441-Gr system never exceeds 100 microns for this P/E ratio. The LMO-Gr is the least expensive in all cases. However, the difference between the two chemistries lessens with smaller limiting electrode thickness. The costs will become even closer for lower designed P/E ratios. In general, thicker electrodes reduce the cost of the battery pack by lessening the amount of inactive materials used (separator, current collector, etc). Moving to 200 microns allows for greater savings in the LMO-Gr design but not the NMC441-Gr design. However, a lower P/E ratio design for NMC441-Gr would take advantage of electrode thicknesses greater than 100 microns.

102
The cell capacity is shown for the NMC441-Gr case limited to 100 microns. While the exact values will change with cell chemistry, they will all be similar. The cell capacity is reduced by one half as a single cell is added in parallel. This approach is commonly used by cell manufacturers and OEMs that cannot reliably produce or successfully operate cells of high capacity for transportation applications. However, this approach also increases the price of the battery pack. In this example, the price is increased by ~ $500 when an additional string of cells is incorporated in a parallel arrangement.
The model calculations show that the lowest cost battery pack will utilize thick electrodes and large capacity cells. In current practice, these two approaches have yet to be successfully implemented within the entire community. In the challenge of lowering costs, it is useful to point out the largest gains come from the initial advances (e.g. moving from 100 to 200 micron limit). After that point, the benefits are diminishing.
7.4 Manufacturing Scale
The effects of manufacturing scale come into the cost calculation even if the annual number of packs produced is unchanged, but the design is altered (e.g. power is increased). For a fixed design, the effect of changing the scale of operations depends on the fraction of the total price that is made up of materials costs. Unit materials costs change little with scale whereas the costs per pack for labor, capital and plant area may decline substantially with increasing production rates, especially at low production rates, Fig. 7.5. 
The lines in the graphs are for the best-fit power relationships through the data with power factors of -0.076, -0.077, -0.147, and -0.211 from the top curve to that at the bottom. The least negative power factor is for the battery pack with the highest fraction of materials cost in the total pack cost. The more negative power factors result from a decreasing contribution of materials cost as a fraction of the total pack cost. These power factors for equations of the cost of a single unit can be converted to factors relating the total annual cost of manufacturing similar to Eq. 5.2 by adding 1.0 to each power factor. Thus the factors become 0.924, 0.923, 0.853, and 0.789. These large factors show only a small to moderate effect of scale. When the power curves are compared to the points in each of the graphs of Fig. 7.5, it is apparent that the scale factors approach one as the scale increases. This is because the model assigns a value of 0.95 for the active materials and 1.0 for the balance of the materials. As the production level increases and the materials costs become a larger fraction of the total price of the battery, the scaling power approaches 1.0 and the effect of scale become very small. Likewise, the effect of scale on battery price is much larger for HEV batteries than for EVs because materials costs constitute a smaller portion of the total cost for HEV batteries. Increasing the production rate for HEV batteries will result in a more dramatic reduction in cost than increasing the production rate for EV batteries.

Figure 7.4 Battery pack cost as a function of number of parallel cells and for different maximum electrode thicknesses. The electrode thicknesses (100 or 200 m) represent the limitation not the exact value calculated by the model. The cell capacity is also shown for the NMC441-Gr battery.


104
Figure 7.5 The effects of manufacturing rate on the price calculated by the model for battery packs of various cell chemistries, power capabilities and vehicle types. The EV and PHEV batteries are composed of 96 cells and the HEV-25 is composed of 48 cells.
y = 15609x-0.076
y = 13935x-0.077
6000
7000
8000
9000
10000
11000
12000
13000
14000
10 100 1000
Price to OEM ($)
Manufacturing rate (1000's /year)
EV150 NCA-Gr
EV150 LMO-Gr
y = 4931.1x-0.147
y = 2462.3x-0.211
500
1000
1500
2000
2500
3000
3500
10 100 1000
Price to OEM ($)
Manufacturing rate (1000's /year)
PHEV20 LMO-Gr
HEV-25 LMO-Gr



8. Statement of Copyright
BatPaC (Battery Performance and Cost Model) SOFTWARE
COPYRIGHT NOTIFICATION
© COPYRIGHT 2011 UCHICAGO ARGONNE, LLC All rights reserved. The BatPaC, version 2.0 and 1.0 software, manual and supporting documentation are protectable under copyright laws of the United States.

NEITHER THE UNITED STATES GOVERNMENT NOR ANY AGENCY THEREOF, NOR THE UCHICAGO ARGONNE, LLC, NOR ANY OF THEIR EMPLOYEES, MAKES ANY WARRANTY, EXPRESS OR IMPLIED, OR ASSUMES ANY LEGAL LIABILITY OR RESPONSIBILITY FOR THE ACCURACY, COMPLETENESS, OR USEFULNESS OF ANY INFORMATION, APPARATUS, PRODUCT, OR PROCESS DISCLOSED, OR REPRESENTS THAT ITS USE WOULD NOT INFRINGE PRIVATELY OWNED RIGHTS.



106
REFERENCES
1. M. Anderman, F. Kalhammer, and D. MacArthur. “Advanced Batteries for Electric Vehicles: An Assessment of Performance, Cost, and Availability.” California Air Resources Board, June (2000). Available from http://www.arb.ca.gov/msprog/zevprog/2000review/btapreport.doc (accessed on December 17, 2010).
2. B. Barnett, D. Ofer, C. McCoy, Y. Yang, T. Rhodes, B. Oh, M. Hastbacka, J. Rempel, and S. Sririramulu “PHEV Battery Cost Assessment,” 2009 DOE Merit Review, May (2009). Available from http://www1.eere.energy.gov/vehiclesandfuels/pdfs/merit_review_2009/energy_storage/ es_02_barnett.pdf (accessed on December 11, 2010).
3. B. Barnett, J. Rempel, D. Ofer, B. Oh, S. Sriramulu, J. Sinha, M. Hastbacka, and C. McCoy, “PHEV Battery Cost Assessment,” 2010 DOE Merit Review, June (2010). Available from http://www1.eere.energy.gov/vehiclesandfuels/pdfs/merit_review_2010/electrochemical_storage/es001_barnett_2010_o.pdf (accessed on December 11, 2010).
4. A. Dinger, R. Martin, X. Mosquet, M. Rabl, D. Rizoulis, M. Russo, and G. Sticher, “Batteries for Electric Vehicles: Challenges, Opportunities, and the Outlook to 2020.” The Boston Consulting Group, Available from http://www.bcg.com/documents/file36615.pdf (accessed on December 11, 2010).
5. L. Gaines and R. Cuenca, “Costs of Lithium-Ion Batteries for Vehicles,” Center for Transportation Research, Energy Systems Division, Argonne National Laboratory, ANL/ESD- 42, Argonne, IL May (2000).
6. F.R. Kalhammer, B.M. Kopf, D.H. Swan, V.P. Roan, M.P. Walsh, “Status and Prospects for Zero Emissions Vehicle Technology: Report of the ARB Independent Expert Panel 2007,” California Air Resources Board, April (2007). Available from http://www.arb.ca.gov/msprog/zevprog/zevreview/zev_panel_report.pdf (accessed on December 17, 2010).
7. M. A. Kromer and J. B. Heywood, “Electric Powertrains: Opportunities and Challenges in the U.S. Light-Duty Vehicle Fleet,” Sloan Automotive Laboratory, Laboratory for Energy and the Environment, Massachusetts Institute of Technology, LFEE 2007-03 RP, Cambridge, MA (2007).
8. P. Mock, “Assessment of Future Li-Ion Battery Production Costs,” presented at Plug-in 2009, Long Beach, CA, (2009).
9. National Research Council of the National Academies, “Transitions to Alternative Transportation Technologies – Plug-in Hybrid Electric Vehicles,” The National Academies Press, Washington, D.C. (2010). Available from http://www.nap.edu/catalog.php?record_id= 12826 (accessed on December 17, 2010).
10. TIAX LLC, “Cost Assessment for Plug-In Hybrid Vehicles (SOW-4656),” Report to US DOE Office of Transportation Technology, October (2007).

107
11. M. Anderman “The Plug-In Hybrid and Electric Vehicle Opportunity Report: A critical assessment of the emerging market and its key underlying technology: Li-Ion batteries,” Advanced Automotive Batteries, May (2010).
12. P.A. Nelson, D.J. Santini, J. Barnes, “Factors Determining the Manufacturing Costs of Lithium-Ion Batteries for PHEVs.” International Electric Vehicles Symposium EVS-24, Stavanger, Norway, (2009).
13. D.J. Santini, K.G. Gallagher, P.A. Nelson, “Modeling the Manufacturing Costs of Lithium Ion Batteries for HEVs, PHEVs, and EVs,” International Electric Vehicles Symposium EVS-25, Shenzhen, China, (2010).
14. K.G. Gallagher, P.A. Nelson, D.W. Dees, “PHEV battery cost assessment” 2011 DOE Merit Review Presentation Washington, DC May 9-12 (2011). Available from http://www1.eere.energy.gov/vehiclesandfuels/pdfs/merit_review_2011/electrochemical_storage/es111_gallagher_2011_o.pdf (Accessed on July 12, 2011).
15. P. Nelson, I. Bloom, K. Amine, G. Henriksen, “Design modeling of lithium-ion battery performance,” Journal of Power Sources, 110, 437 (2002).
16. P. Nelson, D. Dees, K. Amine, G. Henriksen, “Modeling thermal management of lithium-ion PNGV batteries,” Journal of Power Sources, 110, 349 (2002).
17. G.L. Henriksen, K. Amine, J. Liu, and P.A. Nelson, “Materials Cost Evaluation Report for High-Power Li-Ion HEV Batteries,” Electrochemical Technology Program, Chemical Technology Division, Argonne National Laboratory, ANL-03/05, Argonne, IL (2002). 
18. P. Nelson, K. Amine, A. Rousseau, H. Yomoto, “Advanced Lithium-Ion Batteries for Plug-in Hybrid-Electric Vehicles”, International Electric Vehicles Symposium, EVS-23, Anaheim, Ca(2007).
19. P. Nelson, “Modeling the Manufacturing Costs of Lithium-Ion Batteries for PHEVs,” presented at Plug-in 2009, Long Beach, CA, (2009).
20. K.G. Gallagher, P.A. Nelson, and D.W. Dees, “Simplified Calculation of the Area Specific Impedance for Battery Design,” Journal of Power Sources, 196 2289 (2011).
21. “Chevrolet Volt: Development Story of the Pioneering Electrified Vehicle” ed. Lindsay Brooke, SAE International, Warrendale, PA pgs 215 (2011). 
22. A.N. Jansen, K. Amine, and G. L. Henriksen, “Low-Cost Flexible Packaging for High-Power Li-Ion HEV Batteries,” Electrochemical Technology Program, Chemical Technology Division, Argonne National Laboratory, ANL-04/09, Argonne, IL (2004).

108
23. P.A Nelson and A.N. Jansen, “Comparative Costs of Flexible Package Cells and Rigid Cells for Lithium-Ion Hybrid Electric Vehicle Batteries,” Electrochemical Technology Program, Chemical Technology Division, Argonne National Laboratory, ANL-06/43, Argonne, IL (2006).
24. J. Euler and W. Nonnenmacher, “Stromverteilun in Porösen Elektroden,“ Electrochimica Acta, 2 268 (1960).
25. J.S. Newman and C.W. Tobias, “Theoretical Analysis of Current Distributions in Porous Electrodes,” Journal of the Electrochemical Society, 109 1183 (1962).
26. “Diagnostic Examination of Generation 2 Lithium-Ion Cells and Assessment of Performance Degradation Mechanisms,” Chemical Engineering Division, Argonne National Laboratory, ANL-05/21, Argonne, IL (2005).
27. D. Dees, E. Gunen, D. Abraham, A. Jansen, and J. Prakash, “Electrochemical Modeling of Lithium-Ion Positive Electrodes during Hybrid Pulse Power Characterization Tests” Journal of the Electrochemical Society, 155 (8) A603 (2008).
28. D. Dees, E. Gunen, D. Abraham, A. Jansen, and J. Prakash, “Alternating current impedance electrochemical modeling of lithium-ion positive electrodes,” Journal of the Electrochemical Society, 152 (7),A1409 (2005).
29. D. Abraham, S. Kawauchi, and D. Dees, “Modeling the impedance versus voltage characteristics of LiNi0.8Co0.15Al0.05O2,” Electrochimica Acta, 53 2121–2129 (2008).
30. D. P. Abraham, S. D. Poppen, A. N. Jansen, J. Liu, and D. W. Dees, “Application of a lithium-tin reference electrode to determine electrode contributions to impedance rise in high power lithium-ion cells,” Electrochimica Acta, 49 4763 (2004).
31. D. P. Abraham, E. M. Reynolds, E. Sammann, A. N. Jansen, and D. W. Dees, “Aging characteristics of high-power lithium-ion cells with LiNi0.8Co0.15Al0.05O2 and Li4/3Ti5/3O4 electrodes,” Electrochimica Acta, 51, 502 (2005).
32. D.P. Abraham, J. Liu, C.H. Chen, Y.E. Hyung, M. Stoll, N. Elsen, S. MacLaren, R. Twesten, R. Haasch, E. Sammann, I. Petrov, K. Amine, G. Henriksen, Journal of Power Sources, 119-121 511 (2003).
33. D. P. Abraham, R. D. Twesten, M. Balasubramanian, J. Kropf, D. Fischer, J. McBreen, I. Petrov, and K. Amine, “Microscopy and spectroscopy of lithium nickel oxide-based particles used in high power lithium-ion cells,” Journal of the Electrochemical Society, 150 (11) A1450 (2003).
34. A.M. Andersson, D.P. Abraham, R. Haasch, S. MacLaren, J. Liu, K. Amine, “Surface characterization of electrodes from high power lithium-ion batteries,” Journal of the Electrochemical Society, 149 A1358 (2002).


109
35. D. Abraham, J. Knuth, D. Dees, I. Bloom, and J. Christophersen, “Performance degradation of high-power lithium-ion cells - Electrochemistry of harvested electrodes,” Journal of Power Sources, 170 465 (2007).
36. J. Newman and K. E. Thomas-Alyea, “Electrochemical Systems,” 3rd ed., Wiley Interscience, New York (2004).
37. Wei Lai, Can K. Erdonmez, Thomas F. Marinis, Caroline K. Bjune, Nancy J. Dudney, Fan Xu, Ryan Wartena, and Yet-Ming Chiang, “Ultrahigh-Energy-Density Microbatteries Enabled by New Electrode Architecture and Micropackaging Design,” Advanced Materials, 22, E139–E144 (2010).
38. Pankaj Arora, Marc Doyle, and Ralph E. White, “Mathematical Modeling of the Lithium Deoposition Overcharge Reaction in Lithium-Ion Batteries Using Carbon-Based Negative Electrodes,” Journal of the Electrochemical Society, 146 (10) 3542-3553 (1999).
39. Y. Chen and J.W. Evans, “Thermal Analysis of Lithium-Ion Batteries” Journal of the Electrochemical Society, 143 (9) 2708-2712 (1996).
40. S.C. Chen, C.C. Wan, and Y.Y. Wan, “Thermal Analysis of lithium-ion batteries” Journal of Power Sources 140 111-124 (2005).
41. H. Maleki, S.A. Hallaj, J.R. Selman, R.B. Dinwiddie, and H. Wang, “Thermal Properties of Lithium-Ion Battery and Components” Journal of the Electrochemical Society, 146 (3) 947-954 (1999).
42. M. Sievers, U. Sievers, and S.S. Mao “Thermal modelling of new Li-ion cell design modifications” Forsch Ingenieurwes 74 215-231 (2010).
43. T.M. Bandhauer, S. Garimella, and T.F. Fuller “A Critical Review of Thermal Issues in Lithium-Ion Batteries” Journal of the Electrochemical Society, 158 (3) R1-R25 (2011).
44. R. Byron Bird, Warren E. Stewart, and Edwin N. Lightfoot, “Transport Phenomena,” 2nd Ed. John Wiley & Sons, Inc, New York, NY (2002).
45. R.K. Shah and A.L. London, “Laminar Flow Forced Convection in Ducts” Advances in Heat Transfer Supplement, Academies Press, New York, NY (1978).
46. R. Siegel, E.M. Sparrow, and T. M. Hallman, “Steady Laminar Flow Heat Transfer in a Circular Tube with Prescribed Wall Heat Flux,” Applied Scientific Research, Section A, 7 386- 392 (1958).
47. M. Nickolay and H. Martin, “Improved approximation for the Nusselt number for hydrodynamically developed laminar flow between parallel plates,” International Journal of Heat and Mass Transfer, 45 3263-3266 (2002).

110
48. United States Geological Survery, Commodity Statistics and Information, Available from http://minerals.usgs.gov/minerals/pubs/commodity/ (accessed on December 17, 2010). 49. R.H. Perry, D.W. Green, and J.O. Maloney, Perry’s Chemical Engineers’ Handbook, Sixth Edition, pp: 25-68 (1984).
50. M. Broussely, Ph. Biensan, F. Bonhomme, Ph. Blanchard, S. Herreyre, K. Nechev, and R.J. Staniewicz, “Main aging mechanisms in Li ion batteries,” Journal of Power Sources, 146 90-96 (2005).
51. Sun-Ho Kang, Wenquan Lu, Kevin G. Gallagher, Sang-Ho Park, and Vilas G. Pol, “Study of Li1+x(Mn4/9Co1/9Ni4/9)1-xO2 Cathode Materials for Vehicle Battery Applications” Journal of the Electrochemical Society, 158 (8) A936-A941 (2011).


111
Appendix A: BatPaC v1.0 Variation Study
Summary
The following ranges in Table A1 are suggested as an initial approximation to account for variation that will occur in the cost inputs and possible design limitations in BatPaC. The larger uncertainty for LMO in PHEV and EV batteries is due to an interaction with the electrode thickness limitation. Future versions of BatPaC will include error estimation within the model.
Table A1. Suggested confidence bounds as a percentage of the calculated point estimate for a graphite based Li-ion battery using the default inputs in BatPaC.
Discussion
The general approach in this variation study is to produce a distribution of cost inputs and analyze a range of battery designs to capture the spread in calculated battery price if the default cost inputs or design parameters are in error. The eight largest cost contributions comprising the battery price to the OEM, shown in Table A2, were evaluated to determine the range of possible values and the likely form of the distribution, normal or log-normal. For normal distributions, thestandard deviation was approximated as ¼ of the range of values. The parameters for log-normal distributions were hand-fit to set the minimum and maximum at the outer range of the 95 % confidence interval. Equations A1 and A2 were used to create the distribution for each cost input, Cij, from independent sets of 3000 normally distributed random numbers, rij. Here, Ci is the mean and σi is the standard deviation for the normal distribution of cost input i. Additionally, µi is the location parameter and αi is the scale parameter for the log-normal distribution. Each collection of cost inputs was used to produce an end battery price to the OEM. The battery designs used in this study are detailed in Table A3.
normal (A1)
log-normal (A2)
The variation in calculated price solely due to cost input estimates results in a near-normal distribution of values. The results may be adequately summarized by the calculated mean and standard deviation. Only the cases of the default design limitations are shown in Table A4 (100 micron limit, 1 cell in cell group). A value of +/- 10 % would adequately capture the 95% confidence interval of the calculated price distributions for all battery chemistries and battery types.
Battery type Cathodes lower upper
HEV LMO, LFP, NCA, NMC -10% 10%
PHEV, EV NMC, NCA -10% 20%
PHEV, EV LMO, LFP -20% 35%
Confidence Interval


112
Table A2. Cost input ranges and distributions used in variation study
Table A3. Battery designs considered in variation study
Table A4. Distribution in calculated price from cost input variation
Item low medium high distribution mean std dev location scale
Separator 0.75 2 4 log-normal 0.75 0.3
Copper foil 1 1.8 2.6 normal 1.8 0.4
Electrolyte 18 21.6 25.2 normal 21.6 1.8
Graphite anode 12 19 25 normal 19 3.25
LMO cathode 8 10 16 log-normal 2.35 0.15
NMC cathode 22 29 34 normal 29 3
NCA cathode 22 37 42 normal 37 5
LFP cathode 10 20 30 normal 20 5
SOC controller 1.5 2.5 3.5 normal 2.5 0.5
Coating capital 5 8 12 normal 8 1.75
Formation capital 20 30 50 log-normal 3.45 0.2
Battery type HEV-HP PHEV25 EV100
Power (kW) 40 65 115
Energy (kWh) 1.5 10.7 30
Range @ 300 Wh/mi 1 25 80
Number of cells 72 96 96
Number of modules 4 6 6
Cells in parallel group 1 1 1, 2
Electrode thickness limit (micron) 100 50, 100, 150 70, 100, 200
Cathode chemistries LMO, LFP LMO, NMC441, NCA LMO, NMC441, NCA
battery cathode mean std deviation 2/mean
HEV LMO 1268 49 0.08
HEV LFP 1475 65 0.09
PHEV25 LMO 2995 134 0.09
PHEV25 NMC441 3087 128 0.08
PHEV25 NCA 3325 153 0.09
EV100 LMO 6051 339 0.11
EV100 NMC441 5927 279 0.09
EV100 NCA 6648 364 0.11



113
Quantifying the error in calculated price due to the relative success or failure of certain design criteria is more difficult. We have chosen to vary the electrode thickness limitation for the PHEV and EV calculations. In addition, the EV battery was also calculated in a 2P-96S configuration (2 cells in parallel) to capture the possibility of smaller capacity cells while maintaining the 100 micron thickness limit. No design changes were analyzed for the HEVs. Treating each of the battery design occurrences as equally probable, the calculated population of each of the chemistries becomes a skewed distribution. Capturing the skewed and sometime bi-modal distribution in a simple statistical fashion is not straightforward. We suggest the use of a distribution parameter, ε, to establish the outer limits of a 95 % confidence interval from the point estimate, Po, created from the default values. This parameter is used in an empirical fashion in Equation A3 and A4. The factor of 1.05 is used to capture the increase in the mean of the population as compared to a spot estimate using the default inputs. The distribution parameters used in this study are twice the value of the standard deviation divided by the mean.
� � ( ) (A3)
� � ( ) (A4)
The NMC441 and NCA cathodes for PHEV and EV data sets may be captured using a distribution parameter of 0.15. The LMO cathode requires a distribution parameter of 0.28. The larger variation of the LMO cathode results from interaction with the limiting electrode thickness. A similar behavior is expected for LFP in energy batteries as this cathode also has a low volumetric capacity. The NMC441 and NCA cathodes have a significantly higher volumetric capacity and thus are less sensitive to this limitation. Figures A1-A3 present the variation of the PHEV and EV trials with the suggested confidence bounds highlighted by red lines and calculated point estimates from the default inputs are represented by the black line.


114
Figure A1. PHEV25 price distributions for NMC441 / Gr batteries. Red lines denote suggested upper and lower bounds for confidence interval. Black line represents price calculated from default values.
2600 2800 3000 3200 3400 3600 3800 4000 4200 4400
0
200
400
600
800
1000
1200
1400
1600
1800
2000
Count
Battery Price to OEM, US$
NMC441 / Gr
2600 2800 3000 3200 3400 3600 3800 4000 4200 4400
0
200
400
600
800
1000
Count
Battery Price to OEM, US$
150 micron limit
100 micron limit
50 micron limit


115
Figure A2. PHEV25 price distributions for LMO / Gr batteries. Red lines denote suggested upper and lower bounds for confidence interval. Black line represents price calculated from default values.
2500 3000 3500 4000 4500 5000
0
500
1000
1500
2000
2500
Count
Battery Price to the OEM, US$
LMO / Gr
2500 3000 3500 4000 4500 5000
0
200
400
600
800
1000
1200
Count
Battery Price to the OEM, US$
150 micron limit
100 micron limit
50 micron limit


Chemical Sciences and Engineering Division
Argonne National Laboratory
9700 South Cass Avenue, Bldg. 205
Argonne, IL 60439-4837
www.anl.gov



U.S. DEPARTMENT OF ENERGY
Argonne National Laboratory is a U.S. Department of Energy laboratory managed by UChicago Argonne, LLC
