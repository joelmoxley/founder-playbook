Here's an example of a description that appears under a link.

15 MIN READ || Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Credit: [Ricardo PLC](http://www.ricardo.com/)

 {! search-content: !}


Cover Page

														
	Manufacturing Cost Model													
														
	Released:		23-Dec-15											
	Author: Piyush Bubna, Ricardo Strategic Consulting													
														
			Only for use by ARPA-E staff and work on ARPA-E awards											
														
														
														
			This model calculates cost of forming and assembling of components. The file consists of a cost model template and supporting database in different spreadsheets. The model is provided as is. In case of any questions or difficulties with using the model please contact the author.											
														
PROTECTED RIGHTS NOTICE 
These protected data were produced under agreement no.DE-AR0000522 with the U.S. Department of Energy and may not be published, disseminated, or disclosed to others outside the Government until 5 years after development of information under this agreement, unless express written authorization is obtained from the recipient. Upon expiration of the period of protection set forth in this Notice, the Government shall have unlimited rights in this data. This Notice shall be marked on any reproduction of this data, in whole or in part 
														



Cost Model Template

																											
	Legend																										
	User Input																										
	Default Values																										
	Sub-calculations																										
	Final Calculation																										
																											
																											
	Door Trim Main Panel Cost Model																										
															Annual plant operating  hours	4800											
	Component			Production Cost							Process and Calculations																
	Name	Description		Production Volume	300000	200000	100000	50000	10000	1000	Manufacturing Processes	Required Equipment and Tooling	# of Parts out per hit		Tooling Cost ($)	Machine Cost ($)	Process Time (secs)	Annual Production Volume:	300000	200000	100000	50000	10000	1000	NOTES		
	Door Trim Main Panel	Mass (kg)	1.35	Total Capital Cost for  5 yrs (Million $)	2.07	1.39	0.71	0.71	0.68	0.68	Injection Molding	3000 ton press	1	1			44.0	# of machines	1	1	1	1	1	1			
		Length (mm)		Total Unit  Cost ($/piece)	5.33	5.34	5.37	6.79	18.10	143.20		Tooling	1	1	 $680,000 			# of tools	3	2	1	1	1	1			
		Width (mm)		Capital Cost ($/piece)	1.38	1.39	1.42	2.84	13.60	136.00		Robot Arm	1	1	 $30,000 			# of tools	1	1	1	1	0	0			
		Height (mm)		Total Process Burden Cost ($/piece)	1.56	1.56	1.56	1.56	2.03	4.38																	
		Thickness		Material Cost ($/piece)	2.16	2.16	2.16	2.16	2.16	2.16																	
		Material	PP-TD30	Scrap Reclaim ($/piece)	0.00	0.00	0.00	0.00	0.00	0.00																	
				Markup ($/piece)	0.23	0.23	0.23	0.23	0.30	0.66																	
																		Tooling Life (number of hits)	 500,000 	 500,000 	 500,000 	 500,000 	 500,000 	 500,000 	Directional tooling price and life available in "Tooling Data" sheet		
				Shipping cost not included in this template														Total Tooling Cost ($)	 $2,070,000 	 $1,390,000 	 $710,000 	 $710,000 	 $680,000 	 $680,000 			
																		Tooling cost per unit ($/piece)	 $1.38 	 $1.39 	 $1.42 	 $2.84 	 $13.60 	 $136.00 			
																											
																		Tooling Changeover Frequency	12	12	12	12	12	12	# of batches for annual volume production		
																		Tooling Changeover Time (hrs)	0	0	0	0	1.5	1.5	Available in "Process Data" sheet		
																		Process Time (sec)	44	44	44	44	44	44			
																		Annual Processing Hours	3666.7	2444.4	1222.2	611.1	122.2	12.2			
																		Annual Production Hours	3666.7	2444.4	1222.2	611.1	140.2	30.2			
																		Process Rate ($/hr)	 $127.50 	 $127.50 	 $127.50 	 $127.50 	 $145.00 	 $145.00 	Process rate and process time available in "Process Data" or can be calculated in "Process Rate Calculator" Sheet		
																		Process Rate ($/piece)	 $1.56 	 $1.56 	 $1.56 	 $1.56 	 $2.03 	 $4.38 			
																		Markup ($/piece)	 $0.23 	 $0.23 	 $0.23 	 $0.23 	 $0.30 	 $0.66 			
																		Raw Material Quantity (% of part weight)	100%	100%	100%	100%	100%	100%	recommendations available in "Common Assumptions"		
																		Material (kg)	1.35	1.35	1.35	1.35	1.35	1.35			
																		Material Rate ($/kg)	 $1.60 	 $1.60 	 $1.60 	 $1.60 	 $1.60 	 $1.60 	recommendations available in "Common Assumptions"		
																		Material Cost ($/piece)	 $2.16 	 $2.16 	 $2.16 	 $2.16 	 $2.16 	 $2.16 			
																		% of scrap that can be salvaged	100%	100%	100%	100%	100%	100%	recommendations available in "Common Assumptions"		
																		Scrap (kg)	0.00	0.00	0.00	0.00	0.00	0.00			
																		Scrap reclaim price ($/kg)	 $0.16 	 $0.16 	 $0.16 	 $0.16 	 $0.16 	 $0.16 	Generally 10% of material rate;  Aluminum is salvaged at original price		
																		Scrap Reclaim ($/piece)	 $-   	 $-   	 $-   	 $-   	 $-   	 $-   			
																											
																											
																											
																											
	

Common Assumptions
											
	Plant Parameters	Value	Units	Notes		Utility Rates	Value	Units			
	Annual operating hours	4800	hrs/yr	Two 10 hr shifts, 5 days week, 49 weeks		Energy	0.12	$/kWh			
	Wage (including benefits)	45	$/hr								
	Equipment Installation & Commisioning	10%		% of direct equipment cost		Material Rates	Value	Units			
	Equipment Financing Interest Rate	8%				Aluminum Billet Rate	2.08	$/kg			
	Equipment Financing Period	12	years			Steel (DP600)	0.85	$/kg			
	Property tax	1.0%		% of annual cost of direct equipment		Steel (Hot rolled HSLA)	0.80	$/kg			
	Equipment Insurance	0.5%		% of annual cost of direct equipment		Steel (Hot rolled Mild Steel)	0.73	$/kg			
	Spare parts, Maintenance, Repairs	3.0%		% of annual cost of direct equipment		Steel (> 1000 Mpa)	1.5	$/kg			
	Indirect Equipment & other hardware cost	4.4%		% of ammortized equipment cost		Natural Rubber	7.7	$/kg			
	Overhead	122.20	$/sq.m/yr			Polypropylene, 20% Talc Filled	1.8	$/kg			
	Useful Tooling Life	5	years			Polypropylene, 30% Talc Filled	1.6	$/kg			
						Polypropylene, 40% Talc Filled	1.4	$/kg			
	Operational Assumptions	Value	Units	Notes		PBT	2.86	$/kg			
	Raw Material Quantity (% of part weight)					PET	3.125	$/kg			
	Stamped Parts	115%				PE	1	$/kg			
	Die Castings	130%				POM	3.7	$/kg			
	Carbon Fiber Panels	105%				Polycarbonate	2.75	$/kg			
	Injection/Blow molded plastic/rubber parts	100%				PMMA	2.69	$/kg			
	Scrap Salvage Quantity (% of excess raw material)					PPS	4.65	$/kg			
	Stamped Parts	100%				UP (MD60+GF20)	3.36	$/kg			
	Die Castings	75%				PA66-GF30	4	$/kg			
	Carbon Fiber Panels	100%				RTM resin	8.8	$/kg			
	Scrap Reclaim Price (% of raw material cost)					CFRP Fabric	30	$/kg			
	Stamping	10%				PET Sheet (0.1 mm thick)	3.35	$/kg			
	Casting	100%				ABS	2.6	$/kg			
	"Markup (includes profit, SG&A, packaging, process development costs and coverage of rejects)
"					PUR Foam (2mm thick)	0.3	$/sq.m			
	Markup	15%		% of value-added (process cost)		Recycled Fiber (for acoustic)	0.11	$/sq.m			
						Closed Cell Foam	0.35	$/sq.m			
						Primer Paint	25	$/gal			
						Chrome Paint	75	$/gal			
						Clear Coat	40	$/gal			
											
											
						Shipping	Value	Units			
						Distance	200	miles			
						Freight Rate	2	$/mile			
						Available Payload	21100	kg			
						Available Volume	67.7	cu.m			
						Shipping cost ($/kg)	0.02				





Process Data
						
		Important Information				
		Burdened Process Rate includes equipment ammortization, direct and indirect labor, maintenance, utlities, floor space, insurance, tax and supporting plant equipment				
		Process time is the time elapsed per hit before a part or batch of parts come out of the process line. It is NOT the total cycle time from start to finish. The values provided below are typical for the parts and machines analyzed in this program. The values may vary based on part size and design features				
		High volume = production volume of > 30,000 /yr; Low volume = production volume of < 30,000/yr				
		Time lost in tooling changeover is applicable for low volume (<30,000/yr) only.				
						
	Manufacturing Process	Tonnage (Volume)	Burdened Process Rate ($/hr)	Process Time (sec/hit)	Tooling Changeover Time (hrs)     (<30,000 volume)	Notes
	Cold Stamping	50 -200 ton press	72	2	5	Burdened Process Rate Includes 1 direct manpower @ $45/hr
	Cold Stamping	200-600 ton press	111	4.7	5	
	Cold Stamping	600 - 1000 ton press	136	6.2	5	
	Cold Stamping	1000 - 1500 ton press	199	7.65	5	
	Cold Stamping	1500 - 2000 ton press	261	10	5	
	Cold Stamping	2000 - 2500 ton press	352	11.8	5	
	Hot Stamping	1000 - 1500 ton press	300	20	5	Burdened Process Rate includes 1 direct manpower @ $45/hr
	Extrusion		300	2 secs/meter	0.5	
	High Pressure Die Casting	2500 ton press	340	103	5	Burdened Process Rate includes die casting press, trimming, washing and inspection stations and 3.2 direct manpower @ $45/hr
	CNC Machining	Clutch Housing - High Volume	56	642 secs/pc		Burdened Process Rate includes 0.38 direct manpower
	CNC Machining	Clutch Housing - Low Volume	86	642 secs/pc	5	Burdened Process Rate includes 1 direct manpower
	Automated Sand Casting	High Volume	511	11.6		8 parts per hit
	Automated Sand Casting	10,000/yr volume	145	24.3	5	4 parts per hit
	Automated Sand Casting	1,000/yr volume	78.5	121	10	1 part per hit
	CNC Machining	Differential Carrier	115	250 secs/pc	2.5	
	Manual Sand Casting	Door Hinges - High Volume	100	11.6		8 parts per hit
	Manual Sand Casting	Door Hinges - 10,000/yr volume	60	24.3	2.5	4 parts per hit
	Manual Sand Casting	Door Hinges - 1,000/yr volume	25	121	2.5	1 part per hit
	Rubber Molding	High Volume	400 (16 parts/hit)	360		Engine Mount
	Rubber Molding	Low Volume	50 (1 part/hit)	360	2.5	Engine Mount
	Injection Molding	3000 (High Volume)	127.5	44		Process Rate includes 0.5 direct labor and a robot for parts handling
	Injection Molding	3000 (Low Volume)	145	44	1.5	Process rate includes 1 direct labor and no automation for parts handling
	Injection Molding	1500 (High Volume)	78.5	33		Process Rate includes 0.5 direct labor and a robot for parts handling
	Injection Molding	1500 (Low Volume)	96	33	1.5	Process rate includes 1 direct labor and no automation for parts handling
	Injection Molding	800 (High Volume)	56.5	39		Process Rate includes 0.5 direct labor and a robot for parts handling
	Injection Molding	800 (Low Volume)	74	39	1.5	Process rate includes 1 direct labor and no automation for parts handling
	Injection Molding	500 (High Volume)	45.5	30 - 36		Process Rate includes 0.5 direct labor and a robot for parts handling
	Injection Molding	500 (Low Volume)	63	30 - 36	1.5	Process rate includes 1 direct labor and no automation for parts handling
	Injection Molding	200 (High Volume)	35.5	30		Process Rate includes 0.5 direct labor and a robot for parts handling
	Injection Molding	200 (Low Volume)	53	30	1.5	Process rate includes 1 direct labor and no automation for parts handling
	Injection Molding	60 (High Volume)	31	40		Process Rate includes 0.5 direct labor and a robot for parts handling
	Injection Molding	60 (Low Volume)	48.5	40	1.5	Process rate includes 1 direct labor and no automation for parts handling
	Injection Molding	10 (High Volume)	24.5	30		Process Rate includes 0.5 direct labor and a robot for parts handling
	Injection Molding	10 (Low Volume)	47	30	1.5	Process rate includes 1 direct labor and no automation for parts handling
	Blow Molding	Low complexity ducts (High Volume)	44.5	30		
	Blow Molding	Low complexity ducts (Low Volume)	64	30	1.5	
	Blow Molding	High complexity ducts (High Volume)	72.3	40		
	Blow Molding	High complexity ducts (Low Volume)	91.5	40	1.5	
	Aluminum Vapor Deposition	300 parts per rack	53	2400 secs/rack	1	Headlight Reflectors
	Die Cutting	Insert/Armrest Skin and Door Foams	47	10	1.5	19 pcs /hit  for Insert skin; 60 pcs/hit for armrest skin; 48 pcs/hit for door foams
	Painting (non-class A)	55 parts per rack	53	840 secs/rack	0	
	CFRP Preforming and Ultrasonic Cutting 	i3 floor	90	57.6	2	includes robots for part transfer and 1 direct labor for operation of whole process line
	CFRP RTM and Sand Blasting	i3 floor	59.5	230.4	2	includes robots for part transfer and 0.1 direct labor for operation of whole process line
	Water Jet Cutting	i3 floor	10	39.4 secs/meter	0.5	No direct labor required. Process time depends on cutting length






Process Rate Calculator
Process Rate Calculation Table (Default values for B-Pillar low volume (10k-1k) assembly)			Hourly Rate
a	Direct Equipment Cost	$300,000 	
b	Installation & Comissioning	10%	
c	Installed Direct Equipment cost (includes a & b)	$330,000 	
d	Financing Interest Rate	8%	
e	Financing Period (years)	12	
f	Annual Cost of Direct Equipment (calculated from c, d & e)	 $42,865 	
g	Property Tax (% of annual cost of equipment)	1%	
h	Equipment Insurance (% of annual cost of equipment)	0.5%	
i	Equipment Spare parts, Maintenance, Repairs (% of annual cost of equipment)	3%	
j	Total annual cost associated with direct equipment (includes f, g, h & i)	 $44,794 	 $9.33 
k	Indirect equipment & other hardware (% of direct equipment)	4.40%	
l	Overhead ($/sq.m/yr)	122.20	
m	Equipment Space Requirement (sq.m)	450	
n	Indirect annual equipment & Overhead Cost (calculated from k, l & m)	 $56,961 	 $11.87 
o	Energy Consumption (kWh/hr)	4.11	
p	Electricty Rate ($/kWh)	0.12	
q	Energy Cost (calculated from o & p)		 $0.49 
r	Burdened Labor Rate ($/hr)	45	
s	Direct Labor (# of people)	1	
t	Direct Labor Cost (calculated from r & s)		 $45.00 
	Annual operating hours per year	4800	
	Total Process Rate ($/hr) (sum of j, n, q, & t)	 	 $66.69 






Assembly Operation Data
Assembly Equipment Cost	
Spot Weld Gun	 $95,000 
MIG Weld Gun	 $75,000 
Adhesive Gun	 $75,000 
Hemming Press	 $200,000 
Transfer Robots	 $70,000 
Stationary Welder	 $55,000 
	
Energy Consumption	
Spot Welding	0.002 kWh/weld
MIG Welding	4.5 kW (rating)
Adhesive Application 	30 kW (rating)
Laser Welding	115 kW (rating)
	
Consumables	
Adhesive	$ 0.28/meter
Inert Gas	$ 3.60/hr
MIG wire	$ 0.03/ft
	
Welding Speed	
Spot Welding	2 - 3 secs/weld
MIG welding	1 inch/sec






Tooling Data
													
	Tooling cost based on part size (includes dies, fixtures, check fixtures)					Note: Tooling costs for different processes in this table do not include cost of part specific robot end effectors. Cost of end effectors is included in analysis 10 key components of Toyota Corolla and A8/i3 where applicable							
	Process	Part Size	Tooling Cost      (USD)	Tooling Life         (# of hits)									
	Stamping	 Large 	 $1,000,000 	 1,500,000 									
	Stamping	 Medium 	 $500,000 	 1,500,000 									
	Stamping	 Small 	 $80,000 	 1,500,000 									
	Extrusion	 All sizes 	 $1000 - $5000 	 1,500,000 									
	High Pressure Die Casting	 Large 	 $450,000 	 100,000 									
	High Pressure Die Casting	 Medium 	 $300,000 	 100,000 									
	Automated Sand Casting	 Medium (High Volume) 	 $23,000 	 1,500,000 									
	Automated Sand Casting	 Medium (Low Volume) 	 $6,000 	 1,500,000 									
	Manual Sand Casting	 Small (High volume) 	 $20,000 	 1,500,000 									
	Manual Sand Casting	 Small (Low Volume) 	 $5,600 	 1,500,000 									
	Machining	 Large 	 $165,000 	 1,500,000 									
	Machining	 Small - Medium 	 $5000 - $10000 	 1,500,000 									
	Rubber Mold	 Medium (High Volume) 	 $70,000 	 1,500,000 									
	Rubber Mold	 Medium (Low Volume) 	 $10,000 	 1,500,000 									
	Injection Molding	 Large 	 $ 0.5 - 1 MM 	 500,000 									
	Injection Molding	 Medium 	 $200,000 	 500,000 									
	Injection Molding	 Small 	 $50,000 - $100,000 	 500,000 									
	Blow Molding	 Large 	 $115,000 	 1,500,000 									
	Blow Molding	 Medium 	 $25,000 - $50,000 	 1,500,000 									
	Aluminum Vapor Deposition	 Any size 	Negligible										
	Die Cutting	 Any size 	$1000 - $5000	 1,500,000 									
	Painting (non class - A)	 Any size 	Negligible										
	Carbon Fiber Preforming	 Medium 	 $150,000 	 50,000 									
	Resin Transfer Molding	 Medium 	 $150,000 	 50,000 									
	Water Jet Cutting	 Medium 	 $10,000 	 1,500,000 									
	Robot end effectors (part specific)	 Medium 	 $150,000 	N/A									
	Robot end effectors (part specific)	 Small 	 $30,000 	N/A									
	Welding Turntable Tooling per station	 Large 	 $100,000 										
	Welding Turntable Tooling per station	 Medium 	 $70,000 										
	Welding Turntable Tooling per station	 Small 	 $50,000 										
	Assembly Check Fixture	 Any size 	 $25,000 										
