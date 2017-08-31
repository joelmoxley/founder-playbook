Here's an example of a description that appears under a link.

15 MIN READ || This spreadsheet by the MIT Photovoltaic Research Laboratory provides a framework and data to analyze the production and manufacturing costs for mono silicon. 

Credit: [Doug Powell](http://pv.mit.edu/pvmit_people/doug-powell/)

{! search-content: !}

Sheet1

Estimate for Standard mono Si with U.S. Manufacturing																																																	
Doug Powell																																																	
MIT Photovoltaic Research Laboratory																																																	
																																																	
																																																	
	Top-Level Inputs																																																
	Item	Value	Unit																																														
	Module Efficiency	16	[%]																																														
	Cell Thickness	180	[um]																																														
	Ingot Recycled before brick stage	33.8%	[%]																																														
	Ingot Not-Recycled before brick stage	1.5%	[%]																																														
	Wire Sawing Cut Width	130	[um]																																														
	Virgin Silicon Price	23	[$/kg]																																														
	Operator Wage	14.5	[$/hr]																																														
	Technician Wage	20.6	[$/hr]																																														
	Supervisor Wage	27.3	[$/hr]																																														
	Employee Cost Multiplier	1.33	[-]																																														
	Electricity Cost	0.069	[$/kWh]																																														
	Shipping Costs	0	[$/container]																																														
	Uptime	96	[%]																																														
	Nominal WACC	14.00%	[%]																																														
	Expected Price Inflation	0.0%	[%]																																														
	Expected Cost Inflation	0.0%	[%]																																														
	Effective Tax Rate	27.9%	[%]																																														
	SG&A	9.40%	[% of Revenue]																																														
	R&D	1.10%	[% of Revenue]																																														
	Net Working Capital Period	3	[months]																																														
																																																	
																																																	
	Top-Level Outputs																																																
	Variable Cost (w/o depreciation)	0.54	[$/W]																																														
	Variable Cost (w/o depreciation)	86.49	[$/m2]																																														
	Minimum Sustainable Price	0.85	[$/W]		<- To update MSP, use built in Excel Solver. For help, see "Notes" tab																																												
	Minimum Sustainable Price	136.23	[$/m2]																																														
	Capex	0.68	[$/WaCap]																																														
	PP&E Ratio	0.79	[-]																																														
	Silicon Use	4.31	[g/W]																																														
	Gross Margin	36.51	[%]																																														
	Operating Margin (EBIT)	15.07	[%]																																														
																																																	
																																																	
	Cost Breakdown							Allotment [$/W]				Allotment Specific Adder [$/W]																																					
	Item	Cost [$/cell]	Adder [$/W]	Multiplier	Cost [$/m2]	Cost [$/W]	Percentage	Ingot	Wafer	Cell 	Module	Ingot	Wafer	Cell 	Module																																		
	Silicon Feedstock	0.43		1.00	15.85	0.099	18.33%	0.099																																									
	Maintenance		NA	1.00	5.52	0.035	6.38%	0.008	0.005	0.015	0.006																																						
	Labor		NA	1.00	16.70	0.104	19.31%	0.039	0.022	0.022	0.021																																						
	Input Electricity		NA	1.00	7.08	0.044	8.18%	0.008	0.013	0.020	0.003																																						
	Metal Paste	0.140		1.00	5.11	0.032	5.91%			0.032																																							
	Crucible			1.00	0.40	0.002	0.46%	0.002																																									
	Wire	0.065		1.00	2.39	0.015	2.77%		0.015																																								
	Slurry	0.056		1.00	2.06	0.013	2.39%		0.013																																								
	Glass			1.00	5.66	0.035	6.54%				0.035																																						
	Frame			1.00	3.90	0.024	4.51%				0.024																																						
	Encapsulant			1.00	3.64	0.023	4.20%				0.023																																						
	JB and Cable			1.00	4.62	0.029	5.34%				0.029																																						
	Chemicals	0.100		1.00	3.66	0.023	4.23%			0.023																																							
	Backsheet			1.00	4.80	0.030	5.55%				0.030																																						
	Ribbon			1.00	3.79	0.024	4.38%				0.024																																						
	Screens	0.036		1.00	1.32	0.008	1.53%			0.008																																							
	Shipping costs			1.00	0.00	0.000	0.00%				0.000																																						
	Sum of Variable Costs				86.49	0.541	100.00%	0.157	0.068	0.121	0.195																																						
	Depreciation		NA	NA	14.90	0.093		0.023	0.013	0.041	0.015																																						
	SG&A				12.81	0.080																																											
	R&D				1.50	0.009																																											
	Sum of Fixed Costs				29.21	0.183																																											
	Minimum Sustainable Price				136.23	0.851																																											
																																																	
	Manufacturing Cost Calculations																																																
																																																	
	Module Power																																																
	Number of Cells per Module	60.00	[cells/module]																																														
	Area Utilization	89	[%]																																														
	Area of module	1.64	[m^2/module]																																														
	Power Out Per Module	262.50	[W/module]																																														
																																																	
	Silicon Feedstock																																																
	Silicon Density	2329	[kg/m^3]																																														
	Wafer Area	237	[cm^2]																																														
	Mass of Cell 	9.9	[g]																																														
	Total Virgin Si Utilization	0.57	[-]																																														
	Mass of Virgin Si Consumed per Cell at 100% yield	0.02	[kg/cell]																																														
	Dollars per Cell at 100% yield	0.40	[$/cell]																																														
	Yield from this step on	0.922	[-]																																														
	Dollars per Cell	0.43	[$/cell]																																														
	Total Crystallized Si Utilization	0.38	[-]																																														
	Total Mass of Silicon Crystallized per Cell at 100% Yield	0.03	[kg/cell]																																														
																																																	
	Capital Cost																																																
	Reference Plant Output	400.00	[MW/yr]																																														
	Reference Module Efficiency	13.60	[-]																																														
	Maximum Module Output per hour	336	[m^2/hr]																																														
	Module output per m^2	160.00	[W/m^2]																																														
	Maximum Module Output per hour	53,720	[W/hr]																																														
	Adjusted Module Output per hour	47,533	[W/hr]																																														
	Adjusted Module Output per year	416	[MW/yr]																																														
	Maximum Module Output per hour	471	[MW/yr]																																														
	Ingot Equipment Depreciation Period	7	[yr]																																														
	Wafer Equipment Depreciation Period	7	[yr]																																														
	Cell Equipment Depreciation Period	7	[yr]																																														
	Module Equipment Depreciation Period	7	[yr]																																														
	Facility Depreciation Period	25	[yrs]																																														
	Capex Multiplier	1	[-]																																														
					Capex At 100% Yield and Uptime			Capex At Actual Yield and Uptime																																									
	Ingot	Equipment Cost at 100% yield & uptime [$/kg/hr]	Facility Cost at 100% yield & uptime [$/kg/hr]	Equipment [$/WaCap]	Facility [$/WaCap]	Total [$/WaCap]	Equipment [$/(W/yr)]	Facility [$/(W/yr)]	Total [$/(W/yr)]	Straight-Line Depreciation Payment [$/W]																																							
	Czochralski Growth 	201,383	25,732	0.139	0.018	0.157	0.157	0.020	0.177	0.023																																							
	List additional as needed			0.000	0.000	0.000	0.000	0.000	0.000	0.000																																							
				0.000	0.000	0.000	0.000	0.000	0.000	0.000																																							
				0.000	0.000	0.000	0.000	0.000	0.000	0.000																																							
				0.000	0.000	0.000	0.000	0.000	0.000	0.000																																							
				0.000	0.000	0.000	0.000	0.000	0.000	0.000																																							
				0.000	0.000	0.000	0.000	0.000	0.000	0.000																																							
				0.000	0.000	0.000	0.000	0.000	0.000	0.000																																							
				0.000	0.000	0.000	0.000	0.000	0.000	0.000																																							
	Ingot Sum	201,383	25,732	0.139	0.018	0.157	0.157	0.020	0.177	0.023																																							
	Wafer	Equipment Cost at 100% yield & uptime [$/wafer/hr]	Facility Cost at 100% yield & uptime [$/wafer/hr]																																														
	Brick Preparation	910	144	0.024	0.004	0.028	0.027	0.004	0.031	0.004																																							
	Wire Sawing	741	233	0.019	0.006	0.025	0.022	0.007	0.029	0.003																																							
	Slurry & Scrap Collection	1,102	35	0.029	0.001	0.030	0.032	0.001	0.034	0.005																																							
	Inspect and Sort, Package	246	209	0.006	0.005	0.012	0.007	0.006	0.013	0.001																																							
	List additional as needed			0.000	0.000	0.000	0.000	0.000	0.000	0.000																																							
				0.000	0.000	0.000	0.000	0.000	0.000	0.000																																							
				0.000	0.000	0.000	0.000	0.000	0.000	0.000																																							
				0.000	0.000	0.000	0.000	0.000	0.000	0.000																																							
				0.000	0.000	0.000	0.000	0.000	0.000	0.000																																							
	Wafer Sum	2,999	621	0.078	0.016	0.094	0.088	0.018	0.107	0.013																																							
	Cell	Equipment Cost at 100% yield & uptime [$/wafer/hr]	Facility Cost at 100% yield & uptime [$/wafer/hr]																																														
	Wafer Testing	334	315	0.009	0.008	0.017	0.009	0.009	0.018	0.002																																							
	Texture & Damage Etch	1,205	126	0.031	0.003	0.035	0.034	0.004	0.037	0.005																																							
	Emitter Diffusion	1,894	176	0.049	0.005	0.054	0.053	0.005	0.058	0.008																																							
	PSG Removal & Edge Isolate	1,183	75	0.031	0.002	0.033	0.033	0.002	0.035	0.005																																							
	PECVD of SiNx:H	1,224	115	0.032	0.003	0.035	0.034	0.003	0.038	0.005																																							
	Screen Print	1,972	179	0.051	0.005	0.056	0.055	0.005	0.060	0.008																																							
	Co-fire	1,177	122	0.031	0.003	0.034	0.033	0.003	0.036	0.005																																							
	Inspect, Sort, Package	862	517	0.023	0.014	0.036	0.024	0.014	0.039	0.004																																							
	List additional as needed			0.000	0.000	0.000	0.000	0.000	0.000	0.000																																							
				0.000	0.000	0.000	0.000	0.000	0.000	0.000																																							
				0.000	0.000	0.000	0.000	0.000	0.000	0.000																																							
				0.000	0.000	0.000	0.000	0.000	0.000	0.000																																							
				0.000	0.000	0.000	0.000	0.000	0.000	0.000																																							
	Cell Sum	9,852	1,625	0.257	0.042	0.299	0.276	0.046	0.322	0.041																																							
	Module	Equipment Cost at 100% yield & uptime [$/module/hr]	Facility Cost at 100% yield & uptime [$/module/hr]																																														
	Cell Testing	42,924	21,462	0.019	0.009	0.028	0.020	0.010	0.029	0.003																																							
	String, Tab, and Interconnect	40,744	7,545	0.018	0.003	0.021	0.019	0.003	0.022	0.003																																							
	Front Glass Load & Wash	16,556	3,896	0.007	0.002	0.009	0.008	0.002	0.009	0.001																																							
	Encapsulate & Laminate	47,830	12,299	0.021	0.005	0.026	0.022	0.006	0.028	0.003																																							
	Frame and Seal	23,915	7,034	0.010	0.003	0.013	0.011	0.003	0.014	0.002																																							
	J-Box and Potting	12,325	2,054	0.005	0.001	0.006	0.006	0.001	0.007	0.001																																							
	Test, Sort, Package	28,105	22,484	0.012	0.010	0.022	0.013	0.010	0.023	0.002																																							
	List additional as needed			0.000	0.000	0.000	0.000	0.000	0.000	0.000																																							
				0.000	0.000	0.000	0.000	0.000	0.000	0.000																																							
	Module Sum	212,400	76,774	0.092	0.033	0.126	0.097	0.035	0.132	0.015																																							
			Total Sum	0.567	0.110	0.676	0.619	0.119	0.738	0.093																																							
																																																	
	Maintenance																																																
	Equipment percentage of initial investment	5.0%	[-]																																														
	Building percentage of initial investment	3.0%	[-]																																														
		Maintenance Cost [$/W]																																															
	Ingot	0.01																																															
	Wafer	0.00																																															
	Cell	0.02																																															
	Module	0.01																																															
	Total [$/W]	0.03																																															
																																																	
	Labor																																																
		Operator	Technician	Supervisor	Operator [person/shift/MWaCap]	Technician [person/shift/MWaCap]	Supervisor [person/shift/MWaCap]	Operator [person/shift/(MW/yr)]	Technician [person/shift/(MW/yr)]	Supervisor [person/shift/(MW/yr)]	Labor Cost [$/W]																																						
	Ingot [person/shift/(kg/hr)] at 100% yield & uptime 	0.3120	0.0712	0.0191	0.141	0.032	0.009	0.160	0.036	0.010	0.039																																						
	Wafer [person/shift/(wafer/hr)] at 100% yield & uptime 	0.0032	0.0007	0.0002	0.083	0.017	0.005	0.094	0.019	0.006	0.022																																						
	Cell [person/shift/(wafer/hr)] at 100% yield & uptime 	0.0025	0.0013	0.0002	0.066	0.034	0.005	0.071	0.037	0.005	0.022																																						
	Module [person/shift/(module/hr)] at 100% yield & uptime 	0.1426	0.0782	0.0110	0.062	0.034	0.0048	0.065	0.036	0.005	0.021																																						
											0.104																																						
																																																	
	Input Electricity																																																
	Reference Module Efficiency	13.60	[%]																																														
	Ingot Solidification Need	25.40	[kWh/kg]																																														
	Wafering Need at Ref Efficiency	0.200	[kWh/W]																																														
	Cell Need at Ref Efficiency	0.340	[kWh/W]																																														
	Module Need at Ref Efficiency	0.050	[kWh/W]																																														
		At 100% yield [$/W]	Yield from Step	Cost [$/W]																																													
	Ingot Solidification Electricity Cost	0.008	0.922	0.008																																													
	Wafer Electricity Cost	0.012	0.922	0.013																																													
	Cell Electricity Cost	0.020	0.970	0.020																																													
	Module Electricity Cost	0.003	0.990	0.003																																													
	Total Energy Cost			0.044																																													
																																																	
	Yield Loss																																																
	Ingot Yield	1	[-]																																														
	Wafering Yield	0.950	[-]																																														
	Cell Process Yield	0.980	[-]																																														
	Module Process Yield	0.990	[-]																																														
	Total Yield	0.922	[-]																																														
																																																	
																																																	
	Crucible																																																
	Ingot Mass	150	[kg]																																														
	Crucible Cost	400.00	[$/ingot]																																														
	Crucible Uses	5.00	[-]																																														
	Crucibles Cost at 100% yield	0.002	[$/W]																																														
	Yield from this step on	0.922	[-]																																														
	Crucible Cost	0.002	[$/W]																																														
																																																	
	Wire																																																
	Wire Cost	0.50	[$/km]																																														
	Wire Speed	15.00	[m/s]																																														
	Table Speed	210.00	[?m/min]																																														
	Load Length	1.73	[m]																																														
	Kerf Loss per Wire	130.00	[?m]																																														
	Length of wire around each wafer in Load [m]	0.780	[m]																																														
	Time to Cut	12.38	[hr]																																														
	Wire Used Refreshing Web Before Cut	4.4	[km]																																														
	Wire Consumed While Cutting	668.6	[km]																																														
	Total Wire Used per Run	672.9	[km]																																														
	Wire Cost per Run	336.46	[$]																																														
	Wafers Per Run	5581	[wafers]																																														
	Cost per Wafer at 100% yield	0.060	[$/wafer]																																														
	Yield from this step on	0.922	[-]																																														
	Wire Cost per wafer	0.065	[$/wafer]																																														
	Wire consumed per Wafer at 100% yield	121	[m/wafer]																																														
	Wire consumed per Wafer	131	[m/wafer]																																														
	Wire consumed per Wafer at 100% yield	5.0	[km/m2 wafer]																																														
	Wire consumed per Wafer	5.4	[km/m2 wafer]																																														
																																																	
	Slurry																																																
	Slurry Consumption	0.130	[kg/wafer]																																														
	Slurry Cost	1.600	[$/kg]																																														
	Slurry Recovery	75	[%]																																														
	Cost per Wafer at 100% yield	0.052	[$/wafer]																																														
	Yield from this step on	0.922	[-]																																														
	Slurry Cost per wafer	0.056	[$/wafer]																																														
																																																	
																																																	
	Metal Paste																																																
	Cost of Front Silver Paste	562.00	[$/kg]																																														
	Front Silver Paste utilization	0.12	[g/cell]																																														
	Cost of Front Silver Paste	0.06	[$/cell]																																														
	Cost of Rear Silver Paste	562.00	[$/kg]																																														
	Rear Silver Paste utilization	0.09	[g/cell]																																														
	Cost of Rear Silver Paste	0.05	[$/cell]																																														
	Cost of Al Paste	16.50	[$/kg]																																														
	Al Paste utilization	1.40	[g/cell]																																														
	Cost of Al Paste	0.02	[$/cell]																																														
	Cost of Metal Paste at 100% yield	0.14	[$/cell]																																														
	Yield from this step on	0.970	[-]																																														
	Cost of Metal Paste	0.140	[$/cell]																																														
																																																	
	Screen Printing																																																
	Screen Prints per cell	4	[prints/cell]																																														
	Lifetime of Screen	8000	[prints]																																														
	Cost of Screen	70	[$]																																														
	Cost of Screen at 100% yield	0.035	[$/cell]																																														
	Yield from this step on	0.970	[-]																																														
	Cost of Screen	0.036	[$/cell]																																														
																																																	
	Module Materials																																																
		Cost [$/m]	At 100% Yield Cost [$/W]	Yield from Step	Cost [$/W]																																												
	Frame	1.2	0.024	0.990	0.024																																												
		Cost [$/m^2]	At 100% Yield Cost [$/W]		Cost [$/W]																																												
	Backsheet	4.75	0.030	0.990	0.030																																												
	Encapsulant	1.8	0.023	0.990	0.023																																												
	Glass	5.6	0.035	0.990	0.035																																												
		Cost [$/module]	At 100% Yield Cost [$/W]		Cost [$/W]																																												
	JB, Cable, Potting agent, and sticker	7.5	0.029	0.990	0.029																																												
	Ribbon	6.15	0.023	0.990	0.024																																												
																																																	
	Shipping Costs																																																
	Watts in container	156800	[W/container]																																														
	Shipping Costs	0	[$/container]																																														
	Shipping Cost	0.000	[$/W]																																														
																																																	
	Minimum Sustainable Price Calculations																																																
																																																	
	Minimum Sustainable Price																																																
	Shipment	2,000	[MW/yr]																																														
	MSP in Year 0	0.851	[$/W]																																														
	IRR	14.00%	[%]																																														
	Total Capex	1,475,478,466	[$]																																														
	Total NWC	314,978,365	[$]																																														
																																																	
	Ingot																																																
	Ingot Equipment Investment	314,115,308	[$]																																														
	Ingot Facility Investment	40,136,956	[$]																																														
																																																	
	Year	MSP [$/W]	Revenue [$]	Variable Cost [$/W]	Variable Cost [$]	Equipment MACRS Depreciation Factor	Equipment Depreciation [$]	Facility Depreciation Factor	Facility Depreciation [$]	Gross Profit [$]	Operating Expenses [$]	Operating Income [$]	Gain on Salvage [$]	NOL [$]	NOL Remaining [$]	NOL Used [$]	Tax [$]	NWC [$]	Change in NWC [$]	Capital Investment [$]	Salvage of Facility [$]	Salvage Book Value [$]	Incremental Cash Flow [$]																										
	0	0.237	0 	0.157	0 	0	0 	0 	0 	0 	0 	0 	0 	0	0	0	0 	90,886,111 	90,886,111 	(354,252,264)	0 	40,136,956	(445,138,375)																										
	1	0.237	473,694,286 	0.157	(313,806,545)	0.1429	(44,887,078)	0.01391	(558,305)	114,442,358 	(49,737,900)	64,704,458 	0 	0	0	0	(18,052,544)	90,886,111 	0 		0 	39,578,651	92,097,297 																										
	2	0.237	473,694,286 	0.157	(313,806,545)	0.2449	(76,926,839)	0.02564	(1,029,112)	81,931,790 	(49,737,900)	32,193,890 	0 	0	0	0	(8,982,095)	90,886,111 	0 		0 	38,549,539	101,167,745 																										
	3	0.237	473,694,286 	0.157	(313,806,545)	0.1749	(54,938,767)	0.02564	(1,029,112)	103,919,862 	(49,737,900)	54,181,962 	0 	0	0	0	(15,116,767)	90,886,111 	0 		0 	37,520,428	95,033,073 																										
	4	0.237	473,694,286 	0.157	(313,806,545)	0.1249	(39,233,002)	0.02564	(1,029,112)	119,625,627 	(49,737,900)	69,887,727 	0 	0	0	0	(19,498,676)	90,886,111 	0 		0 	36,491,316	90,651,165 																										
	5	0.237	473,694,286 	0.157	(313,806,545)	0.0893	(28,050,497)	0.02564	(1,029,112)	130,808,132 	(49,737,900)	81,070,232 	0 	0	0	0	(22,618,595)	90,886,111 	0 		0 	35,462,205	87,531,246 																										
	6	0.237	473,694,286 	0.157	(313,806,545)	0.0892	(28,019,085)	0.02564	(1,029,112)	130,839,544 	(49,737,900)	81,101,644 	0 	0	0	0	(22,627,359)	90,886,111 	0 		0 	34,433,093	87,522,482 																										
	7	0.237	473,694,286 	0.157	(313,806,545)	0.0893	(28,050,497)	0.02564	(1,029,112)	130,808,132 	(49,737,900)	81,070,232 	(4,505,373)	0	0	0	(21,361,596)	0 	(90,886,111)		28,898,608 	33,403,982	208,572,965 																										
	8	0.000	0 	0.000	0 	0.0446	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	9	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	10	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	11	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	12	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	13	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	14	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	15	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	16	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	17	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	18	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	19	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	20	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
																						NPV for Firm	0																										
																						IRR	14.00%																										
																																																	
	Wafer																																																
	Wafer Equipment Investment	176,883,571	[$]																																														
	Wafer Facility Investment	36,643,409	[$]																																														
																																																	
	Year	MSP [$/W]	Revenue [$]	Variable Cost [$/W]	Variable Cost [$]	Equipment MACRS Depreciation Factor	Equipment Depreciation [$]	Facility Depreciation Factor	Facility Depreciation [$]	Gross Profit [$]	Operating Expenses [$]	Operating Income [$]	Gain on Salvage [$]	NOL [$]	NOL Remaining [$]	NOL Used [$]	Tax [$]	NWC [$]	Change in NWC [$]	Capital Investment [$]	Salvage of Facility [$]	Salvage Book Value [$]	Incremental Cash Flow [$]																										
	0	0.111	0 	0.068	0 	0	0 	0 	0 	0 	0 	0 	0 	0	0	0	0 	39,643,192 	39,643,192 	(213,526,980)	0 	36,643,409	(253,170,172)																										
	1	0.111	221,411,518 	0.068	(135,324,560)	0.1429	(25,276,662)	0.01391	(509,710)	60,300,585 	(23,248,209)	37,052,376 	0 	0	0	0	(10,337,613)	39,643,192 	0 		0 	36,133,699	52,501,135 																										
	2	0.111	221,411,518 	0.068	(135,324,560)	0.2449	(43,318,786)	0.02564	(939,537)	41,828,634 	(23,248,209)	18,580,425 	0 	0	0	0	(5,183,938)	39,643,192 	0 		0 	35,194,162	57,654,810 																										
	3	0.111	221,411,518 	0.068	(135,324,560)	0.1749	(30,936,937)	0.02564	(939,537)	54,210,484 	(23,248,209)	30,962,275 	0 	0	0	0	(8,638,475)	39,643,192 	0 		0 	34,254,625	54,200,274 																										
	4	0.111	221,411,518 	0.068	(135,324,560)	0.1249	(22,092,758)	0.02564	(939,537)	63,054,663 	(23,248,209)	39,806,453 	0 	0	0	0	(11,106,000)	39,643,192 	0 		0 	33,315,088	51,732,748 																										
	5	0.111	221,411,518 	0.068	(135,324,560)	0.0893	(15,795,703)	0.02564	(939,537)	69,351,718 	(23,248,209)	46,103,508 	0 	0	0	0	(12,862,879)	39,643,192 	0 		0 	32,375,551	49,975,869 																										
	6	0.111	221,411,518 	0.068	(135,324,560)	0.0892	(15,778,015)	0.02564	(939,537)	69,369,406 	(23,248,209)	46,121,197 	0 	0	0	0	(12,867,814)	39,643,192 	0 		0 	31,436,014	49,970,934 																										
	7	0.111	221,411,518 	0.068	(135,324,560)	0.0893	(15,795,703)	0.02564	(939,537)	69,351,718 	(23,248,209)	46,103,508 	(4,113,223)	0	0	0	(11,715,290)	0 	(39,643,192)		26,383,255 	30,496,477	117,149,906 																										
	8	0.000	0 	0.000	0 	0.0446	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	9	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	10	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	11	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	12	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	13	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	14	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	15	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	16	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	17	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	18	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	19	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	20	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
																						NPV for Firm	0																										
																						IRR	14.00%																										
																																																	
	Cell																																																
	Cell Equipment Investment	551,992,553	[$]																																														
	Cell Facility Investment	91,071,050	[$]																																														
																																																	
	Year	MSP [$/W]	Revenue [$]	Variable Cost [$/W]	Variable Cost [$]	Equipment MACRS Depreciation Factor	Equipment Depreciation [$]	Facility Depreciation Factor	Facility Depreciation [$]	Gross Profit [$]	Operating Expenses [$]	Operating Income [$]	Gain on Salvage [$]	NOL [$]	NOL Remaining [$]	NOL Used [$]	Tax [$]	NWC [$]	Change in NWC [$]	Capital Investment [$]	Salvage of Facility [$]	Salvage Book Value [$]	Incremental Cash Flow [$]																										
	0	0.236	0 	0.121	0 	0	0 	0 	0 	0 	0 	0 	0 	0	0	0	0 	72,919,053 	72,919,053 	(643,063,603)	0 	91,071,050	(715,982,656)																										
	1	0.236	472,851,998 	0.121	(242,026,752)	0.1429	(78,879,736)	0.01391	(1,266,798)	150,678,712 	(49,649,460)	101,029,253 	0 	0	0	0	(28,187,161)	72,919,053 	0 		0 	89,804,252	152,988,625 																										
	2	0.236	472,851,998 	0.121	(242,026,752)	0.2449	(135,182,976)	0.02564	(2,335,062)	93,307,209 	(49,649,460)	43,657,749 	0 	0	0	0	(12,180,512)	72,919,053 	0 		0 	87,469,190	168,995,275 																										
	3	0.236	472,851,998 	0.121	(242,026,752)	0.1749	(96,543,497)	0.02564	(2,335,062)	131,946,687 	(49,649,460)	82,297,228 	0 	0	0	0	(22,960,926)	72,919,053 	0 		0 	85,134,128	158,214,860 																										
	4	0.236	472,851,998 	0.121	(242,026,752)	0.1249	(68,943,870)	0.02564	(2,335,062)	159,546,315 	(49,649,460)	109,896,855 	0 	0	0	0	(30,661,223)	72,919,053 	0 		0 	82,799,067	150,514,564 																										
	5	0.236	472,851,998 	0.121	(242,026,752)	0.0893	(49,292,935)	0.02564	(2,335,062)	179,197,250 	(49,649,460)	129,547,790 	0 	0	0	0	(36,143,833)	72,919,053 	0 		0 	80,464,005	145,031,953 																										
	6	0.236	472,851,998 	0.121	(242,026,752)	0.0892	(49,237,736)	0.02564	(2,335,062)	179,252,449 	(49,649,460)	129,602,989 	0 	0	0	0	(36,159,234)	72,919,053 	0 		0 	78,128,943	145,016,553 																										
	7	0.236	472,851,998 	0.121	(242,026,752)	0.0893	(49,292,935)	0.02564	(2,335,062)	179,197,250 	(49,649,460)	129,547,790 	(10,222,725)	0	0	0	(33,291,693)	0 	(72,919,053)		65,571,156 	75,793,882	286,374,303 																										
	8	0.000	0 	0.000	0 	0.0446	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	9	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	10	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	11	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	12	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	13	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	14	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	15	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	16	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	17	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	18	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	19	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	20	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
																						NPV for Firm	0																										
																						IRR	14.00%																										
																																																	
	Module																																																
	Module Equipment Investment	194,376,344	[$]																																														
	Module Facility Investment	70,259,274	[$]																																														
																																																	
	Year	MSP [$/W]	Revenue [$]	Variable Cost [$/W]	Variable Cost [$]	Equipment MACRS Depreciation Factor	Equipment Depreciation [$]	Facility Depreciation Factor	Facility Depreciation [$]	Gross Profit [$]	Operating Expenses [$]	Operating Income [$]	Gain on Salvage [$]	NOL [$]	NOL Remaining [$]	NOL Used [$]	Tax [$]	NWC [$]	Change in NWC [$]	Capital Investment [$]	Salvage of Facility [$]	Salvage Book Value [$]	Incremental Cash Flow [$]																										
	0	0.267	0 	0.195	0 	0	0 	0 	0 	0 	0 	0 	0 	0	0	0	0 	111,530,009 	111,530,009 	(264,635,619)	0 	70,259,274	(376,165,627)																										
	1	0.267	534,888,536 	0.195	(389,956,739)	0.1429	(27,776,380)	0.01391	(977,307)	116,178,111 	(56,163,296)	60,014,815 	0 	0	0	0	(16,744,133)	111,530,009 	0 		0 	69,281,968	72,024,368 																										
	2	0.267	534,888,536 	0.195	(389,956,739)	0.2449	(47,602,767)	0.02564	(1,801,448)	95,527,583 	(56,163,296)	39,364,286 	0 	0	0	0	(10,982,636)	111,530,009 	0 		0 	67,480,520	77,785,865 																										
	3	0.267	534,888,536 	0.195	(389,956,739)	0.1749	(33,996,423)	0.02564	(1,801,448)	109,133,927 	(56,163,296)	52,970,630 	0 	0	0	0	(14,778,806)	111,530,009 	0 		0 	65,679,072	73,989,695 																										
	4	0.267	534,888,536 	0.195	(389,956,739)	0.1249	(24,277,605)	0.02564	(1,801,448)	118,852,744 	(56,163,296)	62,689,448 	0 	0	0	0	(17,490,356)	111,530,009 	0 		0 	63,877,624	71,278,145 																										
	5	0.267	534,888,536 	0.195	(389,956,739)	0.0893	(17,357,808)	0.02564	(1,801,448)	125,772,542 	(56,163,296)	69,609,246 	0 	0	0	0	(19,420,980)	111,530,009 	0 		0 	62,076,176	69,347,521 																										
	6	0.267	534,888,536 	0.195	(389,956,739)	0.0892	(17,338,370)	0.02564	(1,801,448)	125,791,979 	(56,163,296)	69,628,683 	0 	0	0	0	(19,426,403)	111,530,009 	0 		0 	60,274,729	69,342,098 																										
	7	0.267	534,888,536 	0.195	(389,956,739)	0.0893	(17,357,808)	0.02564	(1,801,448)	125,772,542 	(56,163,296)	69,609,246 	(7,886,604)	0	0	0	(17,220,617)	0 	(111,530,009)		50,586,677 	58,473,281	233,664,570 																										
	8	0.000	0 	0.000	0 	0.0446	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	9	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	10	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	11	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	12	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	13	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	14	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	15	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	16	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	17	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	18	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	19	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
	20	0.000	0 	0.000	0 	0	0 	0.02564	0 	0 	0 	0 	0 	0	0	0	0 	0 	0 		0 	0	0 																										
																						NPV for Firm	0																										
																						IRR	14.00%																										
																																																	
																																																	
																																																	


Notes
"Notes by Tonio Buonassisi:
• To use this spreadsheet, alter one of the boxes in ""Top-Level Inputs."" Then, open the Solver and click ""Solve.""
• NB: You may first need to ""add"" Excel Solver before you can use it; instructions for Mac https://support.microsoft.com/en-us/kb/2431349 and PC https://support.office.com/en-us/article/load-the-solver-add-in-612926fc-d53b-46b4-872c-e24772f078ca
• The Solver uses a GRG Nonlinear solving method to solve for the minimum sustainable price (defined as when the rate of return equals the weighted average cost of capital). For more on the MSP methodology, see http://dx.doi.org/10.1109/JPHOTOV.2012.2230056. For more on the GRG Nonlinear solving method, see http://www.solver.com/excel-solver-grg-nonlinear-solving-method-stopping-conditions .
• Note the Solver solves the IRR = WACC condition for wafer, ingot, cell, and module simultaneously. Solving four constrained equations is not trivial for any algorithm, and certain initial conditions will cause the Solver to not converge. If you have problems with non-convergence, please re-open the original version of the spreadsheet, and try your inputs again.
• We welcome your feedback to improve this tool: buonassisi@mit.edu"


