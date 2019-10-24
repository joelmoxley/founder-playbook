Example of technoeconomic modeling for hydrogen production.

Credit: [Ahmad Mayyas, Mark Ruth, Bryan Pivovar, Guido Bender and Keith Wipke, NREL](https://sites.google.com/cyclotronroad.org/techonomics/model-downloads)

{! search-content: !}
Manufacturing Cost Analysis for Proton
Exchange Membrane Water
Electrolyzers
Ahmad Mayyas, Mark Ruth, Bryan Pivovar, Guido Bender,
and Keith Wipke
National Renewable Energy Laboratory
NREL is a national laboratory of the U.S. Department of Energy
Office of Energy Efficiency & Renewable Energy
Operated by the Alliance for Sustainable Energy, LLC
This report is available at no cost from the National Renewable Energy
Laboratory (NREL) at www.nrel.gov/publications.
Contract No. DE-AC36-08GO28308
National Renewable Energy Laboratory
15013 Denver West Parkway
Golden, CO 80401
303-275-3000 • www.nrel.gov
Technical Report
NREL/TP-6A20-72740
August 2019
Manufacturing Cost Analysis for Proton
Exchange Membrane Water
Electrolyzers
Ahmad Mayyas, Mark Ruth, Bryan Pivovar, Guido Bender,
and Keith Wipke
National Renewable Energy Laboratory
Suggested Citation (Arial 12 pt Bold)
Mayyas, Ahmad, Mark Ruth, Bryan Pivovar, Guido Bender, and Keith Wipke. 2018.
Manufacturing Cost Analysis for Proton Exchange Membrane Water Electrolyzers.
Golden, CO: National Renewable Energy Laboratory. NREL/TP-6A20-72740.
https://www.nrel.gov/docs/fy10osti/72740.pdf.
NOTICE
This work was authored by the National Renewable Energy Laboratory, operated by Alliance for Sustainable
Energy, LLC, for the U.S. Department of Energy (DOE) under Contract No. DE-AC36-08GO28308. Funding
provided by the Laboratory Directed Research and Development (LDRD) Program at NREL. The views expressed
herein do not necessarily represent the views of the DOE or the U.S. Government.
This report is available at no cost from the National Renewable
Energy Laboratory (NREL) at www.nrel.gov/publications.
U.S. Department of Energy (DOE) reports produced after 1991
and a growing number of pre-1991 documents are available
free via www.OSTI.gov.
Cover Photos by Dennis Schroeder: (clockwise, left to right) NREL 51934, NREL 45897, NREL 42160, NREL 45891, NREL 48097,
NREL 46526.
NREL prints on paper that contains recycled content.
ii
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
Acknowledgment
This work was supported by the Laboratory Directed Research and Development (LDRD) Program at
the National Renewable Energy Laboratory (LDRD 10012-17.02.01 H2 @scale)
iii
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
Executive Summary
Hydrogen is produced by several means, including water electrolysis, in which water molecules are split
into hydrogen and oxygen molecules. Low cost high-capacity electrolysis system is a key technology
that can support greater deployment of zero-carbon hydrogen for a variety of applications and represents
a technology that can potentially facilitate integration of greater renewable electricity sources. While
there are several commercial electrolysis systems, proton exchange membrane (PEM) technology has
emerged as a development opportunity because of its versatility. High differential operating pressure,
variable operating condition potential, high current densities, high power densities, and high efficiencies
are among the advantages of the PEM electrolyzer over other commercial or near-commercial
electrolysis technologies. In this report, we discuss bottom-up manufacturing cost analysis for the PEM
electrolyzers across various power ratings at several annual production rates. We also study the impact
of manufacturing economies of scale on the cost of the PEM electrolyzer and how this can be linked to
reducing the cost of hydrogen production.
Bottom up costing models were developed for the kay parts in the stack. Cost model results show that
direct material costs dominate stack costs at high production volume (Figure ES-1). Stack cost for 1-
MW system can be reduced from $237/kW (±10%) at annual production rate of 10 MW/yr (e.g., 1-MW
systems at a production rate of 10 unit/year) to about $101 (±10%) at annual production rate of 1,000
MW (e.g., 1-MW systems at a production rate of 1,000 unit/year). We expect smaller cost reductions in
the “balance of plant” cost because most parts are outsourced from suppliers that are manufacturing the
components for multiple markets and thus are at high volume already. Depending on the production
volume, we found that CCM shares about 26%–47% for 200-kW PEM stack and about 36%–47% for
the 1-MW stack, with PTL contributing around 17%–25% of the stack cost, bipolar plates about 12%–
21%, and end plates and assembly near 3%–13%. Parametric sensitivity analysis shows that the final
stack cost is sensitive to manufacturing process yields, power density of the cell, gold layer thickness on
porous transport layer and bipolar plates and Pt loading in the catalyst coated membrane. Balance-ofplant cost for a 1-MW electrolyzer contribute to about two-thirds of the system cost, with power
electronics contributing half the BOP cost, while the water circulation and hydrogen processing
subsystems each share about one-fifth of the BOP cost.
We also analyzed several scenarios to study the effect of changing certain cell design parameters and
manufacturing process on the stack and system cost for PEM electrolyzers. These proposed scenarios
represent cases for the future PEM system design and the potential cost reductions when more advanced
manufacturing processes are introduced and adopted in PEM electrolyzer production (Figure ES-2).
Some scenarios we ran here include adoption of the high-throughput, automated manufacturing
processes that have high process yields, such as roll-to-roll manufacturing of catalyst-coated membrane
and advanced coating processes for metal plates which could reduce the cost for the PEM electrolyzer
stack from $237/kW (±10%) at a production volume of 10 MW (e.g., 1-MW systems at a production
rate of 10 units/year) to $69/kW (±10%) at 1,000 MW (e.g., 1-MW systems at 1,000 unit/year). System
cost of 1-MW electrolyzer, including stack and balance of plant, could also be reduced through
manufacturing economies of scale – from $561/kW (±10%) at 10 units/year to $265/kW (±10%) at
1,000 units/year. The base year for the analysis is 2015, so all cost numbers presented in this report are
expressed in 2015 dollars.
In terms of the effect of the electrolysis system capital cost on hydrogen production cost, we found that
electricity price in addition to the electrolyzer capital cost play key role in determining the cost of
iv
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
hydrogen production via water electrolysis. Thus, any cost reduction in the electrolyzer cost will help
reduce the cost of hydrogen production process.
Figure ES-1. 1-MW PEM electrolyzer system cost at different annual production rates
(The annual production rate is the number of electrolyzer systems produced in one year)
Figure ES-2. Waterfall charts showing areas where R&D can play a role in reducing the cost of the 1-MW
electrolysis system
Assumptions: improvement in power density (+20%); Pt loading from 11 g/m2 to 1 g/m2, membrane cost (Nafion 117 vs.
Solvay E98-09S), and power electronics (-20%). Economy of scale is the manufacturing cost of 10 units/yr vs. 100 units/yr vs.
1,000 units/yr.
v
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
Table of Contents
1 Introduction ...........................................................................................................................................1
2 Electrolyzer Functional Specifications and System Design.............................................................4
3 Costing Approach and Considerations ..............................................................................................6
3.1 Modeling Approach .......................................................................................................................6
3.2 Parameters of the Manufacturing Cost Model...............................................................................8
4 Manufacturing Cost Model for PEM Electrolyzer.............................................................................10
4.1 Catalyst-Coated Membrane .........................................................................................................10
4.2 Porous Transport Layer ...............................................................................................................11
4.3 Membrane Electrode Assembly (MEA) and Frame/Seal ............................................................12
4.4 Bipolar and End Plates.................................................................................................................13
4.5 Stack Assembly............................................................................................................................13
5 Results and Discussion......................................................................................................................16
5.1 Cost of the Stack Parts.................................................................................................................16
5.2 Balance-of-Plant Cost..................................................................................................................24
5.3 PEM Electrolyzer System Cost....................................................................................................28
6 Sensitivity Analysis and Potential Cost Reductions.......................................................................32
7 Installed System Cost.........................................................................................................................36
8 Effect of Electrolyzer Capital Cost on the Hydrogen Production Cost .........................................38
9 Conclusions.........................................................................................................................................39
References .................................................................................................................................................40
vi
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
List of Figures
Figure 1. Cell repeat unit showing key components in the PEM electrolyzer – additional units would be stacked to
the right and left of this repeating unit to form a PEM electrolysis stack ................................2
Figure 2. Schematic of the PEM electrolysis system showing stack and BOP parts ....................................5
Figure 3. Process flow for catalyst deposition using spray coating.............................................................11
Figure 4. Process flow of the powder metallurgy process for producing titanium felts used as in the PTL12
Figure 5. Process flow for producing metal bipolar plates..........................................................................13
Figure 6. Process flow for semi-automatic assembly line ...........................................................................15
Figure 7. Manufacturing cost curves for CCM made via spray coating......................................................18
Figure 8. Manufacturing cost curves for the titanium-based PTL...............................................................19
Figure 9. Cost of carbon cloth vs. Ti-based PTL.........................................................................................20
Figure 10. Manufacturing cost curves for the frame ...................................................................................21
Figure 11. Manufacturing cost curves for the stamped stainless-steel plates bipolar plates.......................22
Figure 12. Manufacturing cost analysis for stack assembly process...........................................................23
Figure 13. Cost breakdown for the BOP parts.............................................................................................26
Figure 14. Manufacturing cost curve for (a) 200-kW PEM electrolyzer stack, (b) manufacturing cost curve for 1-
MW PEM electrolyzer stack, (c) cost breakdown for 200-kW stack, and (d) cost breakdown for 1-
MW stack................................................................................................................................29
Figure 15. Cost curves for (a) 200-kW and (b) 1-MW electrolyzer systems showing costs of stack and BOP, and
cost breakdown for (c) 200-kW and (d) 1-MW electrolyzer systems at different annual production
rates.........................................................................................................................................31
Figure 16. Impact of changing some manufacturing and cell design parameters on 200-kW PEM stack cost: (a) at
100 units/yr, and (b) at 1,000 units/yr, and 1-MW stack cost at (c) at 100 units/yr, and (d) at 1,000
units/yr....................................................................................................................................34
Figure 17. Waterfall charts showing areas where R&D can play a role in reducing the cost of the electrolysis
system for (a) 200 kW system and (b) 1-MW system............................................................35
Figure 18. Installed system cost ..................................................................................................................37
Figure 19. Effect of the capital cost, capacity factor, and electricity price on the cost of hydrogen production
(excluding compression, storage and dispensing CSD cost)..................................................38
Figure A1. Functional cell dimensions........................................................................................................43
Figure A2. Example of the polarization curves for PEM electrolyzer cells................................................44
vii
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
List of Tables
Table 1. Functional Specifications of the PEM Electrolysis System (Appendix A reports details)..............4
Table 2. Scope of the Manufacturing Cost Models.......................................................................................7
Table 3. Manufacturing Cost Shared Parameters..........................................................................................8
Table 4. Some Parameters Used in Developing the Cost Model for PEM Electrolyzer Stack....................10
Table 5. Cost of the Balance-of-Plant Parts ................................................................................................27
Table B.1. Cost Components and Their Mathematical Formulas ...............................................................50
Table C.1. Manufacturing parameter for spray coating process of the catalyst coated membrane .............52
Table C.2. Manufacturing parameter for Powder metallurgy of the Porous Transport Layer.....................53
Table C.3. Manufacturing parameter for injection molding of the Seal/Frame ..........................................54
Table C.4. Manufacturing parameter for stamped and coated bipolar plates..............................................55
Table C.5. Manufacturing parameter for stack assembly process...............................................................56
1
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
1 Introduction
Although hydrogen is abundant on the Earth in the form of water, it requires energy to split water
molecules into hydrogen molecules. Hydrogen can be made by several means, including water
electrolysis, hydrocarbon reforming/gasification, renewable liquid hydrocarbon reforming, and
fermentation of the biomass feedstocks (AFDC n.d.).
Most of today’s anthropogenic hydrogen, both internationally and in the U.S., is produced by
steam methane reforming of natural gas (AFDC n.d.). The steam methane reforming process
consists of two process steps. In the first step, the major component of natural gas, methane
(CH4), reacts with steam to form hydrogen and carbon monoxide. In the second step, water gas
shift, carbon monoxide is reacted with steam to produce additional hydrogen and carbon dioxide
(Air Products 2013). Pressure swing adsorption (PSA) technology is needed for hydrogen
purification in the steam-methane reforming (SMR) process, to get high purity hydrogen suitable
for fueling fuel cell electric vehicles (FCEVs). The PSA process involves the adsorption of
impurities from a hydrogen rich feed gas onto a fixed bed of adsorbents at high pressure. The
impurities are subsequently desorbed at low pressure into off-gas stream which results in
production of an extremely pure hydrogen product (99.999%) (Howe-Baker, 2017). Steam
methane reforming systems have high production rates, and need large investment to install,
which makes them suitable for central production facilities that produce tons of hydrogen every
day.
Water electrolysis is the second most common method of hydrogen production. Among the
challenges that face water electrolysis is the high system cost for electrolysis systems which
resulted in low penetrations of PEM electrolysis technology in the markets. Three major types of
electrolyzers are either currently produced commercially or could be produced commercially in
the near future:
• Alkaline electrolyzers are a demonstrated water electrolysis technology at large scale, but
they tend to have lower system efficiency.
• Polymer electrolyte membrane (PEM) electrolyzers work at temperatures between 50°C
and 95°C. PEM electrolysis is a commercial technology that could still be improved through
additional R&D.
• Solid oxide electrolyzers are still in early commercialization stage and still need more work
to scale up into commercial systems.
Alkaline electrolysis is considered a mature technology and has been marketed for decades. PEM
electrolysis technology, on the other hand, has positioned itself as a competitive technology, but
PEM systems are still designed at lower capacities (<1 MW) and have higher costs than alkaline
electrolyzers (Schmidt et al., 2017a, Bertuccioli et al., 2014). In the U.S., Proton (NEL) and Giner
and others have started to produce PEM electrolyzers because (1) manufacturing costs have
decreased significantly in the last few years and (2) PEM electrolyzers tend to have higher current
densities (~5X of the alkaline electrolyzers) and higher efficiencies (up to 6% higher than alkaline
electrolyzers (see Bertuccioli et al., 2014; Hamdan 2013; Ayers et al. 2012, Carmo et al., 2015).
A PEM electrolyzer stack consists of repeating cells that are electrically connected in series and
reactant water/product gas connected in parallel (Figure 1). Thick metal plates (called end plates)
2
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
from both ends are added to structurally hold these cells inside the stack. At the core of each of
these modules is a polymer membrane with cathode and anode catalyst layers coated on the both
sides of the membrane to form what is called catalyst-coated membrane (CCM). The porous
transport layer (PTL) is a layer that enhances water diffusion and water splitting reaction on the
surface of the membrane in the electrolysis cells. Bipolar plates, as the name suggests, have a
cathodic side and an anodic side. Their main function is to separate cells in the stack, and they
have channels that facilitate the transport of water, hydrogen, and oxygen inside the stack
(Hamdan 2013; Ayers et al. 2012).
Figure 1. Cell repeat unit showing key components in the PEM electrolyzer – additional units
would be stacked to the right and left of this repeating unit to form a PEM electrolysis stack
PEM electrolyzer stacks have many similar parts as PEM fuel cell stacks and—include the CCM,
a gas diffusion layer, and bipolar plates. Many technoeconomic studies have revealed that
significant cost reductions are possible for manufacturing these parts for fuel cells and
electrolyzers with economies of scale (Contini et al. 2017; James et al. 2013; James and DeSantis
2015; Wei et al. 2014).
This document reports a detailed cost analysis of PEM electrolysis systems and identifies some
potential areas where cost reductions could be targeted. The results of this work could help direct
future research and development (R&D) for the PEM electrolysis manufacturing. More
specifically, the objectives of this work include to:
• Develop detailed bottom-up manufacturing cost analysis for key systems and parts in the
PEM water electrolysis system
• Identify cost drivers for the PEM electrolyzer and areas for potential cost reduction areas
• Investigate effect of economies of scale and learning experience on the cost of the PEM
electrolysis systems and the impact of the system cost on hydrogen production cost.
This report starts with a summary of some findings from previous technoeconomic studies
on electrolyzers and fuel cells, which we used to estimate the parameters for the cell design and
functional specifications for the water electrolysis system (Section 2). The report then proceeds
in Section 3 to a discussion of the methods used to develop the manufacturing cost of PEM
electrolyzers. Sections 4 and 5 discuss manufacturing processes used to make the key parts in the
PEM stack and the expected cost associated with the manufacturing of these parts in the stack
3
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
and the cost of the balance-of-plant (BOP) parts. Section 6 provides some sensitivity analysis for
some important cell design and manufacturing parameters that could play role in reducing the
cost of the PEM stack. Section 7 expands on Section 5 by reporting total system cost estimates
including markup factor and installation cost. Section 8 addresses the impacts of the economies
of scale electrolyzer costs and translates those capital costs to levelized costs hydrogen.
4
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
2 Electrolyzer Functional Specifications and
System Design
We started this cost analysis study by defining the system diagram and determining the critical
cost components. Next, we used data from the literature, industry inputs, and product fact sheets
for commercial PEM electrolysis systems to obtain functional and operational parameters at the
stack and system levels. These functional and design parameters are often referred to as
functional specifications. We then developed a bottom-up cost analysis for each of the critical
stack cost components (i.e., CCM, PTL, membrane electrode assembly [MEA] frame/seal,
bipolar plate, and stack assembly). Finally, we sum the individual cost curves for each stack part
to calculate the overall stack cost in $/kW.
Functional specifications for 200-kW and 1-MW electrolysis systems are shown in Table 1. A
schematic of the PEM electrolysis system is shown in Figure 2. The stack represents the core
of the system where electrochemical reactions take place. The “balance of plant” (BOP) is
composed of several subsystems that provide secondary functions in the electrolyzer system. The
major subsystems in the BOP and key parts in each system include:
• Power supply: AC/DC rectifier, DC voltage transducer, and DC current transducer
• Deionized water circulation system: oxygen separator tank, circulation pump, piping, valves
and instrumentation, and controls
• Hydrogen processing: dryer bed, hydrogen separator, tubing, and valves and instrumentation
• Cooling: plate heat exchanger, cooling pump, valves and instrumentation, and dry cooler
• Miscellaneous: compressed air valve, ventilation and safety requirements (combustible gas
detector and exhaust ventilation).
Table 1. Functional Specifications of the PEM Electrolysis System (Appendix A reports details)
Parameter Value Unit
Stack power 200 1,000 kW
Gross system power 220 1,100 kW
Average hydrogen (H2) production rate 30 170 Nm3/hr
Average H2 production rate 80 400 kg/day
Turndown ratio 0%–100% 0%–100%
Operating Pressure 0- 30 bar
Total plate area 957 cm2
CCM coated area 748 cm2
Single cell active area 680 cm2
Gross cell inactive area 9 %
Single cell amps 1,156 A
Current density 1.70 A/cm2
Reference voltage 1.70 V
Power density 2.89 W/cm2
5
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
Parameter Value Unit
Platinum (Pt) loading- anode (g/m2) 7.0 g/m2
Platinum-iridium loading- cathode (g/m2) 4.0 g/m2
Single cell power 1,965 W
Cells per system 102 510 cells
Stacks per system 1 2 stacks
Cells per stack 102 255 cells
Water pump 5 25 kW
Other paras. Loads 15 75 kW
Parasitic loss 20 100 kW
Values in italic are parasitic losses in the balance of plant (BOP) and represent average values from several sources.
Figure 2. Schematic of the PEM electrolysis system showing stack and BOP parts
6
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
3 Costing Approach and Considerations
This section describes the overall costing approach and the underlying assumptions used in
developing cost models. Several cost components are included in the direct manufacturing cost
model to account for all cost incurred in the final products. These cost components include
material, labor, capital, energy, maintenance, facility/building, and scrap costs. These
components represent direct manufacturing cost, excluding research and development cost, sales,
general and administration cost, warranty cost or debt service cost. However, all these indirect
cost components are combined in the markup factor, which was assumed to be 50% of the total
direct manufacturing cost (James and DeSantis 2015; Saggiorato et al. 2017).
Bottom up manufacturing cost models were developed for several parts in the stack:
• Catalyst coated membrane (CCM)
• Porous transport layer (PTL)
• Seal/Frame
• Bipolar plates
• Stack assembly and end plates
Cost values for BOP parts were collected from quotes we received from part suppliers for the
critical parts in the BOP and estimates in the literature for general purpose parts such as piping,
pressure gauges, valves, water pumps, and other parts. Assembly and testing are the main
manufacturing processes that take place in assembling BOP parts within the system. The direct
cost of BOP parts and their assembly and testing costs are then added to the direct manufacturing
cost using bottom-up approach for the stack modules to estimate the final electrolyzer system
cost.
A make-or-buy decision is based on whether the part is readily available as a commodity item, if
it is an off-the-shelf part, or if it is a special manufactured part that necessitates certain design
and manufacturing routes, or if the parts are associated with proprietary manufacturing processes
(e.g., Nafion membrane1
). If the product falls outside the scope of the regular business that
electrolyzer manufacturers do (e.g., manufacture pumps, valves, tubes, and electronic
components), the decision was made to outsource these parts from suppliers and include the
price in the BOP cost analysis. In this analysis, BOP components are all assumed to be
outsourced from part vendors, while key stack parts are assumed to be largely manufactured inhouse.
3.1 Modeling Approach
This section describes the direct manufacturing cost modeling approach developed for the PEM
electrolyzer stack components and the cost analysis of the balance of plant (BOP). The first step
in the bottom-up costing analysis is to define the electrolyzer system configuration and key
1 Nafion is a registered trademark of DuPont.
7
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
subsystems in it. Next, literature reviews and industry inputs are used to obtain functional and
operational stack and system parameters (also known as functional specifications). The system
configuration and functional specifications are then used to define the system size, key
subsystems and system components, and stack and system performance specifications. Then, we
use these specifications and system functional parameters to develop the direct manufacturing
cost model (Wei et al., 2014).
The direct manufacturing cost analysis uses activity-based costing for the major manufacturing
processes required to make the key components in the PEM stack. A machine rate that
corresponds to annual production rates is computed and broken down by cost components that
cover capital, facilities, energy, and maintenance costs. To obtain the process cost per
module/part, one can multiply machine rates expressed in dollars per hours ($/hr) by the total
time required to finish each part or batch of parts. Normalized manufacturing cost per part
($/piece) is calculated by dividing machine rate ($/hr) over line throughput (piece/hr). Labor and
material costs are added to the normalized part cost ($/piece) to calculate the final part cost in
($/piece). Overall manufacturing costs are then calculated as the sum of all modules or cost
components normalized to the annual production rates in units per year2
.
Several cost components are included in the direct manufacturing cost model to account for all
cost incurred in the final products. These cost components include material, labor, capital,
energy, maintenance, facility, and scrap costs. And, these components represent direct
manufacturing cost, excluding any research and development cost, sales, general and
administration cost, warranty cost or debt service cost. However, all these indirect cost
components are combined in the markup factor (Saggiorato et al. 2017). Table 2 summarizes
direct and indirect manufacturing cost components.
Table 2. Scope of the Manufacturing Cost Models
Direct Manufacturing Cost Indirect Manufacturing Cost
Capital costs Research and development costs
Facilities/building costs General and administration costs
Materials costs Sales and marketing costs
Scrap costs (yield losses) Product warranty costs
Labor costs Debt service costs
Energy costs Transportation costs
Maintenance costs
Appendix B contains detailed economic calculations and the mathematical formulas used in the
bottom-up manufacturing cost analysis (both direct and indirect manufacturing cost models).
The electrolysis system is made up of the stack and other subsystems needed to ensure full
functionality of the electrolysis process from water supply at one end to hydrogen storage at the
other end of the system. These subsystems are bundled in the BOP. Cost values for BOP parts
were collected from the direct quotes we received from part suppliers and estimates in the
2 Units here refer to number of electrolyzers produced per annum
8
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
literature for general purpose parts such as piping, pressure gauges, valves, water pumps, and
other parts. The direct cost of BOP parts and their assembly and testing costs are then added to
the direct manufacturing cost for the stack parts to estimate the final electrolyzer system cost.
3.2 Parameters of the Manufacturing Cost Model
To facilitate a better understanding of cost drivers and their role in determining final product
cost, we collected data from multiple sources, including previous studies, patents, technical
reports, and data sheets for commercial electrolyzer systems. We then used the collected data to
develop assumptions for different manufacturing process studies in this analysis. Key parameters
used in developing the cost model are summarized in Table 3. Worth mentioning that the base
year for the cost analysis is 2015, so all cost values are expressed in 2015 dollars. Economic
calculations are discussed in Appendix B.
Table 3. Manufacturing Cost Shared Parameters for U.S. based manufacturing facility
Parameter Symbol Value Units Notes/Sources
Operating hours 𝑡𝑡ℎ𝑠𝑠 vary hours 8-hour base shift, 2 shifts per day
Annual operating days 𝑡𝑡𝑑𝑑𝑑𝑑 250 days 52 weeks/yr, 5 working days per week,
10 holidays/yr
Average inflation rate 𝑗𝑗 2.6% World Bank dataa
Discount rate 𝑗𝑗𝑑𝑑 10% From James et al., (2015)
Corporate income tax 𝑖𝑖𝑖𝑖 40% Tax Foundationb; for profitable income only
Property tax 𝑖𝑖𝑝𝑝 1.4% New York Timesc
End-of-life salvage value 𝑘𝑘𝑒𝑒𝑒𝑒𝑒𝑒 2% assume 2% of the original equipment value
Tool lifetime 𝑇𝑇𝑡𝑡 15 years typical value in practice
Energy tax credits 𝐼𝐼𝐼𝐼𝐼𝐼 0 dollars
Energy cost 𝑐𝑐𝑒𝑒 0.1 $/kWhe
Floor space Cost 𝑐𝑐𝑓𝑓𝑓𝑓 880 $/m2 average for factoryd
Building depreciation 𝑗𝑗𝑏𝑏𝑏𝑏 0.031 U.S. Bureau of Economic Analysis ratese
Building recovery 𝑇𝑇𝑏𝑏𝑏𝑏 31 years U.S. Bureau of Economic Analysis ratese
Building footprint 𝑎𝑎𝑏𝑏𝑏𝑏 varies m2
Hourly labor cost 𝑐𝑐𝑙𝑙𝑙𝑙𝑙𝑙𝑙𝑙𝑙𝑙 23.63 $/hr hourly wage per worker
a “Inflation, GDP Deflator (Annual %)” The World Bank., https://data.worldbank.org/indicator/ny.gdp.defl.kd.zg
b Pomerleau 2014
c “State-by-State Property-Tax Rates,” New York Times, April 10, 2007, https://www.nytimes.com/2007/04/10/business/11leonhardtavgproptaxrates.html,
d See for example, Turner and Townsend n.d. (http://www.turnerandtownsend.com/ICC_Survey_Brochure_final_6MGJa.pdf.file)
and CBRE n.d. (http://www.cbre.us/services/projectmanagement/AssetLibrary/EMEA%20Fit_Out_Cost_Guide_2014.pdf)
e BEA n.d.
9
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
The annualized cost in $/yr (excluding variable cost components: materials and labor) was
adopted from the economic model developed by Haberl (1993):
Cy = Cc + Cr + Coc + Cp + Cbr + Ci + Cm − Cs − Cint − Cdep (9)
where:
Cy is the total annualized cost.
Cc is the annualized capital/system cost (with interest).
Cr is the replacements or disposal cost.
Coc is the operating cost (e.g., electricity), excluding labor.
Cp is the property tax cost.
Cbr is the building or floor space cost.
Ci is the tool insurance cost.
Cm is the maintenance cost.
Cs is the end-of-life salvage value.
Cint is the deduction from income tax.
Cdep is the deduction due to tool depreciation.
In addition to the annualized overhead cost components shown above, we also added the
following cost components to get the complete direct manufacturing cost:
• Labor cost is estimated using hourly paid workers to make a certain number of units per year.
• Materials cost (including scrap cost) is based on the materials required to make certain
products (e.g., costs of stainless-steel sheets and coating materials used in bipolar plates).
All values are adjusted to 2015 dollars. In the current version of the model, Cr (the replacement
or disposal cost) and Ci (the tool insurance cost) are assumed to be zero. In this analysis, we
assumed the manufacturing facility would be constructed solely to manufacture a certain type
of products (e.g., coating of the catalyst layers in the CCM and production of PTL). We also
assumed investors would start from scratch (i.e., they would build the facility and acquire
new equipment to run the facility and would then hire people to work in the plant). This
latter assumption led to another assumption where we assumed no net income for the new
manufacturing facility; thus, income tax credits such as interest tax credits do not factor into
the final cost calculations.
10
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
4 Manufacturing Cost Model for PEM Electrolyzer
Manufacturing cost models were developed for the key parts in the stack, including the CCM,
PTL, bipolar plate, seal and frame, and end plates with the required assembly process to
assemble these components into the stack. Table 4 summarizes the main manufacturing
processes along with some key parameters used in developing cost models for these stack parts.
Other important manufacturing process parameters for all manufacturing routes investigated in
this study are shown in Appendix C.
Table 4. Some Parameters Used in Developing the Cost Model for PEM Electrolyzer Stack
Part Assumptions Notes
Membrane Nafion 117 (purchased part) Alternatives include PFSA (PEEK, PBI)
membranesa
Pt Pt-price = 1,500/tr.ozb U.S. Department of Energy (DOE)
current value
CCM Platinum loadings:
Anode: 7 g/m2 (Pt)
Cathode: 4 g/m2 (Pt-Ir)
Spray coating (alternative processes
include slot-die coating and screen
printing)
PTL Sintered porous titanium (anode side)
Caron paper (cathode side)
Titanium powder price = $35/kg
Ti-PTL Porosity=30%; Ti-PTL coated with
gold (100 nm)
Carbon cloth: Toray Paper 090 - TGP-H090 (thickness = 280 μm)
Frame PPS-40GF or PEEK thermoplastics 0.625 cm from each side of the CCM was
used for MEA frame bonding (injection
molding)
Total frame width = 2.445 cm
Plates Stamped stainless steel 316L sheets
Thickness=5 mm
Coated with gold (100 nm)
a PFSA = perfluorosulfonic acid, PEEK = polyetheretherketone, PBI = polybenzimidazole, PPS-40GF: polyphenylene
sulfide with 40% glass fiber filler
b tr.oz: troy ounce = 31.103477 grams
4.1 Catalyst-Coated Membrane
The catalyst-coated membrane (CCM) is made by depositing catalyst layers (platinum group
metals) on each side of the Nafion membrane to form the cathode and anode layers. The anode
side of the selective polymer membrane is where splitting of the water molecules takes place
to make oxygen molecules, protons, and electrons. After this happens, the protons pass through
the membrane and combine with electrons delivered through an external circuit to produce
hydrogen molecules. Nafion is a perfluorosulfonic acid-based (PFSA) polymer. PFSA polymers
have characteristics (e.g., high conductivity, high chemical stability) that make it the preferred
membrane technology for use in PEM stacks.
Current catalyst deposition methods include spray coating and screen printing. Emerging coating
technologies such as the slot-die and doctor blade coatings (forms of roll-to-roll manufacturing
processes) can increase the speed of coating process and improve the quality of the coated CCM
11
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
parts. In this cost analysis, we used spray coating as the base of the analysis. Figure 3 shows a
schematic of the spray coating process with the quality control unit that uses optical and/or
infrared scanning systems. This process starts by unrolling the Nafion membrane sheet. Then the
Nafion membrane is coated using precise spraying nozzles to deposit platinum group metal on
the surface of the membrane, e.g., the anode side first. After that, the wet membrane is dried and
cooled down, then it undergoes into a second coating process where the other side of the
membrane is coated (cathode side) to obtain the dried catalyst coated membrane (CCM). The
final CCM is then cut into smaller individual pieces to be used in the MEAs.
Figure 3. Process flow for catalyst deposition using spray coating
QC = quality control
4.2 Porous Transport Layer
The corrosive environment inside the PEM stack may limit the type of materials that can be used
in the PTL, which is also called the gas diffusion layer in the literature. The PTL should possess
certain characteristics (e.g., good corrosion resistance) and certain porosity to facilitate the
transport and diffusion of the gases and fluids inside the MEA.
12
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
The PTL can be made from sintered titanium via powder metallurgy or from carbon cloth with
a certain thickness.3 In this study, we assumed anode PTL is made from titanium powder via the
powder metallurgy process, while the cathode PTL is made from carbon cloth. The process flow
for manufacturing of titanium-felts used in the PTL is shown in Figure 4. This process starts by
mixing titanium powder with small amounts of adhesive powder and lubricants to facilitate
compaction of the brittle titanium particles. The “green” compacts coming from the compaction
process are then placed in the sintering furnace, where sintering (partial melting process) takes
place under controlled conditions (e.g., temperature, oxygen level, and cooling time). Parts
coming out of the furnace need minor cleaning or machining to get the final titanium felts, which
are sent to the coating station where they are coated with a precious material (gold or platinum)
to reduce the contact resistance and reduce oxidation (Lettenmeier et al., 2017). The powder
metallurgy process is versatile process that offers several advantages such as the ability to
compact several parts in one shot and the ability to adjust the compaction pressure to get the
desired porosity in the PTL; in this analysis, porosity was assumed to be 30% by volume.
Manufacturing process parameters for powder metallurgy and coating processes are summarized
in Appendix C.
Figure 4. Process flow of the powder metallurgy process for producing titanium felts used as
in the PTL
4.3 Membrane Electrode Assembly (MEA) and Frame/Seal
CCM and PTL together represent the MEA. Parts in the MEA are held together by the frame,
which is made from polyphenylene sulfide (PPS) resin mixed with 40% glass fiber. The width of
the frame is 4.9 cm from each side of the MEA. The PPS-based frame provides the flexibility
required to hold the MEA and the durability to withstand the high operating temperature (50°C –
120°C) and the corrosive environment inside the stack. Injection molding was assumed to be the
base process in this analysis. Manufacturing process parameters for an injection molding
production line are summarized in Appendix C.
3 A common carbon cloth used in PEM electrolyzers and fuel cells is Toray Paper 090 - TGP-H-090
(thickness = 280 μm), which is a carbon fiber composite sheet suitable for use as a catalyst backing layer
in the PEM electrolyzer stack.
13
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
4.4 Bipolar and End Plates
Bipolar plates can be made from several materials, including metals with good corrosion
resistance such as stainless steel or from carbon composites made through injection molding or
powder metallurgy (Wei et al. 2014). In this study, we assumed a stamped stainless-steel plate
(thickness=5 mm) that is coated with a very thin gold layer (100 nm) to improve its corrosion
resistance and surface finish.
As shown in Figure 5, the process for producing metal bipolar plates starts by making stainless
steel blanks from the received coils. Then, the required channels are created on both sides of the
sheet using a stamping die. After that, the stamped parts are cleaned in a chemical bath to
remove dirt and grease, and they are then inserted into the physical vapor deposition machine.
Temperature and voltage are then adjusted to create the required environment for gold to
vaporize and bombard the plate surface to make a very thin gold layer. This coating process
produces better corrosion resistance parts and improves the durability of the stainless-steel plates
(Kumar at al., 2010; Yoon et al., 2008).
Figure 5. Process flow for producing metal bipolar plates
4.5 Stack Assembly
Most of the electrolyzer stack assembly lines today rely less on automated operations than
manual ones, where workers stack, align, and connect the components to produce an electrolyzer
stack. However, electrolyzer manufacturers can replicate battery assembly line automation in the
fuel cell and electrolyzer assembly lines by investing in increasing the level of automation and
adding more robots to the assembly line. And, investing in automation should be linked to the
expected benefits (cost, time, and quality), so any investment in the automation level for
assembly line should be justified at least by the production volumes and payback periods. In this
study, we assumed three different levels of automation in the stack assembly line that correspond
to the annual production volume. We assumed a manual assembly line for the low production
volumes (<100k MEAs/yr), where most of the assembly steps are made manually by skilled
workers. A semi-automated assembly line was assumed for medium production volumes
(100,000–700,000 MEAs/yr), and a fully automated assembly line was assumed for high
production volumes (>700k MEAs/yr).
14
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
The stack assembly process in the semi-automatic stack assembly line is shown in Figure 6. This
line combines the framed MEAs with the bipolar plates and assembles them in the electrolyzer
stack. The proposed numbers of annual MEAs and level of automation were validated by our
industrial collaborators. In the automated case, a robotic feed of plates is followed by screen
printing or injection molding of the gaskets and UV curing steps. The plate/MEA are then
stacked and gently compressed to add the compression bands or tie rods to hold the stack parts
together and decrease the gaps between parts before proceeding to the next step, where balanceof-stack parts are added to the system. In the last step, the stack undergoes multiple stages of
conditioning and testing.
15
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
Figure 6. Process flow for semi-automatic assembly line
CT=cycle time
16
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
5 Results and Discussion
5.1 Cost of the Stack Parts
The manufacturing cost per produced item is typically high at low-production volumes and
therefore some manufacturers may find it more economic to outsource some of these parts rather
than produce them in-house. However, this analysis assumed all stack components—except those
specifically mentioned in Section 4—are manufactured in-house. In this section, we discuss
individual component cost breakdowns in natural units (e.g., $/m2 for the CCM or $/piece for
the plate) and normalized units in $/kW for 200-kW and 1-MW PEM electrolysis systems;
these system sizes were selected as baselines for small and large size (MW-scale) electrolysis
systems respectively
Figure 7 shows the cost curves for CCM made via spray coating in $/m2 and for the total stack
cost in $/kW. Economies of scale have greater impact on the overall cost because the capital and
building costs are divided over more units. In many cases, cost curves for the individual stack part
and for the whole stack start to flatten out (i.e., be less steep) at annual production rates of 1,000
units per year or more. For both 200-kW and 1-MW systems, CCM cost is dominated by the
Nafion membrane and precious metal (Pt and Ir used in the catalyst layers) which are mixed with
Nafion ionomer and other solvents to make the catalyst ink.
When we look at the cost curve for the PTL (Figure 8), we see that material cost starts to
dominate at production rates of 100 units/yr or more for the 200-kW electrolyzer and 20 units/yr
or more for the 1-MW system. The cost of titanium powder is still much lower than that of
precious materials (Pt and Ir) and the expensive membrane used in the CCM. The expensive
coating material (gold) also adds extra cost to the Ti-based PTL. Contributions of the overhead
cost (building and capital costs) start to decrease at higher production rates because of the impact
of economies of scale. A comparison between Ti-based and carbon cloth- based PTL is shown in
Figure 9, which shows that Ti-based PTL from both sides could be competitive at higher
production rates. Purchased carbon cloth seems to be cheaper and suitable to be used in the
cathode side of the MEAs. Carbon cloth (cathode) and Ti-based PTL (anode) are assumed as a
base case in this study.
Cost curves for the MEA frame made by injection molding process is shown in Figure 10. We
can see that capital and building cost dominate at most annual production rates. Cost curves for
stamped and coated bipolar plates show that materials dominate the cost at high production rates,
leaving less than 10% of the total cost for other cost contributors starting at 1,000 units/yr or more
(Figure 11). Labor cost here is nominal because of the underlying assumption that we need small
labor-hours per piece because the blanking and stamping processes are batch processes where
several pieces can be produced at one time, and many units can be inserted in one batch in the
physical vapor deposition machine.
For stack assembly process cost analysis, we used normalized units ($/kW) because unlike other
parts in the stack, there is no clear natural unit to allocate stack assembly cost to. The
manufacturing cost chart for stack assembly is shown in Figure 12, which reveals that the biggest
contributor in the stack assembly is the labor cost at the low production rates where the manual
assembly line is used to assemble the stacks. Semiautomated and fully automated assembly lines
17
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
may be needed for production volumes that exceed 1,000 stacks per year. Direct material cost
here includes the cost of the stainless-steel end plates and compression bands.
The cost breakdown in Figure 12c for the 200 kW system shows sort of a sharp change in the
capital cost contribution between 100 systems/yr and 1,000 systems/yr. The cause of the change
comes from the change from the manual assembly line to semi-automated assembly line which
occurs at an annual production rate of 1,000 system/yr (equivalent to 102,000 MEAs), and
another change to a fully-automated line occurs at 10,000 systems/yr (equivalent to 1,020,000
MEAs). Similarly, for the 1 MW stack (Figure 12d) we switched from manual assembly line to
semi-automated line at annual production rate of 1,000 system/yr (equivalent to 509,000 MEAs).
Another change from semi-automated to fully automated assembly line takes place at annual
production rate of 2,000 system/yr (equivalent to 1,018,000 MEAs).
Balance of stack cost covers the cost of some parts (e.g., stack housing, manifolds, wires,
insulation material, compression bands, etc.). The cost of balance of the stack is assumed to be
13% of the total stack cost. This estimate is based on average values from other cost studies (see
for example Ayers, 2016, Ayers et al., 2015)
18
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
(a) (b)
(c) (d)
Figure 7. Manufacturing cost curves for CCM made via spray coating in (a) CCM cost for 200-kW system in $/m2, (b) CCM cost for
200-kW system $/kW, (c) CCM cost for 1-MW system in $/m2, and (d) CCM cost for 1-MW system in $/kW
Annual production rate is the number of systems produced in one year.
19
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
(a) (b)
(c) (d)
Figure 8. Manufacturing cost curves for the titanium-based PTL in (a) $/piece for 200-kW system, (b) $/kW for 200-kW system,
(c) $/piece for 1-MW system, and (d) $/kW for 1-MW system
The annual production rate is the number of electrolyzer systems produced in one year.
20
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
Figure 9. Cost of carbon cloth vs. Ti-based PTL
21
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
(a) (b)
(c) (d)
Figure 10. Manufacturing cost curves for the frame in (a) $/piece for 200-kW system, (b) $/kW for 200-kW system,
(c) $/piece for 1-MW system, and (d) $/kW for 1-MW system
The annual production rate is the number of electrolyzer systems produced in one year.
22
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
(a) (b)
(c) (d)
Figure 11. Manufacturing cost curves for the stamped stainless-steel plates bipolar plates in (a) $/piece for 200-kW system, (b) $/kW for
200-kW system, (c) $/piece for 1-MW system, and (d) $/kW for 1-MW system
The annual production rate is the number of electrolyzer systems produced in one year.
23
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
(a) (b)
(c) (d)
Figure 12. Manufacturing cost analysis for stack assembly process: (a) cost curve as a function of the annual production rate for 200-
kW system, (b) cost breakdown as a function of the annual production rate for 200-kW system, (c) cost curve as a function of the annual
production rate for 1-MW system, and (d) cost breakdown as a function of the annual production rate for 1-MW system
The annual production rate is the number of electrolyzer systems produced in one year.
24
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
5.2 Balance-of-Plant Cost
As discussed in Section 2, the “balance of plant” (BOP) consists of several subsystems that
complement the function of the stack. Table 5 summarizes our cost estimates for the key parts in
the BOP for a 1-MW system. To determine the cost of each component in the BOP, we collected
cost data from direct quotes we received from parts vendors and from discussions with industry
advisors to estimate the cost of the general-purpose parts such as stainless-steel pipes, pressure
gauges, and water pumps.
The system discussed here reflects our best assessment of the existing or similar systems, but it
does not necessarily capture all system components with exact fidelity to existing commercial
systems. Moreover, existing physical or commercial systems may not have the exact design or
parts we describe here. Thus, this analysis should be used as an informative tool, and it should
not be considered an analysis of any commercial products.
Because many generic parts are used in the BOP, there is a potential room for savings by
purchasing larger quantities. In this analysis, we applied the discount values as a function of
purchase quantity, using the quotes we received directly from sales representatives. We also
assumed a 20% price scaling for a 10x-factor increase in the purchased quantity for the generic
and power electronics parts that did not come with direct quotes from the part vendors (Wei et
al., 2014; Saggiorato et al. 2017; Contini et al., 2017). The rationale behind this assumption is
that other clean energy technologies (e.g., photovoltaic solar cells and li-ion batteries) have
experienced significant cost reductions in the past decade or so (more than 20% reduction in the
price for doubling of the cumulative shipped volume (Liebreich, 2014). We think that fuel cells
and electrolyzers could follow such trend in the coming years when the production volumes
become at scale. Other factors that could also play role in reducing the cost of these parts are
improvements in the part performance, thus less material or smaller parts could be manufactured
in the future and improvements in the manufacturing processes of these parts. Schmidt et al.,
(2017b) estimated the learning experience rate for fuel cells and electrolyzers to be around 18%
compared to 12% for li-ion batteries used in residential and utility applications. This means we
could see larger cost reductions in the fuel cells and electrolyzers prices with production
volumes.
The cost breakdown of the BOP in Figure 13a and 13b shows that about 29% of the BOP part
cost for the 200-kW and half the cost in the 1-MW system come from the power supplies, which
includes an expensive AC/DC rectifier that is designed to supply certain current to the cells in
the stack. Cost breakdown in Figures 13a and 13b is based on purchasing 1 unit. Cost curve for
other annual production rates (a proxy of the purchased quantities) is shown in Figures 13c and
13d for 200 kW and 1 MW systems, respectively. For the 1-MW system, a deionized water
circulation system and a hydrogen processing unit contribute to about one-fifth each. Cooling
system shares about 11% and 7% of the total BOP part cost for the 200-kW and 1-MW systems
respectively.
The cost of the oxygen tank is relatively high because we assume it is made from 316 stainless
steel, electropolished, passivated, pickled, oxygen-cleaned tank; rated at 150 psi working
pressure (ASME-stamped). However, other cheaper alternatives can also be used in the BOP, for
example we can use a smaller size atmospheric vessel that does not capture oxygen which could
cost one-third to one-fourth the cost of the stainless-steel tank. A polypropylene-based tank could
25
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
also be used for just a few thousand dollars. Overall, using cheaper tanks could save a couple
dollars per kW in the system cost, but that means that pure oxygen is vented to the atmosphere
and we lose a high value by-product which can be sold for other end-uses.
26
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
(a) (b)
(c) (d)
Figure 13. Cost breakdown for the BOP parts for (a) 200-kW system (cost for 1 item) and (b) 1-MW system (cost for 1 item), (c) cost
breakdown as a function of the annual production rate for 200-kW system, and (d) cost curve as a function of the annual production rate
for 1-MW system
27
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
Table 5. Cost of the Balance-of-Plant Parts (cost of one item)
System Subsystem 200 kW 1 MW
Power Supplies Power Supply $44,000 $198,000
DC Voltage Transducer $225 $225
DC Current Transducer $340 $340
Total $44,565 $198,225
Deionized Water
Circulation
Oxygen Separator Tank† $20,000 $40,000
Circulation Pump $7,053 $10,962
Polishing Pump $2,289 $5,000
Piping $10,000 $15,157
Valves and Instrumentation
• Pressure, temperature, conductivity, flowmeter
• A Class I, Division 2, Group B rating drives up prices.
$7,500 $11,368
Controls $2,000 $4,595
Total $48,842 $87,082
Hydrogen Processing Dryer Bed $13,860 $36,589
Water/Hydrogen Separator $10,000 $26,390
Tubing $5,000 $7,579
Valves & Instrumentation
• Pressure, temperature, conductivity, flowmeter
$5,000 $7,579
Controls $2,500 $5,743
Total $36,360 $83,880
Cooling Plate heat exchanger $9,000 $10,525
Cooling pump $1,500 $3,797
Valves, instrumentation $2,000 $4,595
28
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
Piping $1,000 $2,297
Dry cooler $4,000 $7,464
Total $17,500 $28,679
Miscellaneous Valve air supply – nitrogen or compressed air $2,000 $2,000
Ventilation and safety requirements
• Combustible gas detectors
• Exhaust ventilation
$2,000
$2,000
$2,000
$2,000
Total $6,000 $6,000
BOP Grand Total $153,267 $403,865
BOP Cost $766/kW $404/kW
† This cost is for 316SS, electropolished, passivated, pickled, oxygen-cleaned tank; 150 psi working pressure rating, ASME-stamped. It has multiple large
nozzles integrated into the design for versatility and expansion, plus vortex breaker, and has large manway access for oxygen-cleaning operation.
5.3 PEM Electrolyzer System Cost
Stack and system costs are shown in Figures 14 and 15, respectively. The stack cost curves in Figures 14a and 14b show the effect of
the annual production rates on the total stack cost for 200-kW and 1-MW stacks respectively. As with the trends we saw in the cost
analysis for stack parts, we expect stack cost to decrease with higher annual production rates. Figure 14c and 14d show that stack cost
is dominated by the CCM cost, followed by the following parts in order from high-cost to low-cost contributions: PTL, assembly and
end-plates, bipolar plates and frame/seal. The CCM consists of a Nafion membrane and platinum group metals, where Nafion
membrane shares about one-third to half of the CCM cost and 13-46% for PGM catalyst.
There is no clear cutoff identifying the point where economies of scale are met on the stack cost, but based on current market demands
and our experience, that producing 1,000 electrolyzer stacks per year is within the range that is considered “economies of scale.”
29
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
(a) (b)
(c) (d)
Figure 14. Manufacturing cost curve for (a) 200-kW PEM electrolyzer stack, (b) manufacturing cost curve for 1-MW PEM electrolyzer
stack, (c) cost breakdown for 200-kW stack, and (d) cost breakdown for 1-MW stack
The annual production rate is the number of electrolyzer systems produced in one year.
30
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
The system cost shown in Figure 15 is the summation of the stack and BOP costs. BOP costs for 200-kW and 1-MW systems
dominate the total system cost across all annual production rates. Since BOP parts are outsourced from part vendors, we do not expect
economies of scale to have the same effect on the system cost as in the case of stack that is manufactured in-house. Power electronics
including power supplies (AC/DC rectifier), current and voltage transducers, dominate the BOP cost. Similar findings were also
observed in the stationary fuel cell systems where power electronics share significant part of the BOP cost (see Wei et al., 2014,
Collela et al., 2014; James et al., 2015). It seems that a follow-up work is needed to study the key cost drivers in the production of the
power electronics for PEM electrolyzer system. The second cost contributor at the BOP is the deionized water circulation unit, which
contains an expensive water/oxygen separation tank that separates oxygen and water coming out of the stack.
31
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
(a) (b)
(c) (d)
Figure 15. Cost curves for (a) 200-kW and (b) 1-MW electrolyzer systems showing costs of stack and BOP, and cost breakdown for (c)
200-kW and (d) 1-MW electrolyzer systems at different annual production rates
The annual production rate is the number of electrolyzer systems produced in one year.
32
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
6 Sensitivity Analysis and Potential Cost Reductions
Sensitivity analysis allows us to study the impact on the overall stack and system costs of
changing certain parameters in the manufacturing process or varying some parameters in the cell
design. While we tried to use consistent values in this analysis (±20% of the base value for each
parameter), we thought that some parameters may change beyond this range in the near term. For
example, some manufacturers are working to reduce the platinum group metal loadings from 11
g/m2 that are currently used in some commercial system to less than 1 g/m2 in the near term (see
for example Ayers 2015; Yu et al., 2015; Xu 2016). Nafion 117 membrane is expensive. Today,
there are several cheaper alternatives used in PEM electrolysis environment such as SPEEK
(sulfonated poly(ether ether keton)) and Solvay Aquivion PFSA (perfluorosulfonic
acid) membranes (Hansen et al., 2012)
A sensitivity analysis at the stack level was made for 200-kW and 1-MW systems at different
production volumes (as shown in Figure 16). We can see that stack cost is more sensitive to
manufacturing process yields (including process yeild for CCM coating, PTL powder
metallurgy, plate stamping and coating, and stack assembly) and power density. Pt loading and
Nafion membrane cost are among some of the important factors that have large impacts on the
stack cost. This is unsurprising for high-cost materials, especially when material cost starts to
dominate at high production volumes. The cost of commodities such as titanium, stainless steel
and PPS-40%GF is not a large factor in relative to the manufacturing yield, power density, and
platinum loading.
(a)
33
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
(b)
(c)
34
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
(d)
Figure 16. Impact of changing some manufacturing and cell design parameters on 200-kW PEM
stack cost: (a) at 100 units/yr, and (b) at 1,000 units/yr, and 1-MW stack cost at (c) at 100 units/yr,
and (d) at 1,000 units/yr
The annual production rate is the number of electrolyzer systems produced in one year.
Pt loading was varied between 11 g/m2 (nominal value) and 1 g/m2, Membrane cost for Nafion 117
(thickness=178μm) from DuPont (base case) and Aquivion ES98-09S (thickness=90μm) from Solvay
We also investigated the potential areas where we could potentially target a cost reduction,
including cost reductions from changing certain design parameters or the costs of certain key
materials used in the PEM stack. We found that manufacturing engineering and economies of
scale play a key role in reducing the cost of the PEM system (Figure 17). Some design changes
in the MEA cells, such as reductions in platinum group metal loading and any possible cost
reduction in the membrane cost, could also play role in decreasing the cost of the electrolyzer
system. A 20% improvement in the power density and using cheaper membrane could reduce the
cost of the stack significantly. Cost of the power electronics remains the largest portion of the
cost in the PEM electrolyzer system. So, we expect that any reduction in the power electronics
cost to have a great impact in the PEM electrolyzer cost, as shown in Figure 17.
The combination of the abovementioned scenarios could reduce the cost of the PEM electrolyzer
stack from $237/kW (±10%) at a production volume of 10 MW (e.g., 1-MW systems at a
production rate of 10 units/year) to $69/kW at 1,000 MW (e.g., 1-MW systems at 1,000
unit/year). System cost, including stack and balance of plant, could also be reduced through
manufacturing economies of scale, improvements in power density, reduction in platinum group
35
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
metal loading and membrane cost, and reductions in power electronics – from $561/kW (±10%)
for the 1-MW electrolysis system at 10 units/year to $265/kW (±10%) at 1,000 units/year.
(a)
(b)
Figure 17. Waterfall charts showing areas where R&D can play a role in reducing the cost of the
electrolysis system for (a) 200 kW system and (b) 1-MW system
Assumptions: improvement in power density (+20%); Pt loading from 11 g/m2 to 1 g/m2, membrane cost (Nafion 117
vs. Solvay E98-09S), and power electronics (-20%). Economy of scale is the manufacturing cost of 10 units/yr vs. 100
units/yr vs. 1,000 units/yr.
36
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
7 Installed System Cost
Installed system cost was estimated using the following assumptions:
• A markup factor (50% of the total system cost) accounts for profit margin, general and
administration, sales and marketing, warranty costs, and other such costs. This estimate for
the “factory gate price” is consistent with the previous technoeconomic studies for fuel
cells (see James and DeSantis 2015; Saggiorato et al. 2017; Wei et al. 2014)
• Another 33% was added to the factory gate price to estimate the installation cost (Wei et
al. 2014)
Figure 18 shows the installed system cost for 200-kW and 1-MW PEM electrolyzer systems.
Both markup and installation costs depend on the estimated system cost and follow the same
trend of the system cost. That means we expect markup and installation cost to decrease with
annual production rates and the expected impact of economies of scale in all cost components,
including the markup factor. Additional cost reductions may be possible due to learning and
cumulative experience that are developed by system providers and installer with time (Mayyas
and Mann 2018).
(a)
37
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
(b)
Figure 18. Installed system cost for (a) 200-kW PEM electrolyzer system, and (b) 1-MW PEM
electrolyzer system
Other technoeconomic studies reported similar cost ranges. For example, Strategic Analysis Inc.
estimated the uninstalled PEM electrolysis system cost to be around $940/kW (in 2012 dollars)
(Colella et al., 2014). Their estimate for future forecourt that can produce up to 1,500 kg-H2 per
day is $450/kW. In this report, authors also the potential cost reduction of huge central PEM
plant that can produce up to 50,000 kg-H2 per day. Their estimate for capital cost of the future
central PEM plant could reach as low as $400/kW. Thomas (2018), as part of the cost analysis
done for Hydrogenics, estimated the price of a MW-scale PEM electrolysis system to be around
$1,000/kW by 2030, and $550/kW by 2050. This price, however, can be reduced to $700/kW
and $385/kW for multi-MW system in 2030 and 2050, respectively.
38
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
8 Effect of Electrolyzer Capital Cost on the Hydrogen
Production Cost
We used the H2A4 model to study the effect of decreasing the capital cost of the electrolyzer on
the hydrogen production cost. Figure 19 shows several scenarios of capital cost for 1 MW
electrolysis system using two annual production rates: 10 units/yr and 1,000 units per year. These
production rates, in our opinion, could represent the current production volumes and future
production rates at economies of scale. We also tried to combine this effect with another
important parameter, electricity price. If we look at the capital cost contribution for 97% capacity
factor (i.e., the percentage of time we use the electrolyzer to generate hydrogen), we can see that
the cost of hydrogen can be lowered by (1) reducing the capital cost of the electrolyzer and (2)
using less-expensive electricity in the electrolysis process. However, if the capacity factor of the
electrolyzer is decreased to lower values, we expect the capital cost contribution to increase
because of spreading the capital cost over a shorter period of operation periods and smaller
amounts of the generated hydrogen.
Figure 19. Effect of the capital cost, capacity factor, and electricity price on the cost of hydrogen
production (excluding compression, storage and dispensing CSD cost)
Assumptions: (1) 1-MW PEM electrolyzer, (2) system cost includes markup factor (50%), and (3) economies of scale:
cost of producing 10 units/yr (cost is $841/kW) versus 1,000 units/yr (cost is $462/kW)
4 For information about H2A model, see “DOE H2A Analysis,” https://www.hydrogen.energy.gov/h2a_analysis.html.
39
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
9 Conclusions
The development of high throughput, automated processes achieving high yield are estimated
to push the cost per kilowatt for the PEM electrolyzer stack to $125/kW (±10%) for an overall
production volume of 100 MW (e.g., 1-MW systems x 100 units/year). The stack cost could be
pushed as low as $90/kW (±10%) at 50,000 systems/year. At low volumes the stack cost is
sharply reduced when moving from a production volume of 10 to 1,000 systems per year,
because tool utilization increases rapidly, and capital and facility costs drop sharply.
Direct material costs dominate stack costs at high volume. For the PEM electrolyzer stacks,
depending on the annual production rate, we found that CCM manufacturing cost is about 26%–
47% for 200-kW PEM stack and about 36%–47% for the 1-MW stack, with PTL contributing
around 17%–25% of the stack cost, bipolar plates about 12%–21%, and end plates and assembly
near 3%–13%. In terms of cost-dominating factors at the stack level, it was found that
manufacturing process yield, power density, gold layer thickness on PTL and bipolar plates and
Pt loading and/or Pt price contribute most to the overall stack cost.
Balance-of-plant costs for a 1-MW electrolyzer contribute to about two-thirds of the system cost,
with power electronics contributing half the BOP cost, while the water circulation and hydrogen
processing subsystems each share about one-fifth of the BOP cost. System cost including stack
and BOP could also be pushed down with economies of scale. The uninstalled 1 MW system
cost could be reduced from $560/kW at 10 units/year to $258/kW at 10,000 units/year.
Electricity price and electrolyzer capital cost are the most important factors that determine the
cost of hydrogen production in the water electrolysis process, so any cost reduction in the
electrolyzer cost would reflect in lowering the cost of hydrogen generation process.
40
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
References
AFDC (Alternative Fuels Data Center). n.d. “Hydrogen Production and Distribution.”
U.S. Department of Energy. https://www.afdc.energy.gov/fuels/hydrogen_production.html
Air Products. 2013. Steam Methane Reformer: Overview. Air Products. (35981) 352-13-008-US.
http://www.airproducts.com/~/media/Files/PDF/industries/energy/energy-hydrogen-steammethane-reformer-datasheet.pdf.
Anderson E., Ayers, K., Capuano, C., Szymanski, S. 2013. Long Life PEM Water Electrolysis
Stack Experience and Future Directions. Technical Forum Hannover Messe, Germany. 9 April
2013
Ayers, K.E. Renner, J.N. Danilovic, N., Wang, J.X., Zhang, Y., Maric, R., Yu, H. 2016.
Pathways to ultra-low platinum group metal catalyst loading in proton exchange membrane
electrolyzers. Catalysis Today262(2016) 121–132
Ayers, K. 2015. Single Step Manufacturing of Low Catalyst Loading Electrolyzer MEAs. U.S.
DOE Advanced Manufacturing Office Program Review Meeting Washington, D.C. May 28-29,
2015. https://www.energy.gov/sites/prod/files/2015/06/f23/P7-
AMO%20Merit%20Review%202015%20-%20Proton%20Final.pdf
Ayers, K.E., C. B. Capuano, and E. B. Anderson. 2012. “Recent Advances in Cell Cost and
Efficiency for PEM-Based Water Electrolysis.” ECS Transactions 41 (10):15–22.
Ayers, K. 2015. Single Step Manufacturing of Low Catalyst Loading Electrolyzer MEAs.
Advanced Manufacturing Office Annual Merit Review. Washington, D.C. May 28-29, 2015.
https://www.energy.gov/sites/prod/files/2015/06/f23/P7-
AMO%20Merit%20Review%202015%20-%20Proton%20Final.pdf
BEA (U.S. Bureau of Economic Analysis). n.d. “Table C. BEA Rates of Depreciation, Service
Lives, Declining-Balance Rates, and Hulten-Wykoff Categories.”
Bertuccioli, L., Chan, A., Hart, D., Lehner, F. Madden, B. Standen, E. 2014. Development of
Water Electrolysis in the European Union. Fuel Cells and Hydrogen Joint Undertaking, February
2014.
Carmo, M., Fritz, D., Maier, W., Stolten, D. 2015. Alkaline Water Electrolysis vs. PEM Water
Electrolysis - Exploring their Full Performance. 227th ECS Meeting. Chicago, 2015.
CBRE. n.d. Fit-Out Cost Guide: Occupier Project Management, EMEA, 2014 Edition.
Colella, W.G., James, B.D., Moton, J.M., Saur, G., Ramsden, T. 2014. Techno-economic
Analysis of PEM Electrolysis for Hydrogen Production. Strategic Analysis Inc. Electrolytic
Hydrogen Production Workshop. NREL, Golden, Colorado. February 2014.
41
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
Contini, V., Eubanks, F., Heinrichs, M., Valluri, M., Jansen, M., George, P., Mansouri, M. 2016.
Manufacturing Cost Analyses of Fuel Cell Systems for Primary Power and Combined Heat and
Power Applications. Battelle 3/31/2017.
https://www.energy.gov/sites/prod/files/2017/05/f34/fcto_bop_workshop_contini.pdf
Haberl, J.S. (1993). Economic Calculations for the ASHRAE Handbook. Energy Systems
Laboratory (http://esl.tamu.edu), Texas A&M University; Department of Mechanical
Engineering, Texas A&M University.
Hamdan, M. 2011. Synergy of Giner, Inc./GES Technologies.
https://www.energy.gov/sites/prod/files/2014/03/f12/webinarslides052311_pemelectrolysis_ham
dan.pdf
Hamdan, M. 2013. PEM Electrolyzer Incorporating an Advanced Low-Cost
Membrane. Washington, D.C.: U.S. Department of Energy. DOE/GO/18065-22.
https://www.osti.gov/servlets/purl/1091385.
Hansen, M.K. Aili, D., Christensen, E., Pan, C., Eriksen, S., Jensen, J.O., Barner, J.H., Li, Q.,
Bjerrum, N.J. 2012. PEM steam electrolysis at 130 °C using a phosphoric acid doped short side
chain PFSA membrane. International Journal of Hydrogen Energy 37, 10992-11000
Howe-Baker International. 2017. Recovery and purification of Hydrogen using PSA technology.
https://howe-baker.com/recovery-and-purification-of-hydrogen-using-psa-technology/
James, B., Colella, W., Moton, J., Saur, G., Ramsden, T. 2013. PEM Electrolysis H2A
Production Case Study Documentation.
https://www.hydrogen.energy.gov/pdfs/h2a_pem_electrolysis_case_study_documentation.pdf
James, B.D., D.A. DeSantis. 2015. Manufacturing Cost and Installed Price Analysis of
Stationary Fuel Cell Systems. Revision 3, 30 September 2015.
https://www.sainc.com/assets/site_18/files/publications/sa%202015%20manufacturing%20cost
%20and%20installed%20price%20of%20stationary%20fuel%20cell%20systems_rev3.pdf
Kumar, A., Ricketts, M., Hirano, S. Ex situ evaluation of nanometer range gold coating on
stainless steel substrate for automotive polymer electrolyte membrane fuel cell bipolar plate.
Journal of Power Sources 195 (2010) 1401–1407
Lettenmeier, P., Kolb, S., Sata, N., Fallisch, A. Zielke, CL. Thiele, S., Gago A.S., Friedrich,
K.A. 2017. Comprehensive investigation of novel pore-graded gas diffusion layers for highperformance and cost-effective proton exchange membrane electrolyzers. Energy Environ. Sci.,
10, 2521-2533.
Liebreich, M. 2015. Bloomberg New Energy Finance Summit 2015. New York, April 2015.
https://data.bloomberglp.com/bnef/sites/4/2015/04/BNEF_2014-04-08-ML-SummitKeynote_Final.pdf
Mayyas, A. Mann, M. Emerging Manufacturing Technologies for Fuel Cells and Electrolyzers. Accepted
for publication in the Procedia Manufacturing/Elsevier, 2018.
42
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
Pomerleau, Kyle. 2014. Corporate Income Tax Rates around the World, 2014. Washington,
D.C.: Tax Foundation. No. 436. https://files.taxfoundation.org/legacy/docs/FF436_0.pdf.
Saggiorato, N., Wei, M., Lipman, T., Mayyas, A., Chan, S.H., Breunig, H., McKone, T., et al. 2017.
A Total Cost of Ownership Model for Low Temperature PEM Fuel Cells in Combined Heat
and Power and Backup Power Applications. Berkeley, CA: Lawrence Berkeley National
Laboratory.
https://www.energy.gov/sites/prod/files/2017/02/f34/fcto_2016_tco_model_low_temp_pem_fc.pdf.
Schmidt, O., Gambhir, Staffell, A. I., Hawkes, Nelson, A. J. Few, S. Future cost and performance of
water electrolysis: An expert elicitation study. International journal of hydrogen energy 42 (2017)
30470-30492
Schmidt, O., Hawkes, A. I., Gambhir, A., Staffell, I. 2017. The future cost of electrical energy
storage based on experience rates. Nature Energy 2, 17110.
THOMAS, D. 2018. Cost reduction potential for electrolyser technology. European Power-to-Gas.
18 June 2018, Berlin. http://europeanpowertogas.com/wpcontent/uploads/2018/06/20180619_Hydrogenics_EU-P2G-Platform_for-distribution.pdf
Turner & Townsend. n.d. A Brighter Outlook: International Construction Cost Survey 2013.
http://www.turnerandtownsend.com/media/1459/1349-1-icc-survey-brochureflipbook-final.pdf.
Wei, M., Lipman, T., Mayyas, A., et al. 2014. A Total Cost of Ownership Model for Low
Temperature PEM Fuel Cells in Combined Heat and Power and Backup Power Applications.
Environmental Energy Technologies Division. October 2014.
https://www.energy.gov/sites/prod/files/2016/12/f34/fcto_tco_model_low_temp_pem_fc.pdf
PDR 3 (Hilton Chicago)
Xu, H. High-Performance, Long-Lifetime Catalysts for Proton Exchange Membrane
Electrolysis. Hydrogen and Fuel Cell Technologies office Annual Merit Review. Washington,
D.C. June 8, 2016. https://www.hydrogen.energy.gov/pdfs/review16/pd103_xu_2016_o.pdf
Yoon, W., Huang, X., Fazzino, P., Reifsnider, K.L. Akkaoui, M.A. 2008. Evaluation of coated
metallic bipolar plates for polymer electrolyte membrane fuel cells. Journal of Power Sources
179, 265–273.
Yu, H., Danilovic, N., Zhao, S., Wang, Y., Capuano, C., Mustain, W.E., Ayers, K E. Maric, R.
2015. Manufacturing of Low Catalyst Loading PEM Electrolyzer Meas Using Reactive Spray
Deposition Technology. 227th ECS Meeting. May 24-28, 2015, Chicago, IL.
https://ecs.confex.com/ecs/227/webprogram/Paper48975.html
43
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
Appendix A. Functional Specification
Functional specifications were estimated based on the average values for commercial PEM
electrolyzers with similar size in kW. Some examples of these commercial systems and their
specifications are summarized in Table A1.
Functional cell dimensions were estimated based on typical cell size in some commercial PEM
electrolyzers. Schematic of the cell dimensions including plate area, CCM coated area and cell
active area, are shown in Figure A1 below. These areas were used in the bottom-up
manufacturing cost analysis to determine the required material per system. Bipolar plate area was
assumed to be 957 cm2
, while cell total coated area =748 cm2 with cell active area=680 cm2
,
assuming 9% of the CCM coated area will be lost in bonding CCM to the seal/frame. Total frame
width is 2.445 cm which includes 0.625 cm of each side that overlaps with the MEA and another
1.82 cm of each side that extend outside the MEA area. These estimates are based on suggested
values by some of our industry advisors.
Figure A1. Functional cell dimensions
Loadings in (g/m2
) of the platinum group metal (PGM) on anode and cathode side of the
membrane were estimated based on discussions with industry advisors who suggested loadings
of 7 g/m2 of platinum on the anode side and 4 g/m2 of platinum-iridium on the cathode side.
Current density and reference voltage at the cell level are two important parameters that play role
in determining the cell efficiency and energy consumption per kg-H2. We used average values
from several polarization curves to estimate cell current density and voltage. Some examples of
the polarization curves used in this analysis are shown in Figure A2. Power density was then
used to calculate number of cells per stack to match it with the system size in kW.
44
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
(a)
(b)
Figure A2. Example of the polarization curves for PEM electrolyzer cells
Source of Images: Proton Onsite (Anderson et al. 2013) and Giner (Hamdan 2011)
45
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
Table A1. Examples of commercial PEM electrolyzer and their specifications
Specificati
ons
Hydroge
nics†
Hydroge
nics†
Proton
OnSite†
†
Proton
OnSite†
†
Proton
OnSite†
†
Proton
OnSite††† Giner‡ Siemens‡‡ Units
Model
Number
HyLYZE
R™-1
HyLYZE
R™-2 H2 H2 H6
FuelGen1
2, Series
2
Merrim
ack
SILYZER
200 basic
Rated
stack
Consumpti
on 7.20 14.40 14.00 28.00 40.00 45.00 160.00 1250.00 kW
Startup
time:
millise
cond
scale < 10 sec Sec
Hydrogen
purity
(dep. on
operating
point):
99.999
5%
99.999
5%
99.999
5% 99.9995%
99.5% –
99.9%
Specific
Energy
Consumpti
on 6.70 6.70 7.30 7.00 6.80 7.50 5.56
kWh/N
m3
Net
Production
Rate 1 2 2 4 6 6 30.59 225 Nm3/h
Net
Production
Rate (scfh) 38 76 76 152 228 228 1162 8,550 scfh
Net
Production
Rate
(kg/day) 2.16 4.32 4.31 8.63 12.94 12.95 66.00 485.46 kg/day
Turndown
Ratio
0 to
100%
0 to
100%
net
product
delivery
(Autom
atic)
0 to
100%
net
product
delivery
(Autom
atic)
0 to
100%
net
product
delivery
(Autom
atic) 10:1 %
Output
pressure Up to 7.9 Up to 7.9 15
0-40
bar Up to 35 bar
Feed
Water
Potable
main
water
supply
Fresh
water
demand: 1 1 1.83 3.66 5.5 54 1.5
ltr /
Nm³ H2
Inlet water
pressure 0.7-6.9 0.7-6.9 1.5 to 4 1.5 to 4 1.5 to 4 1 to 10 barg
Relative
Humidity 0 to 90%
0 to
90%
0 to
90%
0 to
90% %
Power
Supply
208/120,3 phase,4
wire+gnd,50/60 Hz
200-260,1 phase,2
wire+gnd, 50/60 Hz
Direct connection to
DC possible upon
request.
380 to
480
VAC, 3
phase,
50 or
60 Hz
380 to
480
VAC, 3
phase,
50 or
60 Hz
380 to
480
VAC, 3
phase,
50 or
60 Hz
420-480
VAC, 3
phase, 60
Hz, 112
FLA
46
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
Cooling
strategy
Air
Cooled
Air
Cooled
Liquid
cooled
8.1 kW
Liquid
cooled
16.1
kW
Liquid
cooled
23.7
kW Air Cooled
Operating
Temperatu
re 5 to 40 5 to 40 5 to 60 5 to 60 5 to 60 -23 to 46 °C
Dimension
s
0.75 X
0.66 X
1.17
1.30 X
1.00 X
1.25
180 cm
x 81
cm x
191 cm
180 cm
x 81
cm x
191 cm
180 cm
x 81
cm x
191 cm
2.18
X0.84
X1.91
6.3 X 3.10
X 3.00
mXmX
m
Weight 250 275 682 858 908 900 17000 kg
† http://www.hydrogenics.com/wp-content/uploads/2-1-1-1-hylyzer-1-223F620871645.pdf
†† https://www.protononsite.com/sites/default/files/2019-02/H%20Series.pdf
††† http://proton.artbizcreative.com/backend/arc_contenido/archivo21.pdf
‡ https://h2agentur.de/en/pem-electrolysis-stacks/#merrimack
‡‡ https://www.siemens.com/content/dam/webassetpool/mam/tag-siemens-com/smdb/corporatecore/sustainable_energy/hydrogensolutions/brosch%C3%BCren/silyzer200-broschure-en.pdf
47
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
Appendix B. Bottom-Up Costing Analysis
In this appendix, we discuss the economic analysis used in developing the direct manufacturing
cost analysis. The model was adopted from the ASHRAE handbook; see Haberl (1993) and Wei
et al. (2014) for details about the model. Below are definitions of terms used in developing
economic equations:
abr is the building area (m2
)
Ce is the energy cost for one accounting period (i.e., one year) ($).
Cf is the factory floor space cost ($/m2
).
Clabor is the labor rate per hour ($/hr).
Cs,assess is the initial assessed system value ($).
Cs,salvage is the system salvage value at the end of its useful life in constant dollars.
Cs init is the initial system cost ($).
Cy is the annualized system cost in constant dollars ($/yr).
Dk,sl or Dk,SD is the amount of depreciation at the end of period k depending on the type
of depreciation schedule used, where Dksl is the straight-line depreciation method and
DkSD represents the sum-of-digits depreciation method in constant dollars.
F is the future value ($).
imPk is the interest charged at the end of period k ($).
i'= (id-j)/1+j) is the effective discount rate adjusted for energy inflation, sometimes called
the real discount rate.
i"= (id-je)/1+ je) is the effective discount rate adjusted for energy inflation je.
i is the annual insurance costs.
ITC is the investment tax credit for energy efficiency improvements, if applicable.
48
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
j is the general inflation rate per period.
jd is the discount rate.
jbr is the building depreciation rate.
je is the general energy inflation rate per period.
jm is the average mortgage rate (real rate + general inflation rate).
k is the end if the period(s) in which replacement(s), repair(s), depreciation, or interest
is calculated.
M is the periodic maintenance cost ($).
n is the number of period(s) under consideration (years).
P is the sum of money at the present time (i.e., its present value) ($).
Pk is the outstanding principle of the loan for C-s,init at the end of period k in current
dollars.
Rk is the net replacement(s), repair cost(s), or disposals at the end of period k in
constant dollars.
Tinc is the (state tax rate + federal tax rate) - (state tax rate X federal tax rate) where tax
rates are based on the last dollar earned (i.e., the marginal rates).
Tprop is the property tax rate.
Tbr is the salvage value of the building ($).
For any proposed capital investment, the capital and interest costs, salvage costs, replacement
costs, energy costs, taxes, maintenance costs, insurance costs, interest deductions, depreciation
allowances, and other factors have to be weighed against the value of the services provided by
the system (Haberl 1993).
B.1 Single Payment
The present value or present worth factor (PWF) is a common method for analyzing the impact
of a future payment on the value of money at the present time. The primary underlying principle
is that all present and future payments (in and out) can be evaluated according to their present
purchasing power using a discounted cash flow method. The relationship between the present
value p and the future value F with compound interest rate i and accounting periods n can be
calculated as follows:
𝐹𝐹 = 𝑝𝑝(1 + 𝑖𝑖)𝑛𝑛
49
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
The relationship between the present value P or present worth factor PWF and the future sum of
money F is given by:
𝑃𝑃 = 𝐹𝐹
(1 + 𝑖𝑖) � 𝑛𝑛 = 𝐹𝐹 × 𝑃𝑃𝑃𝑃𝑃𝑃(𝑖𝑖, 𝑛𝑛)
where PWF(i,n) the present worth factor and can be calculated using the following equation:
𝑃𝑃𝑃𝑃𝑃𝑃(𝑖𝑖, 𝑛𝑛) = 1
(1 + 𝑖𝑖) � 𝑛𝑛
B.2 Accounting for Varying Inflation Rates
Inflation is another important economic parameter that needs to be considered when converting
future values to present values or vice versa. Inflation rate accounts for the rise in costs of goods
and services over time. Inflation has an adverse effect on the economy, so governments—
through their central banks—try to limit it and avoid deflation in order to keep the economy
running smoothly. One way to account for inflation in economic calculations is to use interest
rates that account effectively for varying rates of inflation. Haberl (1993) suggested the
following effective interest rate i', sometimes called the real rate, which considers the effects of
general inflation j and the discount rate id. Effective interest rate can be expressed as follows:
𝑖𝑖
′ = 1 + 𝑖𝑖𝑑𝑑
1 + 𝑗𝑗 − 1 = 𝑖𝑖𝑑𝑑 − 𝑗𝑗
1 + 𝑗𝑗
However, this expression can also be used to account for energy inflation by considering the
general discount rate id and the energy inflation rate je, thus:
𝑖𝑖′′ = 1 + 𝑖𝑖𝑑𝑑
1 + 𝑗𝑗𝑒𝑒
− 1 = 𝑖𝑖𝑑𝑑 − 𝑗𝑗𝑒𝑒
1 + 𝑗𝑗𝑒𝑒
Based on these equations, we can revise the equation of the future value F, using constant
currency of an invested sum P with a discount rate 𝑖𝑖𝑑𝑑 under inflation i during n periods:
𝐹𝐹 = 𝑃𝑃[
1 + 𝑖𝑖𝑑𝑑
1 + 𝑗𝑗
]
𝑛𝑛 = 𝑃𝑃(1 + 𝑖𝑖′
)𝑛𝑛
The present worth P, in constant dollars, of a future sum of money F with discount rate 𝑗𝑗𝑑𝑑
under inflation rate j during n periods is:
𝑃𝑃 = 𝐹𝐹/[
1 + 𝑗𝑗𝑑𝑑
1 + 𝑗𝑗
]
𝑛𝑛
In constant currency, the present worth P of a sum of money F can be expressed using
the effective interest rate 𝑖𝑖′, which is adjusted for inflation by:
𝑃𝑃 = 𝐹𝐹
(1 + 𝑖𝑖′) � 𝑛𝑛 = 𝐹𝐹 × 𝑃𝑃𝑃𝑃𝑃𝑃(𝑖𝑖′, 𝑛𝑛)
Similarly, the effective present worth factor PWF can be calculated using the following equation:
50
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
𝑃𝑃𝑃𝑃𝑃𝑃(𝑖𝑖′, 𝑛𝑛) = 1
(1 + 𝑖𝑖′) � 𝑛𝑛
B.3 Recovering Capital as a Series of Payments
Another important economic concept is the recovery of capital as a series of uniform payments
or what is called the capital recovery factor. It is commonly used to describe periodic uniform
mortgage or loan payments. S is the ratio of the periodic payment to the total sum being repaid.
The discounted sum S of such an annual series of payments A invested over n periods with
interest rate i is given by:
𝑆𝑆 = 𝐴𝐴[1 ± (1 + 𝑖𝑖)−𝑛𝑛/𝑖𝑖
𝐴𝐴 = (𝑆𝑆 × 𝑖𝑖)/[1 + (1 + 𝑖𝑖)−𝑛𝑛/𝑖𝑖
𝐶𝐶𝐶𝐶𝐶𝐶(𝑖𝑖, 𝑛𝑛) = 𝑖𝑖
[1 − (1 + 𝑖𝑖)−𝑛𝑛]
= 𝑖𝑖(1 + 𝑖𝑖)𝑛𝑛
(1 + 𝑖𝑖)𝑛𝑛 − 1
Table B-1 summarizes some of the mathematical formulas used in calculating these
cost components.
Table B.1. Cost Components and Their Mathematical Formulas [from Haberl (1993)]
Cost Component Formula
Building cost Cbr = 𝐶𝐶𝐶𝐶𝐶𝐶𝑚𝑚 × 𝑐𝑐𝑓𝑓𝑓𝑓 × 𝑎𝑎𝑏𝑏𝑏𝑏
Capital and Interest (𝐶𝐶𝐶𝐶𝐶𝐶𝑖𝑖,𝑖𝑖𝑖𝑖𝑖𝑖𝑖𝑖 − 𝐼𝐼𝐼𝐼𝐼𝐼)𝐶𝐶𝐶𝐶𝐶𝐶(𝑖𝑖
′
, 𝑛𝑛)
Depreciation
𝑇𝑇𝑖𝑖𝑖𝑖𝑖𝑖 �[𝐷𝐷𝑘𝑘𝑃𝑃𝑃𝑃𝑃𝑃(𝑖𝑖𝑑𝑑, 𝑘𝑘)]
𝑛𝑛
𝑘𝑘=1
𝐶𝐶𝐶𝐶𝐶𝐶(𝑖𝑖′
, 𝑛𝑛)
Insurance 𝐼𝐼(1 − 𝑇𝑇𝑖𝑖𝑖𝑖𝑖𝑖)
Interest tax deduction
𝑇𝑇𝑖𝑖𝑖𝑖𝑖𝑖 �[𝑗𝑗𝑚𝑚𝑃𝑃𝑘𝑘−1𝑃𝑃𝑃𝑃𝑃𝑃(𝑖𝑖𝑑𝑑, 𝑘𝑘)]
𝑛𝑛
𝑘𝑘=1
𝐶𝐶𝐶𝐶𝐶𝐶(𝑖𝑖′
, 𝑛𝑛)
Maintenance 𝑀𝑀(1 − 𝑇𝑇𝑖𝑖𝑖𝑖𝑖𝑖)
Operating energy 𝐶𝐶𝑒𝑒[
𝐶𝐶𝐶𝐶𝐶𝐶(𝑖𝑖′
, 𝑛𝑛)
𝐶𝐶𝐶𝐶𝐶𝐶(𝑖𝑖′′, 𝑛𝑛)
](1 − 𝑇𝑇𝑖𝑖𝑖𝑖𝑖𝑖)
Principle Pk during year K
at market mortgage rate im 𝑃𝑃𝑘𝑘 = (𝐶𝐶𝑖𝑖,𝑖𝑖𝑖𝑖𝑖𝑖𝑖𝑖 − 𝐼𝐼𝐼𝐼𝐼𝐼) �(1 + 𝑗𝑗𝑚𝑚)𝑘𝑘−1
+ (1 + 𝑗𝑗𝑚𝑚)𝑘𝑘−1 − 1
(1 + 𝑗𝑗𝑚𝑚)−𝑛𝑛 − 1 �
51
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
Cost Component Formula
Property tax 𝐶𝐶𝑠𝑠,𝑎𝑎𝑎𝑎𝑎𝑎𝑎𝑎𝑎𝑎𝑎𝑎𝑇𝑇𝑝𝑝𝑝𝑝𝑝𝑝𝑝𝑝(1 − 𝑇𝑇𝑖𝑖𝑖𝑖𝑖𝑖)
Replacement or disposal �[𝑅𝑅𝑘𝑘𝑃𝑃𝑃𝑃𝑃𝑃(𝑖𝑖′
, 𝑘𝑘)]
𝑛𝑛
𝑘𝑘=1
𝐶𝐶𝐶𝐶𝐶𝐶(𝑖𝑖′
, 𝑛𝑛)( 1
− 𝑇𝑇𝑖𝑖𝑖𝑖𝑖𝑖)
Salvage value (𝐶𝐶𝑠𝑠,𝑠𝑠𝑠𝑠𝑠𝑠𝑃𝑃𝑃𝑃𝑃𝑃(𝑖𝑖′
, 𝑛𝑛)𝐶𝐶𝐶𝐶𝐶𝐶(𝑖𝑖′
, 𝑛𝑛)(1
− 𝑇𝑇𝑠𝑠𝑠𝑠𝑠𝑠𝑠𝑠)
52
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
Appendix C. Assumptions Used in Developing the
Direct Manufacturing Costs Analysis
Following tables summarize some important manufacturing process parameters and some related
part specifications used in developing the bottom-up manufacturing cost models.
Table C.1. Manufacturing parameter for spray coating process of the catalyst coated membrane
Parameter Value Source/Notes
Nafion membrane cost Variable (the lowest assumed
value= $500/m2
)
Coating line cost
(Ultrasonic Spray Coating)
$1,000,000 Based on similar spray coating
lines used in production of
photovoltaic, li-ion battery
electrodes, etc.
Coating line footprint 88.2 m2
Spray coating process yield 90%
Line speed 50 cm/min http://www.sonotek.com/flexicoat-oversizeultrasonic-coating-system/
Web width 109 cm Width of 4 CCMs
Platinum group metal
loading
7 g/m2 (anode): Pt only
4 g/m2
: 1:1 Pt:Ir
Using similar values for
commercial PEM systems
Pt price $1,500/tr.oz FCTO value for 2017
Ir price $23.63/g Average spot price for 2017
Nafion ionomer $1.53/g D2020 Nafion Dispersion -
Alcohol based 1000 EW at 20
wt%
Solvents $10 per gallon Alcoholic solvent
Workers/line 2 workers Hourly paid workers
53
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
Table C.2. Manufacturing parameter for Powder metallurgy of the Porous Transport Layer
Parameter Value Source/Notes
Titanium powder
cost
$35/kg Average price for high purity Titanium powder
Powder metallurgy
production line
$1,500,000 Includes compacting press, sintering oven, powder
mixing system, powder pumping system and
quality control unit
Gold coating layer 100 nm
$41 per gram
Kumar at al., (2010); Yoon et al., (2008). Physical
vapor deposition (PVD)
Carbon cloth cost $200-500/m2 Carbon cloth: Toray Paper 090 - TGP-H-090
(thickness = 280 μm)
Physical Vapor
Deposition Machine
$400,000
Production line
footprint
150 m2
Powder metallurgy
process yield
99%
Coating process
yield
99.9
P/M Line throughput 2 pieces/min
Workers/line 4 workers Hourly paid workers
(2 workers for P/M line, and 2 workers for coating
production line)
54
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
Table C.3. Manufacturing parameter for injection molding of the Seal/Frame
Parameter Value Source/Notes
Width of the
frame
0.625 cm from all
edges of the MEA
Total frame width=
2.445 cm
PPS-40%GF
resin cost
($/kg)
$15.40/kg http://www.plasticsnews.com/resin/hightemperature-thermoplastics/current-pricing
Injection
molding
production line
$700,000 Includes injection molding machine, curing
oven, and quality control unit
Production line
footprint
100 m2
Process yield 99%
Line
throughput
2 pieces/min Including the time required for injection molding
and quality checking
Workers/line 2 workers Hourly paid workers
55
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
Table C.4. Manufacturing parameter for stamped and coated bipolar plates
Parameter Value Source/Notes
Stainless steel
316L cost
$5/piece Plate area 957.44 cm2
Gold coating
layer
100 nm
$41 per gram
Kumar at al., (2010); Yoon et al., (2008).
Physical vapor deposition (PVD)
Consumables
cost
$0.60/piece Including alcohol for cleaning
Production line $1,500,000 Includes stamping press, PVD machine, quality
control unit (scanning electron microscope and
material characterization)
Production line
footprint
100 m2
Stamping
process yield
95%
PVD coating
process yield
99.9%
Stamping line
throughput
11 pieces/min Using precise stamping press
Workers/line 3 workers Hourly paid workers
56
This report is available at no cost from the National Renewable Energy Laboratory (NREL) at www.nrel.gov/publications.
Table C.5. Manufacturing parameter for stack assembly process
Parameter Value Source/Notes
Assembly line
type
Variable 3 assembly lines assumed in this study: manual (for
MEAs≤100,000/yr; semi-automatic ≤700,000, and
fully automatic (MEAs≥700,000)
Assembly line $0.5M (manual)
$ 1M (Semiautomatic)
$ 2M (Automatic)
Includes robots, compacting press, stack
conditioning station, and quality testing station
Production line
footprint
150 m2 For each assembly line. More than 1 assembly line
may be needed for larger annual production rates.
Assembly
yield
99.5%
Index time
(assembly
time)
Variable Depending on the stack size in kW (i.e., number of
assembled MEAs per stack)
Line
throughput
11 pieces/min Using precise stamping press
Workers/line 4 or 3 or 2 Hourly paid workers. 4 workers/line for manual
assembly, 3 workers/line for semi-automatic, and 2
workers/line for fully automatic line
