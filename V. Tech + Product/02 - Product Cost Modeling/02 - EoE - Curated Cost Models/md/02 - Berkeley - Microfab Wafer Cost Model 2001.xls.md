Here's an example of a description that appears under a link.

15 MIN READ || Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Credit: [University of California, Berkeley](http://www.berkeley.edu/)

{! search-content: !}

Introduction

 			
			
	University of California at Berkeley		
	Competitive Semiconductor Manufacturing (CSM) Program		
			
	Spreadsheet Models for Fab Economic Analysis		
			
	Prepared by: Robert C. Leachman, Shengwei Ding and Nancy S. Sato-Misawa		
	Last Updated: December 19, 2001		
			
			
Introduction			
			
       This Excel workbook provides spreadsheet models for calculating revenues and costs of wafer fabrication.			
The intent is to provide the engineering analyst with the means to evaluate the economic impacts of 			
changes to process and equipment, changes in the timing of when process or equipment are installed and 			
qualified, changes in the time to ramp up die yield, and changes in manufacturing cycle time. Cash flows			
for both expenditures and revenues from fabrication are computed. 			
			
       At present, the models assume the fabrication line operates a single process technology consisting			
of up to 300 major process steps utilizing up to 50 major types of process equipment. The user may			
compute costs and revenues for one of two basic cases: (1) wafer start volumes are pre-specified over time, 			
or (2) equipment counts are pre-specified over time. In case (1), higher equipment efficiencies or reduced			
process times result in reduced investment in equipment and facilities to accommodate the pre-specified			
wafer starts. Higher yields in this case result in reduced investment costs as well as higher revenues for			
the given wafer start volumes. In case (2), higher equipment efficiencies or reduced process times result in			
higher wafer throughput for the given equipment set and hence both higher revenues and lower costs per			
wafer. Higher yields in this case result in higher die throughput for the given equipment set and both higher 			
revienues and lower costs per wafer.			
			
        The calculation of fab expenses uses an enhanced version of SEMATECH's Cost-Resource Model (CRM).			
This model accounts for expenses of fab construction and operation. In order to compute wafer and die costs,			
all wafers and die produced over the life of the technology are burdened equally with capital expenses.			
Important differences compared to CRM include (1) staffing costs are computed for varying levels of fab 			
automation, and (2) equipment performance is defined by the user in terms of theoretical throughput 			
rates and capability for equipment efficiency (CEE), rather than average throughput rates and equipment			
availability as is traditionally done using CRM.			
			
       The calculation of fab revenues accounts for a user-specified decline of die prices over time. Delays for			
fab construction, process development and qualification, equipment installation and qualification, yield ramp,			
and manufacturing cycle time depress revenues obtained from the process technology over its life. Our Delay			
Cost Model expresses a die cost equivalent to the foregone revenues resulting from delays for process			
development and qualification, equipment installation and qualification, factory construction, time to ramp die			
yield, and manufacturing cycle time.  			
			
        These models are explained in detail for the static wafer-starts case in the Competitive Semiconductor 			
Manufacturing (CSM) Program Report "Understanding Fab Economics", CSM-47, authored by Robert C. 			
Leachman, John Plummer and Nancy Sato-Misawa. This report may be ordered at			
	http://euler.berkeley.edu/esrc/csm/csmreports.html		
The important mathematical formulas also are displayed below.			
			
     This workbook is organized into seven spreadsheets to facilitate data input and visualization of results:  			
			
1.  The "Introduction" spreadsheet briefly explains these cost models, summarizes the required input data			
      and provides the formulae used in the calculations. 			
			
2. The "Input Data" spreadsheet includes shaded cells where the user defines the parameters in the cost models 			
     that can be modified to simulate different situations.   These input parameters include unit costs of equipment,			
     masks, staff and space; space consumption by equipment and staff; equipment efficiencies and lifetimes;			
     wafer start rates or tool counts; yields and yield ramp times; process lifetime; factory life; time until process 			
     qualification; total cycle time; initial revenue per die (at start of process development), and rate of revenue decline.			
  			
     The user must define additional more detailed input parameters for the Expense Model in the "Process Data" 			
     spreadsheet (discussed below). 			
			
3.  The "Process Data" spreadsheet contains the detailed process data.  Input parameters for each step of the 			
     process, including machine type, mask type (if any), theoretical wafer throughput for the step, direct and indirect 			
     material costs for the step, and actual step cycle times (or step batch size and handling time). These factors 			
     should be input in the appropriate shaded cell . The only allowable machine types and mask types are those 			
     appearing in the tables of machine types and mask types appearing on the "Input Data" spreadsheet. 			
     SEMATECH nomenclature for tool types and mask types is used. At present it is not possible to include more 			
     than 300 process steps or more than 50 tool types in the spreadsheet. It is possible to rename the tool types from 			
     the names given in the sample data. Renaming of a tool type is allowed in the "Tool Set" table (any name change 			
     in this list will be automatically updated in the "Expense Cost Calculation" and "Number of tools" spreadsheets). 			
     After modifying tool type names or other input data, be sure to press "control-n" to make the changes take effect.			
			
4.  The "Expense Cost Calculation" spreadsheet contains the model that calculates the fab expense per wafer.  This 			
     spreadsheet uses the data in the "Input Data" spreadsheet and process data in the '"Process" spreadsheet.			
     After modifying data in this spreadhseet, press "control-u" to update calculations of required numbers of tools.  			
     Cells shaded in 'blue' provide partial cost totals.			
			
5.  The "Total Cost" spreadsheet summarizes the results of cost and revenue calculations.   First it presents 			
     a table of cost components (fab expenses) for four possible levels of automation and for two calculation			
     assumptions (fractional and integer numbers of tools).  Below this table is shown the number of die			
     produced over the life of  the factory (TD). This is used to calculate the Expense Cost per die and the			
      Delay Cost per die which are shown next.  Finally, the Total Cost per die (the sum of these two costs) is shown.			
			
6.  The "Number of Tools" spreadsheet presents a table of the calculated number of tools per type, for the two			
     cases (fractional numbers of process tools and integer numbers of tools). It also shows the CEE and OEE factors.			
			
7.  The "Personnel Requirements" spreadsheet presents the caculated numbers of each personnel type, for each of 			
      the four alternative automation levels. One table corresponds to the case in which fractional tools are assumed 			
     and the other case corresponds to the assumption of integer tools.			
			
8.  The "Phased Capacity" spreadsheet presents the results for each of the capacity phases. The expense related 			
     cost table shows the expense in each phase. The revenue related cost table calculates the fab's real die output 			
     andrevenue over product life. And the tool requirement table shows the number of tools and OEE in each phase.			
			
			
			
Automation Levels			
			
     We classify automation into two major types, material handling automation (MHA) and information handling 			
automation (IHA).  Possible combinations of information and material handling automation are indicated 			
as an ordered pair (MHA,IHA) with values as defined below.			
			
     Material handling automation refers to wafer and reticle movement, both within processing bays, as well as			
 between bays. The four possible levels of MHA are as follows.			
			
 MHA Level	Description		
0	None		
1	Interbay rail system only		
1.5	Interbay system plus AGVs in photolithography and diffusion areas		
2	Interbay system plus AGVs in all areas		
			
     Information handling automation involves automation of the download of processing instructions and upload 			
results to/from processing equipment. The four levels of IHA evaluated here are as follows.			
			
IHA Level	Description		
0	None		
1	100%  auto recipe download		
1.5	100%  auto recipe download and 100% auto metrology upload		
2	100%  auto recipe download, 100% auto metrology upload, 		
	100% auto track-in/track-out, 100% auto lot and machine selection		
			
Fab expenses are automatically computed for the automation levels (0, 0), (1, 1), (1.5, 1.5) and (2, 2).			
At present, capital and maintenance expenses for automation are excluded from cost calculations.			
			
	
			
Summary of Sample Input Data			
			
     The default values for the input variables considered in the calculation of fab expenses were taken from 			
SEMATECH's CRM dataset for a 0.25um logic process as well as from data collected by the CSM program.			
These default values are summarized below.			
			
Fab Expense Parameters			
			
General Variable	Default value		
Line Yield (LY)	0.98		
Wafer starts per month (W)	25000		
Blank wafer cost ($)	200		
			
			
Mask Type	Purchase Cost ($/unit)	Life (wafer passes)	
248_Mask_8	25,000	40,000	
248C_Mask_8	80,000	40,000	
Iw_Mask_8	4,000	40,000	
I_Mask_8	7,000	40,000	
			
			
Personnel	Annual Salary ($)		
Operator	60,000		
Supervisor	80,000		
Manager	125,000		
Overhead	70,000		
Engineer	125,000		
Technicians	70,000		
			
			
Factory Space	Default Value		
Life expectancy (years)	25		
Construction cost ($ per sq. ft.)			
Cleanroom	3500		
Non-cleanroom	175		
Non-manufacturing	175		
Annual occupancy cost ($ per sq. ft.)			
Cleanroom	175		
Non-cleanroom	50		
Non-manufacturing	50		
Space/person (sq.ft.)	150		
Space/tool (sq.ft.)	various (see "Input Data" spreadsheet)		
			
			
Tool Set	Default value		
CEE	various (see "Input Data" spreadsheet)		Note: CEE (capability for equipment
Purchase ($mm)	various (see "Input Data" spreadsheet)		efficiency) is the OEE of the
Additional tools ($mm)	various (see "Input Data" spreadsheet)		equipment if it is the bottleneck.
Installation ($mm)	various (see "Input Data" spreadsheet)		The OEE will be less when some
Maintenance ($mm/year)	various (see "Input Data" spreadsheet)		other equipment is the bottleneck
			or due to rounding to integer tools.
Process Data	Default values		
Step number	Default process is the "250_Al_82" process flow		
Process description	created by SEMATECH. This is a 19 mask, 5 metal		
Tool type	process for logic devices with 250nm design rule 		
Mask type	fabricated on 8-inch wafers. User may enter a different 		
Wafers/hour	process that uses the same or fewer steps and tool types.		
Indirect material ($ per wafer pass)			
Direct material ($ per wafer pass)			
			
			
Delay-Related Cost Parameters			
			
Description	Input Variable	Default value	
Mature Yield	YF	0.95	
Initial Yield	Y0	0.5	
Factory Life (days)	H	1800	
Yield ramp time (days)	RT	120	
Yield learning rate *		0.67	
Initial Revenue	R0	10000	
discount factor per year**		0.25	
duration until process is qualified			
and salable wafer starts begin (days)	VT	210	
total manufacturing cycle time	CT TOTAL	30	
			
* NOTE:  The yield learning rate is the fraction of the total yield improvement completed halfway through the ramp. 			
                  For example, 0.67 means that 2/3 of the yield improvement is completed in time 0.5 RT.			
			
**NOTE: The discount factor per year indicates how fast the revenue per wafer is decreasing.  For example, 			
                  if R0=10,000 and the discount factor is 0.25, then the revenue per wafer after one year is 7,500.			
			

			
			
			
Cost Model Formulae			
			
Cost model formulas			
			
Number of process tools			
			
In option 2 (fixed equipment set), the number of process tools of type i, Ni, is pre-specified. In option 1 (fixed wafer			
 starts), Ni is computed from the given wafer starts as follows:			

where W is the given wafer starts per month, LY is the line yield of the process flow, jei denotes that process step j			
   is performed using equipment type i, UPHj is the theoretical wafers-per-hour processing rate for step j, and CEEi is			
   the capability for equipment efficiency of tool type i. In the case that the integer tools options is specified, 			
   the expression for Ni is rounded up to an integer.			
			
			
When time-varying wafer starts and equipment efficiencies are specified by phase under option 1, Ni is computed 			
 each phase. However, the number of process tools of each type is not allowed to decline in subsequent for phases.			
			
Number of wafer starts			
			
In option 1, the number of wafer starts per 30-day month is pre-specified by the user for each phase. In option 2, 			
   the number of wafer starts is calculated from the pre-specified numbers of tools as follows:			
			
			
where ThPTj is the theoretical process time per wafer for step j (i.e., the reciprocal of UPHj).			
			
Fab expense			
			
Fab expenses are calculated in terms of four basic expense pools: process tools, staff, factory space, and materials.			
 Staffing requirements are assumed to be linear functions of the number of wafer starts and the numbers of process			
 tools, added to a certain minimum fixed staff. Space requirements also are assumed to be a linear function of the			
 numbers of the process tools and the number of wafer starts, added to a certain minimum fixed space requirement.			
 Materials consumption at each process step is assumed to be proportional to wafer throughput of that step. These			
 linear functions are stored as coefficients in the spreadsheets. Capital expenses for process tools and factory 			
 space are annualized uniformly over pre-specified lifetimes.			
			
The total fab expense per year is calculated as			
			
where Cei denotes the annualized installation and purchase cost of tool type i, Lei denotes the portion of annual			
 labor cost that is proportional to the number of tools of type i (per tool), Sei denotes the annualized cost of factory			
 space per tool of type i, Ni denotes the number of tools of type i, Lw denotes the portion of total labor cost that is			
 proportional to wafer starts (per wafer start), Mw denotes the total materials and mask costs per wafer start, Sw			
 denotes the factory space cost per wafer start, Lf denotes the portion of total labor cost that is fixed, and Sf			
 denotes the portion of total space cost that is fixed. In the case that wafer starts are held constant at rate W per			
 month, the fab expense per wafer, EPW, is calculated by dividing EPY by 12W.			
			
 The total die output over the process life in the case of constant wafer starts is calculated as			

where Y0 is the die yield times line yield at the time of process qualification, YF is the mature die yield times line			
 yield, H is the process lifetime, RT is the duration from process qualification until mature die yield is attained,			
 and b is the yield learning rate.  The fab expense per die is calculated as the total fab expense over the process			
 life divided by the total die output.			
			
Revenues and delay costs			
			
The ideal revenue realized over the process life is calculated in the case of constant wafer starts as			
	
where R0 is the initial selling price for a 100%-yielding wafer, and a is the rate of sales price decline. Considering			
 the delays for process qualification, yield ramp and manufacturing cycle, the total revenue actually realized over			
 the process life is			
					
where VT is the duration until salable wafer starts commence and CT is the manufacturing cycle time.			
			
The total delay cost is computed as			
			
				
Extension to time-varying wafer starts			
			
The input formats allow the user to specify up to eight phases of process life. Either the wafer starts rate in each			
 phase is pre-specified (option 1), or the wafer starts rate is calculated from the pre-specified number of tools in			
 each phase (option 2). To illustrate, suppose the process life is divided into n phases spanning the intervals			
 [ti-1, ti], i=1, 2, …, n, and suppose the wafer starts rate in phase i is aiW, where an = 1.			
			
The expense per wafer is calculated as			

  For the phases before RT, the die output is calculated as			
			
 the actually realized revenue is calculated as			
			
 for the phases after RT, the die output is calculated as			
			
 the actually realized revenue is calculated as			
			
 The summation of the actually realized revenue for all the phases is the total realized revenue. Thus the total delay			
 cost is calculated as the total realized revenue subtracted from the ideal revenue .			
		
Queueing model for calculation of step cycle times			
			
 For multi-machine, general inter-arrival distribution and general service time distribution, an easy estimation			
 of cycle time for each equipment in each step can be done by Heavy-traffic approximation. The formula is			
         s = (# wafers in one load) / (tool UPH)			
			
         c is number of machines			
			
 For semiconductor equipment with production scheduling, the varances are quite small and the following values			
 are used:			

			
To the value of CT derived using the above formulae, we add the handling time specified by the user to determine			
the total step cycle time.			
			
(This approach is applied only in the case the user does not specify actual step cycle times.)			



Input Data

Input data 																																																															
																																																															
								Tool Costs and Space Requirements																																																							
Fab Expense Inputs																																																															
								DO NOT SORT THIS TABLE.																																																							
Please change data only in the cells shaded this color.								Tool Set	Cost per unit of equipment																																																						
									purchase 	add'l tools	install	maintce		Space consumed per tool																																																	
								Tool Type	$mm	$mm	$mm	$mm/yr	tool life	Cleanroom(sq.ft.)	non-cleanroom(sq.ft.)																																																
								CMP_Ins	2	0.4	0.3	0.14	5	400	1600																																																
								CMP_Ins(C) 	2	0.4	0.3	0.14	5	400	1600																																																
								CMP_Ins(I)	2	0.4	0.3	0.14	5	400	1600																																																
								CMP_Met	2	0.4	0.3	0.14	5	400	1600																																																
Blank wafer cost ($)	200							CVD_Ins	3	0.6	0.45	0.21	5	400	1600																																																
								CVD_Ins(C) 	3	0.6	0.45	0.21	5	400	1600																																																
DO NOT SORT THIS TABLE								CVD_Ins(I)	3	0.6	0.45	0.21	5	400	1600																																																
Mask Type	Purch cost ($/unit)	Life Exp(wafers)						CVD_Ins_Thin	2	0.4	0.3	0.14	5	400	1600																																																
248_Mask	25000	40000						CVD_Met	3.5	0.7	0.525	0.245	5	400	1600																																																
248C_Mask	80000	40000						CVD_Met(C) 	3.5	0.7	0.525	0.245	5	400	1600																																																
Iw_Mask	4000	40000						CVD_MetW	3.5	0.7	0.525	0.245	5	400	1600																																																
I_Mask	7000	40000						CVD_MetW(C) 	3.5	0.7	0.525	0.245	5	400	1600																																																
								Dry_Etch	2.5	0.5	0.375	0.175	5	400	1600																																																
								Dry_Etch(A)	2.5	0.5	0.375	0.175	5	400	1600																																																
Personnel	Annual Salary							Dry_Etch(C) 	2.5	0.5	0.375	0.175	5	400	1600																																																
Operator	60000							Dry_Etch(I)	2.5	0.5	0.375	0.175	5	400	1600																																																
Supervisor	80000							Dry_Etch_Met	2.5	0.5	0.375	0.175	5	400	1600																																																
Manager	125000							Dry_Strip	1	0.2	0.15	0.07	5	280	1120																																																
Overhead staff	70000							Dry_Strip(D)	1	0.2	0.15	0.07	5	280	1120																																																
Engineer	125000							Dry_Strip(I)	1	0.2	0.15	0.07	5	280	1120																																																
Technicians	70000							Furn_FastRmp	1	0.2	0.15	0.07	5	240	960																																																
								Furn_Nitr	1	0.2	0.15	0.07	5	240	960																																																
								Furn_OxAn	1	0.2	0.15	0.07	5	240	960																																																
Space Costs	Life (years)	Construction ($)	Occupancy cost ($/yr)	space/person (sq.ft.)				Furn_OxAn(I)	1	0.2	0.15	0.07	5	240	960																																																
Direct								Furn_Poly	1	0.2	0.15	0.07	5	240	960																																																
Cleanroom	25	3500	175					Furn_TEOS	1	0.2	0.15	0.07	5	240	960																																																
Non-cleanroom	25	175	50					Implant_HiE	3	0.6	0.45	0.21	5	1400	5600																																																
Indirect								Implant_LoE	3	0.6	0.45	0.21	5	800	3200																																																
Non-manufacturing	25	175	50	150				Insp_PLY	3	0.6	0.45	0.21	5	120	480																																																
								Insp_Visual	0.5	0.1	0.075	0.035	5	120	480																																																
								Litho_248	9	1.8	1.35	0.63	5	500	2000																																																
								Litho_I	6	1.2	0.9	0.42	5	400	1600																																																
Delay Cost Inputs								Litho_Iw	5	1	0.75	0.35	5	400	1600																																																
								Meas_CD	1.5	0.3	0.225	0.105	5	120	480																																																
								Meas_Film	0.7	0.14	0.105	0.049	5	120	480																																																
Description	Input Variable	Value						Meas_Overlay	1	0.2	0.15	0.07	5	120	480																																																
Line Yield (LY)	LY	0.98						PVD_Met	4	0.8	0.6	0.28	5	500	2000																																																
Mature Yield	YF	0.95						PVD_Met(C) 	4	0.8	0.6	0.28	5	500	2000																																																
Initial Yield	Y0	0.5						RTP_OxAn(C) 	1.5	0.3	0.225	0.105	5	400	1600																																																
Factory Life (days)	H	1800						Test	1	0.2	0.15	0.07	5	120	480																																																
Ramp time (days)	RT	120						VP_HF_Clean	0.8	0.16	0.12	0.056	5	320	1280																																																
Yield learning rate *		0.67						Wet_Bench	2	0.4	0.3	0.14	5	500	2000																																																
Initial Revenue #	R0	10000		# NOTE: Initial revenue applies at start of process development 				Wet_Bench(I)	2	0.4	0.3	0.14	5	500	2000																																																
discount factor per year**		0.25		and qualification.																																																											
process dev & qual (days)***	VT	120																																																													
manufacturing cycle time	CT TOTAL																																																														
Derived Variables																																																															
manufacturing cycle time ##	CT	26.84639237		## NOTE:  For Cycle Time Calculation, there are 3 possible sources:																																																											
Wafer starts per month (W)	WS	25000			1. If the cell "CT TOTAL" has a value, that value will be used as CT. Step cycle times in the "Process Data" sheet will be automatically scaled to match CT.																																																										
designed die output capacity (per monthly period) at mature die yield, expressed in units of equivalent 100%-yielding wafers.	D 	23750			2. If the cell "CT TOTAL" is left blank, the sum of "Actual CT" and handling time for all steps in sheet "Process Data" will be taken to be the value of CT.																																																										
learning curve factor	b	0.018310205			    WARNING: If some values of "Actual CT" are filled in but others are left blank, the steps with blank cells will be assumed to have 0 cycle time.																																																										
discount factor per day	a 	0.000799117			3. If both "CT TOTAL" and "Actual CT" are left blank, then step cycle time will be calculated from equipment CEE and numbers of tools, then summed 																																																										
					    with handling time for all steps to compute CT.																																																										
																																																															
* NOTE:  The yield learning rate is the fraction of the total yield improvement completed halfway through the yield ramp. 																																																															
                   For example, 0.67 means that 2/3 of the yield improvement is completed at time 0.5 RT.																																																															
																																																															
**NOTE: The discount factor per year indicates how fast the revenue per wafer is decreasing.  																																																															
                   For example, if R0=10,000 and the discount factor is 0.25, then the revenue per wafer one year after start of process development is 7,500.																																																															
																																																															
***NOTE: VT is the time when wafers that will be sold are first started, accounting for all delays for process development																																																															
                   and qualification, factory construction, equipment installation and qualification.																																																															
																																																															
																																																															
																																																															
Wafer start rates (wafers per month)																																																															
				Fixed wafer starts case only			Tool CEE and Tool Quantities by Phase of Wafer Starts																																																								
																		Tool quantities		Fixed eqpt counts case only																																											
		Phase No.	Start time	Wafer start rate				DO NOT RESORT THIS TABLE. ALSO, PHASES MUST MATCH THOSE IN THE TABLE AT LEFT.																																																							
		1	0	15000				   Phase Number   	1	2	3	4	5	6	7	8		1	2	3	4	5	6	7	8																																						
		2	120	25000				Tool Type	CEE	CEE	CEE	CEE	CEE	CEE	CEE	CEE	Tool Type	Quantity	Quantity	Quantity	Quantity	Quantity	Quantity	Quantity	Quantity																																						
		3						CMP_Ins	0.23								CMP_Ins	1	2	3	3																																										
		4						CMP_Ins(C) 	0.23								CMP_Ins(C) 	5	10	15	20																																										
		5						CMP_Ins(I)	0.23								CMP_Ins(I)	1	2	3	3																																										
		6						CMP_Met	0.23								CMP_Met	4	7	10	13																																										
		7						CVD_Ins	0.64								CVD_Ins	1	2	3	4																																										
		8						CVD_Ins(C) 	0.64								CVD_Ins(C) 	3	5	8	10																																										
								CVD_Ins(I)	0.64								CVD_Ins(I)	1	2	3	3																																										
								CVD_Ins_Thin	0.64								CVD_Ins_Thin	1	1	2	2																																										
		NOTE: Time 0 in this table is right after process qualification, i.e., after the duration 'VT'.						CVD_Met	0.48								CVD_Met	1	1	2	2																																										
		                A Phase is a time interval with either a fixed wafer start rate or a fixed equipment set.						CVD_Met(C) 	0.48								CVD_Met(C) 	2	3	4	5																																										
		                Time before and after RT must be placed in different phases.						CVD_MetW	0.48								CVD_MetW	1	1	2	2																																										
		                The last phase is automatically assumed to end at the process life time H.						CVD_MetW(C) 	0.48								CVD_MetW(C) 	2	3	4	5																																										
								Dry_Etch	0.59								Dry_Etch	1	2	3	3																																										
		BE SURE TO INCLUDE "RT" IN THE START TIMES.						Dry_Etch(A)	0.53								Dry_Etch(A)	1	2	3	3																																										
								Dry_Etch(C) 	0.53								Dry_Etch(C) 	4	7	11	14																																										
								Dry_Etch(I)	0.53								Dry_Etch(I)	2	4	6	7																																										
Calculation Type								Dry_Etch_Met	0.59								Dry_Etch_Met	3	5	8	10																																										
								Dry_Strip	0.65								Dry_Strip	1	1	2	2																																										
	Fixed wafer starts, variable eqpt counts:				Click to Run			Dry_Strip(D)	0.65								Dry_Strip(D)	1	1	2	2																																										
	TO DO:							Dry_Strip(I)	0.65								Dry_Strip(I)	2	3	5	6																																										
	Fill in Start times and Wafer start rates above							Furn_FastRmp	0.5								Furn_FastRmp	3	5	7	9																																										
	Fill in CEEs in each phase							Furn_Nitr	0.5								Furn_Nitr	1	2	3	3																																										
	in table at immediate right							Furn_OxAn	0.5								Furn_OxAn	4	7	11	14																																										
								Furn_OxAn(I)	0.5								Furn_OxAn(I)	1	2	3	4																																										
								Furn_Poly	0.5								Furn_Poly	1	2	3	3																																										
								Furn_TEOS	0.5								Furn_TEOS	1	2	3	3																																										
								Implant_HiE	0.37								Implant_HiE	1	1	2	2																																										
								Implant_LoE	0.42								Implant_LoE	1	2	3	4																																										
	Fixed eqpt counts, unlimited market:				Click to Run			Insp_PLY	0.3								Insp_PLY	7	13	19	25																																										
	TO DO:							Insp_Visual	0.35								Insp_Visual	1	1	1	1																																										
	Fill in Start times above (Wafer start rates will be overwritten by calculation)							Litho_248	0.8								Litho_248	1	2	3	4																																										
	Fill in CEEs and tool quantities in each pahse							Litho_I	0.8								Litho_I	3	6	9	11																																										
	in table at immediate right							Litho_Iw	0.8								Litho_Iw	3	6	9	11																																										
								Meas_CD	0.35								Meas_CD	4	8	12	15																																										
								Meas_Film	0.35								Meas_Film	3	6	9	12																																										
								Meas_Overlay	0.3								Meas_Overlay	3	6	9	11																																										
								PVD_Met	0.51								PVD_Met	1	1	2	2																																										
								PVD_Met(C) 	0.51								PVD_Met(C) 	3	5	7	9																																										
								RTP_OxAn(C) 	0.57								RTP_OxAn(C) 	1	2	3	3																																										
								Test	0.39								Test	6	11	17	22																																										
								VP_HF_Clean	0.45								VP_HF_Clean	2	3	4	5																																										
								Wet_Bench	0.54								Wet_Bench	3	6	9	11																																										
								Wet_Bench(I)	0.54								Wet_Bench(I)	3	5	8	10																																										
																																																															
																																																															
																																																															

Process Data

Input data 	Macros:	To sort by step: ctrl-f					step number	Process description	Tool_type	Mask type	wafers/hour	Indirect Material ($/pass)	Direct material ($/pass)	Actual CT (hours)	Mask cost/pass	Mask cost/mo	Indirect material/mo	Direct material/mo	1-CEE	#tools	Twafer																																																									
partial cost total		To sort by Tool Name: ctrl-r					118	CMP_BPSG	CMP_Ins		60	2.0		1.98162037		0.00	49584.12	0.00	0.77	2.50	0.02					Tool_type	Batch Size	Handling Time (mins)	tool type	Availability	OEE	#steps	#tool	#fraction	SVT	VAR	Tsvc	Ce2	utilization	CTq	CT Data	CT Calculated																																				
							151	CMP_Oxide	CMP_Ins(C) 		30	2.0		1.98162037		0.00	49467.45	0.00	0.77	4.98	0.03					CMP_Ins	25	5	0	0.742	0.191296765	1	2.495175191	3	0.016666667	#DIV/0!	0.561545373	0.19188928	0.210426441	0.432212189	1.98162037	1.193048604																																				
             Please change input data only in the cells shaded this color.							184	CMP_Oxide	CMP_Ins(C) 		30	2.0		1.98162037		0.00	49351.05	0.00	0.77	4.97	0.03					CMP_Ins(C) 	25	5	0	0.742	0.228217033	4	19.84495943	20	0.033333333	0	1.123090746	0.14594464	0.251038737	0.833461358	1.98162037	2.300629032																																				
							217	CMP_Oxide	CMP_Ins(C) 		30	2.0		1.98162037		0.00	49234.93	0.00	0.77	4.96	0.03					CMP_Ins(I)	25	5	0	0.742	0.192626016	1	2.512513249	3	0.016666667	#DIV/0!	0.561545373	0.19188928	0.211888617	0.432453689	1.98162037	1.193715224																																				
Notes:  Make sure that step numbers are distinct consecutive integer numbers. In column J, only use the exact 							248	CMP_Oxide	CMP_Ins(C) 		30	2.0		1.98162037		0.00	49126.09	0.00	0.77	4.94	0.03					CMP_Met	25	5	0	0.742	0.21947751	5	12.40525056	13	0.016666667	5.42101E-20	0.561545373	0.19188928	0.241425261	0.416974953	1.98162037	1.150988795																																				
             tool and mask names appearing in the "Input Data" spreadsheet. (For convenience, these are listed at lower left.)							21	CMP_AA	CMP_Ins(I)		60	2.0		1.98162037		0.00	49928.66	0.00	0.77	2.51	0.02					CVD_Ins	25	5	0	0.875	0.559613727	3	3.497585797	4	0.021666667	8.33333E-06	0.619047619	0.158136095	0.6155751	0.682969823	3.204055556	1.88522262																																				
             The reciprocal of theoretical process time for each step is entered in column L (Wafers/hour).							132	CMP_W	CMP_Met		60	2.0		1.98162037		0.00	49534.59	0.00	0.77	2.49	0.02					CVD_Ins(C) 	25	5	0	0.875	0.592720695	5	9.261260862	10	0.034666667	8.88889E-06	0.99047619	0.132636834	0.651992765	0.940983438	3.204055556	2.597425539																																				
							165	CMP_W	CMP_Met		60	2.0		1.98162037		0.00	49418.03	0.00	0.77	2.49	0.02					CVD_Ins(I)	25	5	0	0.875	0.346801092	1	1.083753414	2	0.02	#DIV/0!	0.571428571	0.14375	0.381481202	0.586965253	3.204055556	1.620218249																																				
             There are two options for step cycle time data. One option is to enter actual cycle times in column O, including							198	CMP_W	CMP_Met		60	2.0		1.98162037		0.00	49301.75	0.00	0.77	2.48	0.02					CVD_Ins_Thin	25	5	0	0.875	0.514661912	3	1.608318476	2	0.01	2.71051E-20	0.285714286	0.1875	0.566128103	0.377834002	3.204055556	1.042946823																																				
             all waiting, process and material handling times. The other option is to enter step batch size in column P and step							231	CMP_W	CMP_Met		60	2.0		1.98162037		0.00	49185.74	0.00	0.77	2.48	0.02					CVD_Met	25	5	0	0.875	0.28669944	1	1.194581001	2	0.016666667	#DIV/0!	0.476190476	0.1525	0.315369384	0.465539894	3.204055556	1.285044094																																				
             handling time in column Q, and let the system calculate step cycle times.							262	CMP_W	CMP_Met		60	2.0		1.98162037		0.00	49077.02	0.00	0.77	2.47	0.02					CVD_Met(C) 	25	5	0	0.875	0.456043229	4	4.750450304	5	0.016666667	0	0.476190476	0.1525	0.501647552	0.449322494	3.204055556	1.240278705																																				
             If data for Actual CT is entered, it must be entered for every step. If some are left blank, they will be assumed							113	CVD_Nitr/TEOS	CVD_Ins		50	1.5		3.204055556		0.00	37201.37	0.00	0.36	1.08	0.02					CVD_MetW	25	5	0	0.875	0.245724835	1	1.023853479	2	0.014285714	#DIV/0!	0.408163265	0.16125	0.270297318	0.388380983	3.204055556	1.072059978																																				
             to be zero. If Actual CT is left blank for ALL steps, then CT will be calculated automatically for all steps based on							115	CVD_BPSG	CVD_Ins		40	1.5		3.204055556		0.00	37196.06	0.00	0.36	1.35	0.03					CVD_MetW(C) 	25	5	0	0.875	0.390866292	4	4.071523879	5	0.014285714	0	0.408163265	0.16125	0.429952922	0.373322601	3.204055556	1.030493864																																				
            queuing analysis of equipment counts and CEE factors and the user input data from columns P and Q. If the total							121	APCVD_Ox	CVD_Ins		50	1.5		3.204055556		0.00	37180.13	0.00	0.36	1.08	0.02					Dry_Etch	25	5	0	0.85	0.46269864	1	2.352704948	3	0.04	#DIV/0!	1.176470588	0.1255	0.508968504	1.215356413	4.683229167	3.354785705																																				
            of step cycle times is different from the "CT TOTAL" entry on the "Input Data" page, then step cycle times will 							148	CVD_ILD	CVD_Ins(C) 		30	1.5		3.204055556		0.00	37108.53	0.00	0.36	1.79	0.03					Dry_Etch(A)	25	5	0	0.85	0.45885011	1	2.597264776	3	0.04	#DIV/0!	1.176470588	0.1255	0.504735122	1.209492024	4.683229167	3.338598052																																				
            be automatically re-scaled to be consistent with "CT TOTAL". If "CT TOTAL" is left blank, no re-scaling is performed.							181	CVD_ILD	CVD_Ins(C) 		30	1.5		3.204055556		0.00	37021.22	0.00	0.36	1.79	0.03					Dry_Etch(C) 	25	5	0	0.85	0.509141857	8	13.44903018	14	0.026041667	6.82044E-05	0.765931373	0.239739429	0.560056042	0.666396675	4.683229167	1.839475249																																				
							214	CVD_ILD	CVD_Ins(C) 		30	1.5		3.204055556		0.00	36934.10	0.00	0.36	1.78	0.03					Dry_Etch(I)	25	5	0	0.85	0.526184222	3	6.949602933	7	0.035555556	1.48148E-05	1.045751634	0.14040625	0.578802644	0.973189034	3.64147539	2.686323637																																				
							245	CVD_ILD	CVD_Ins(C) 		30	1.5		3.204055556		0.00	36852.46	0.00	0.36	1.78	0.03					Dry_Etch_Met	25	5	0	0.85	0.57030747	5	9.666228304	10	0.033333333	2.1684E-19	0.980392157	0.1306	0.627338217	0.902297392	4.189074074	2.490639257																																				
							276	CVD_TEOS/Nitride	CVD_Ins(C) 		25	1.5		3.204055556		0.00	36770.99	0.00	0.36	2.13	0.04					Dry_Strip	25	5	0	0.85	0.577795546	1	1.77783245	2	0.033333333	#DIV/0!	0.980392157	0.1306	0.635575101	1.554094662	1.557967836	4.289815318																																				
Process ID :250_Al_82							18	Oxide_STI	CVD_Ins(I)		50	1.5		3.204055556		0.00	37454.52	0.00	0.36	1.08	0.02					Dry_Strip(D)	25	5	0	0.85	0.643213659	3	1.979118952	2	0.0125	0	0.367647059	0.1816	0.707535025	0.809172525	1.557967836	2.233583821																																				
							135	CVD_Oxide	CVD_Ins_Thin		100	1.0		3.204055556		0.00	24761.99	0.00	0.36	0.54	0.01					Dry_Strip(I)	25	5	0	0.85	0.576257152	8	5.31929679	6	0.0125	6.19544E-20	0.367647059	0.1816	0.633882867	0.376199458	1.557967836	1.038434939																																				
							168	CVD_Oxide	CVD_Ins_Thin		100	1.0		3.204055556		0.00	24703.73	0.00	0.36	0.54	0.01					Furn_FastRmp	150	5	0	0.893	0.462044474	6	8.316800541	9	0.02	0	3.359462486	0.106370067	0.508248922	3.067713813	10.41560185	8.467904835																																				
Number of process steps (J)	283						201	CVD_Oxide	CVD_Ins_Thin		100	1.0		3.204055556		0.00	24645.60	0.00	0.36	0.53	0.01					Furn_Nitr	150	5	0	0.893	0.385719853	1	2.31431912	3	0.033333333	#DIV/0!	5.599104143	0.10382204	0.424291839	5.50337521	14.27951389	15.19113594																																				
							130	CVD_Ti/TiN	CVD_Met		60	2.0		3.204055556		0.00	49541.66	0.00	0.52	1.19	0.02					Furn_OxAn	25	5	0	0.893	0.467716616	7	13.09606526	14	0.027346939	1.04956E-05	0.765591791	0.141986539	0.514488278	0.68991203	3.174791667	1.904385406																																				
Total material a month		3.89	0.00	0.00			163	CVD_Ti/TiN	CVD_Met(C) 		60	2.0		3.204055556		0.00	49425.09	0.00	0.52	1.19	0.02					Furn_OxAn(I)	25	5	0	0.893	0.492767152	2	3.942137217	4	0.028571429	0	0.79987202	0.12675428	0.542043867	0.811681407	3.174791667	2.240509165																																				
							196	CVD_Ti/TiN	CVD_Met(C) 		60	2.0		3.204055556		0.00	49308.79	0.00	0.52	1.19	0.02					Furn_Poly	150	5	0	0.893	0.384482738	1	2.306896427	3	0.033333333	#DIV/0!	5.599104143	0.10382204	0.422931012	5.498978478	3.174791667	15.1789995																																				
Material Cost per Wafer		Indirect 	Direct	Mask	Wafer		229	CVD_Ti/TiN	CVD_Met(C) 		60	2.0		3.204055556		0.00	49192.77	0.00	0.52	1.19	0.02					Furn_TEOS	150	5	0	0.893	0.383632812	1	2.30179687	3	0.033333333	#DIV/0!	5.599104143	0.10382204	0.421996093	5.495977073	3.174791667	15.17071463																																				
							260	CVD_Ti/TiN	CVD_Met(C) 		60	2.0		3.204055556		0.00	49084.02	0.00	0.52	1.18	0.02					Implant_HiE	150	5	0	0.8	0.346355765	4	1.872193324	2	0.005	0	0.9375	0.142666667	0.380991341	0.924465134	2.942098765	2.551829555																																				
	$/wafer	0.000158891	0	0	200		131	CVD_W	CVD_MetW		70	2.0		3.204055556		0.00	49538.13	0.00	0.52	1.02	0.01					Implant_LoE	150	5	0	0.895	0.34556182	6	3.291064951	4	0.006666667	1.0842E-20	1.117318436	0.118795	0.380118002	1.042637508	2.942098765	2.878024398																																				
							164	CVD_W	CVD_MetW(C) 		70	2.0		3.204055556		0.00	49421.56	0.00	0.52	1.02	0.01					Insp_PLY	25	5	0	0.95	0.295143567	43	24.59529728	25	0.005	0	0.131578947	0.176	0.324657924	0.12500597	0.903689236	0.345057827																																				
	$/wafer	0.000158891	200				197	CVD_W	CVD_MetW(C) 		70	2.0		3.204055556		0.00	49305.27	0.00	0.52	1.02	0.01					Insp_Visual	25	5	0	0.95	0.345196189	2	0.986274826	1	0.005	0	0.131578947	0.176	0.379715808	0.176514689	0.695802469	0.487238926																																				
							230	CVD_W	CVD_MetW(C) 		70	2.0		3.204055556		0.00	49189.26	0.00	0.52	1.02	0.01					Litho_248	25	45	1	0.9	0.690220928	2	3.45110464	4	0.04	0	1.111111111	0.118	0.759243021	4.350272782	11.08736111	12.00819182																																				
							261	CVD_W	CVD_MetW(C) 		70	2.0		3.204055556		0.00	49080.52	0.00	0.52	1.01	0.01					Litho_I	25	45	1	0.9	0.728568874	7	10.01782202	11	0.033333333	2.89121E-19	0.925925926	0.1216	0.801425762	5.055001735	6.055173611	13.95347684																																				
From "Input data" spreadsheet							9	Etch_AA	Dry_Etch		25	1.5		4.683229167		0.00	37478.59	0.00	0.41	2.35	0.04					Litho_Iw	25	45	1	0.9	0.781323717	10	10.7432011	11	0.025	3.85494E-19	0.694444444	0.1288	0.840661858	6.177798509	6.055173611	17.05276732																																				
Tool Name  	Mask Name						126	Etch_Contact	Dry_Etch(A)		25	1.5		4.683229167		0.00	37166.86	0.00	0.47	2.60	0.04					Meas_CD	25	5	0	0.95	0.343545887	30	14.72339515	15	0.005	0	0.131578947	0.176	0.377900476	0.12511705	0.903689236	0.345364443																																				
CMP_Ins	248_Mask						140	Etch_Mask	Dry_Etch(C) 		60	1.5		4.683229167		0.00	37129.73	0.00	0.47	1.08	0.02					Meas_Film	25	5	0	0.95	0.344590163	24	11.81451988	12	0.005	0	0.131578947	0.176	0.37904918	0.125248247	0.483333333	0.34572659																																				
CMP_Ins(C) 	248C_Mask						158	Etch_Via	Dry_Etch(C) 		30	1.5		4.683229167		0.00	37082.05	0.00	0.47	2.16	0.03					Meas_Overlay	25	5	0	0.95	0.281126488	18	10.30797121	11	0.005	3.18883E-21	0.131578947	0.176	0.309239136	0.125131136	1.089259259	0.345403326																																				
CMP_Ins(I)	Iw_Mask						173	Etch_Mask	Dry_Etch(C) 		60	1.5		4.683229167		0.00	37042.36	0.00	0.47	1.08	0.02					PVD_Met	25	5	0	0.854	0.287150064	1	1.126078681	2	0.016666667	#DIV/0!	0.487900078	0.15984832	0.31586507	0.4697701	3.204055556	1.296720863																																				
CMP_Met	I_Mask						191	Etch_Via	Dry_Etch(C) 		30	1.5		4.683229167		0.00	36994.80	0.00	0.47	2.15	0.03					PVD_Met(C) 	25	5	0	0.854	0.475466715	5	8.390589091	9	0.025	1.0842E-19	0.731850117	0.13989888	0.523013387	0.646791604	3.204055556	1.785358766																																				
CVD_Ins							206	Etch_Mask	Dry_Etch(C) 		60	1.5		4.683229167		0.00	36955.20	0.00	0.47	1.08	0.02					RTP_OxAn(C) 	25	5	0	0.854	0.459341718	2	2.417587991	3	0.02	0	0.585480094	0.1498736	0.50527589	0.605253071	3.204055556	1.670698677																																				
CVD_Ins(C) 							224	Etch_Via	Dry_Etch(C) 		30	1.5		4.683229167		0.00	36907.75	0.00	0.47	2.15	0.03					Test	25	5	0	0.95	0.37283889	6	21.03193739	22	0.04	0	1.052631579	0.1095	0.410122779	1.000363019	1.001944444	2.761332824																																				
CVD_Ins(I)							255	Etch_Via	Dry_Etch(C) 		30	1.5		4.683229167		0.00	36826.16	0.00	0.47	2.14	0.03					VP_HF_Clean	25	5	0	0.9	0.391937367	3	4.354859633	5	0.018888889	0.000112037	0.524691358	0.452131488	0.431131104	0.496072441	1.283395062	1.369324024																																				
CVD_Ins_Thin							279	Etch_PAD	Dry_Etch(C) 		40	1.5		4.683229167		0.00	36763.12	0.00	0.47	1.61	0.03					Wet_Bench	25	5	0	0.9	0.522667868	21	10.64693805	11	0.008	0	0.222222222	0.19	0.574934655	0.205798939	1.393263889	0.568073144																																				
CVD_Met							55	Etch_Gate	Dry_Etch(I)		25	1.5		4.683229167		0.00	37355.72	0.00	0.47	2.61	0.04					Wet_Bench(I)	25	5	0	0.9	0.497996628	18	9.222159775	10	0.008	0	0.222222222	0.19	0.547796291	0.205407705	1.393263889	0.566993208																																				
CVD_Met(C) 							82	Etch_Spacer	Dry_Etch(I)		30	1.5		4.683229167		0.00	37283.79	0.00	0.47	2.17	0.03																																																									
CVD_MetW							103	Dry_Strip	Dry_Etch(I)		30	1.5		1.557967836		0.00	37227.93	0.00	0.47	2.17	0.03																																																									
CVD_MetW(C) 							141	Etch_Metal	Dry_Etch_Met		30	1.5		4.189074074		0.00	37127.08	0.00	0.41	1.94	0.03																																																									
Dry_Etch							174	Etch_Metal	Dry_Etch_Met		30	1.5		4.189074074		0.00	37039.72	0.00	0.41	1.94	0.03																			Sum (hr)	Sum (hr)	factor																																				
Dry_Etch(A)							207	Etch_Metal	Dry_Etch_Met		30	1.5		4.189074074		0.00	36952.57	0.00	0.41	1.93	0.03																			233.4189162	644.3134169	2.760330771																																				
Dry_Etch(C) 							238	Etch_Metal	Dry_Etch_Met		30	1.5		4.189074074		0.00	36870.88	0.00	0.41	1.93	0.03																																																									
Dry_Etch(I)							269	Etch_Metal	Dry_Etch_Met		30	1.5		4.189074074		0.00	36789.37	0.00	0.41	1.92	0.03																																																									
Dry_Etch_Met							23	Dry_Strip	Dry_Strip		30	0.0		1.557967836		0.00	0.00	0.00	0.35	1.78	0.03																																																									
Dry_Strip							105	Plasma_Strip	Dry_Strip(D)		80	0.0		1.557967836		0.00	0.00	0.00	0.35	0.66	0.01																																																									
Dry_Strip(D)							127	Plasma_Strip	Dry_Strip(D)		80	0.0		1.557967836		0.00	0.00	0.00	0.35	0.66	0.01																																																									
Dry_Strip(I)							280	Plasma_Strip	Dry_Strip(D)		80	0.0		1.557967836		0.00	0.00	0.00	0.35	0.65	0.01																																																									
Furn_FastRmp							10	Plasma_Strip	Dry_Strip(I)		80	0.0		1.557967836		0.00	0.00	0.00	0.35	0.67	0.01																																																									
Furn_Nitr							34	Plasma_Strip	Dry_Strip(I)		80	0.0		1.557967836		0.00	0.00	0.00	0.35	0.67	0.01																																																									
Furn_OxAn							43	Plasma_Strip	Dry_Strip(I)		80	0.0		1.557967836		0.00	0.00	0.00	0.35	0.67	0.01																																																									
Furn_OxAn(I)							58	Plasma_Strip	Dry_Strip(I)		80	0.0		1.557967836		0.00	0.00	0.00	0.35	0.67	0.01																																																									
Furn_Poly							70	Plasma_Strip	Dry_Strip(I)		80	0.0		1.557967836		0.00	0.00	0.00	0.35	0.66	0.01																																																									
Furn_TEOS							77	Plasma_Strip	Dry_Strip(I)		80	0.0		1.557967836		0.00	0.00	0.00	0.35	0.66	0.01																																																									
Implant_HiE							92	Plasma_Strip	Dry_Strip(I)		80	0.0		1.557967836		0.00	0.00	0.00	0.35	0.66	0.01																																																									
Implant_LoE							99	Plasma_Strip	Dry_Strip(I)		80	0.0		1.557967836		0.00	0.00	0.00	0.35	0.66	0.01																																																									
Insp_PLY							2	Oxidation_Sac	Furn_FastRmp		50	0.6		10.41560185		0.00	14998.93	0.00	0.5	1.39	0.02																																																									
Insp_Visual							16	Oxidation	Furn_FastRmp		50	0.6		10.41560185		0.00	14983.95	0.00	0.5	1.39	0.02																																																									
Litho_248							20	Densification	Furn_FastRmp		50	0.6		10.41560185		0.00	14979.67	0.00	0.5	1.39	0.02																																																									
Litho_I							25	Oxidation_Sac	Furn_FastRmp		50	0.6		10.41560185		0.00	14974.32	0.00	0.5	1.39	0.02																																																									
Litho_Iw							47	Oxidation_Gate	Furn_FastRmp		50	0.6		10.41560185		0.00	14950.82	0.00	0.5	1.38	0.02																																																									
Meas_CD							63	Oxidation	Furn_FastRmp		50	0.6		10.41560185		0.00	14933.76	0.00	0.5	1.38	0.02																																																									
Meas_Film							4	LPCVD_Nitride	Furn_Nitr		30	0.6		14.27951389		0.00	14996.79	0.00	0.5	2.31	0.03																																																									
Meas_Overlay							117	Densification	Furn_OxAn		50	0.5		3.174791667		0.00	12396.92	0.00	0.5	1.38	0.02																																																									
PVD_Met							145	Anneal_Metal	Furn_OxAn		35	0.5		3.174791667		0.00	12372.16	0.00	0.5	1.96	0.03																																																									
PVD_Met(C) 							178	Anneal_Metal	Furn_OxAn		35	0.5		3.174791667		0.00	12343.05	0.00	0.5	1.96	0.03																																																									
RTP_OxAn(C) 							211	Anneal_Metal	Furn_OxAn		35	0.5		3.174791667		0.00	12314.01	0.00	0.5	1.95	0.03																																																									
Test							242	Anneal_Metal	Furn_OxAn		35	0.5		3.174791667		0.00	12286.78	0.00	0.5	1.95	0.03																																																									
VP_HF_Clean							273	Anneal_Metal	Furn_OxAn		35	0.5		3.174791667		0.00	12259.62	0.00	0.5	1.95	0.03																																																									
Wet_Bench							282	Anneal_Metal	Furn_OxAn		35	0.5		3.174791667		0.00	12251.75	0.00	0.5	1.94	0.03																																																									
Wet_Bench(I)							85	Anneal/Ox	Furn_OxAn(I)		35	0.5		3.174791667		0.00	12425.27	0.00	0.5	1.97	0.03																																																									
							102	Anneal	Furn_OxAn(I)		35	0.5		3.174791667		0.00	12410.20	0.00	0.5	1.97	0.03																																																									
							49	LPCVD_Poly	Furn_Poly		30	0.6		3.174791667		0.00	14948.69	0.00	0.5	2.31	0.03																																																									
							80	LPCVD_TEOS	Furn_TEOS		30	0.6		3.174791667		0.00	14915.64	0.00	0.5	2.30	0.03																																																									
							31	Implant	Implant_HiE		200	0.3		2.942098765		0.00	7483.95	0.00	0.63	0.47	0.01																																																									
							32	Implant	Implant_HiE		200	0.3		2.942098765		0.00	7483.42	0.00	0.63	0.47	0.01																																																									
							40	Implant	Implant_HiE		200	0.3		2.942098765		0.00	7479.15	0.00	0.63	0.47	0.01																																																									
							41	Implant	Implant_HiE		200	0.3		2.942098765		0.00	7478.61	0.00	0.63	0.47	0.01																																																									
							33	Implant	Implant_LoE		150	0.3		2.942098765		0.00	7482.89	0.00	0.58	0.55	0.01																																																									
							42	Implant	Implant_LoE		150	0.3		2.942098765		0.00	7478.08	0.00	0.58	0.55	0.01																																																									
							69	Implant	Implant_LoE		150	0.3		2.942098765		0.00	7463.68	0.00	0.58	0.55	0.01																																																									
							76	Implant	Implant_LoE		150	0.3		2.942098765		0.00	7459.95	0.00	0.58	0.55	0.01																																																									
							91	Implant	Implant_LoE		150	0.3		2.942098765		0.00	7451.97	0.00	0.58	0.55	0.01																																																									
							98	Implant	Implant_LoE		150	0.3		2.942098765		0.00	7448.24	0.00	0.58	0.55	0.01																																																									
							7	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.58	0.01																																																									
							13	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.58	0.01																																																									
							29	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.58	0.01																																																									
							38	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.58	0.01																																																									
							53	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.58	0.01																																																									
							60	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.58	0.01																																																									
							67	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.58	0.01																																																									
							74	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.58	0.01																																																									
							89	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.58	0.01																																																									
							96	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							120	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							124	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							133	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							138	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							144	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							150	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							153	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							156	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							161	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							166	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							171	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							177	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							183	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							186	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							189	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							194	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							199	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							204	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							210	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							216	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							219	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							222	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							227	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							232	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							236	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							241	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							247	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							250	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							253	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							258	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							263	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							267	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							272	Inspect_PLY	Insp_PLY		200	0.0		0.903689236		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							57	Inspect_Visual	Insp_Visual		200	0.0		0.695802469		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							109	Inspect_Visual	Insp_Visual		200	0.0		0.695802469		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							51	Expose_Gate	Litho_248	248C_Mask	25	3.5	2.25	11.08736111	2.00	49821.85	87188.24	56049.58	0.2	1.73	0.04																																																									
							122	Expose_Contact	Litho_248	248_Mask	25	3.5	2.25	11.08736111	0.63	15490.61	86747.44	55766.21	0.2	1.72	0.04																																																									
							6	Expose_AA	Litho_I	I_Mask	30	0.8	0.70	6.055173611	0.18	4373.44	19992.86	17493.75	0.2	1.45	0.03																																																									
							136	Expose_Line	Litho_I	I_Mask	30	0.8	0.70	6.055173611	0.18	4333.04	19808.18	17332.16	0.2	1.43	0.03																																																									
							154	Expose_Via	Litho_I	I_Mask	30	0.8	0.70	6.055173611	0.18	4327.47	19782.74	17309.90	0.2	1.43	0.03																																																									
							169	Expose_Line	Litho_I	I_Mask	30	0.8	0.70	6.055173611	0.18	4322.84	19761.57	17291.37	0.2	1.43	0.03																																																									
							187	Expose_Via	Litho_I	I_Mask	30	0.8	0.70	6.055173611	0.18	4317.29	19736.19	17269.17	0.2	1.43	0.03																																																									
							202	Expose_Line	Litho_I	I_Mask	30	0.8	0.70	6.055173611	0.18	4312.67	19715.07	17250.69	0.2	1.43	0.03																																																									
							220	Expose_Via	Litho_I	I_Mask	30	0.8	0.70	6.055173611	0.18	4307.13	19689.75	17228.53	0.2	1.42	0.03																																																									
							27	Expose_Implant	Litho_Iw	Iw_Mask	40	0.8	0.70	6.055173611	0.10	2495.36	19962.91	17467.55	0.2	1.08	0.03																																																									
							36	Expose_Implant	Litho_Iw	Iw_Mask	40	0.8	0.70	6.055173611	0.10	2493.76	19950.09	17456.33	0.2	1.08	0.03																																																									
							65	Expose_Implant	Litho_Iw	Iw_Mask	40	0.8	0.70	6.055173611	0.10	2488.60	19908.83	17420.23	0.2	1.08	0.03																																																									
							72	Expose_Implant	Litho_Iw	Iw_Mask	40	0.8	0.70	6.055173611	0.10	2487.36	19898.89	17411.53	0.2	1.08	0.03																																																									
							87	Expose_Implant	Litho_Iw	Iw_Mask	40	0.8	0.70	6.055173611	0.10	2484.70	19877.59	17392.89	0.2	1.08	0.03																																																									
							94	Expose_Implant	Litho_Iw	Iw_Mask	40	0.8	0.70	6.055173611	0.10	2483.46	19867.66	17384.20	0.2	1.08	0.03																																																									
							234	Expose_Line	Litho_Iw	Iw_Mask	40	0.8	0.70	6.055173611	0.10	2458.76	19670.08	17211.32	0.2	1.07	0.03																																																									
							251	Expose_Via	Litho_Iw	Iw_Mask	40	0.8	0.70	6.055173611	0.10	2455.78	19646.23	17190.45	0.2	1.07	0.03																																																									
							265	Expose_Line	Litho_Iw	Iw_Mask	40	0.8	0.70	6.055173611	0.10	2453.33	19626.60	17173.28	0.2	1.06	0.03																																																									
							277	Expose_Pad	Litho_Iw	Iw_Mask	40	0.8	0.70	6.055173611	0.10	2451.22	19609.80	17158.57	0.2	1.06	0.03																																																									
							8	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.50	0.01																																																									
							14	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.50	0.01																																																									
							30	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.50	0.01																																																									
							39	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							54	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							61	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							68	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							75	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							90	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							97	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							125	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							129	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							139	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							143	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							157	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							160	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							172	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							176	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							190	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							193	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							205	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							209	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							223	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							226	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							237	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							240	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							254	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							257	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							268	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							271	Meas_CD	Meas_CD		200	0.0		0.903689236		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							3	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.50	0.01																																																									
							5	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.50	0.01																																																									
							17	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.50	0.01																																																									
							19	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.50	0.01																																																									
							26	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.50	0.01																																																									
							48	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							50	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							56	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							64	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							81	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							83	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							86	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							104	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							114	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							116	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							119	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							149	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							152	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							182	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							185	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							215	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							218	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							246	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							249	Meas_Film	Meas_Film		200	0.0		0.483333333		0.00	0.00	0.00	0.65	0.49	0.01																																																									
							28	Meas_Overlay	Meas_Overlay		200	0.0		1.089259259		0.00	0.00	0.00	0.7	0.58	0.01																																																									
							37	Meas_Overlay	Meas_Overlay		200	0.0		1.089259259		0.00	0.00	0.00	0.7	0.58	0.01																																																									
							52	Meas_Overlay	Meas_Overlay		200	0.0		1.089259259		0.00	0.00	0.00	0.7	0.58	0.01																																																									
							66	Meas_Overlay	Meas_Overlay		200	0.0		1.089259259		0.00	0.00	0.00	0.7	0.58	0.01																																																									
							73	Meas_Overlay	Meas_Overlay		200	0.0		1.089259259		0.00	0.00	0.00	0.7	0.58	0.01																																																									
							88	Meas_Overlay	Meas_Overlay		200	0.0		1.089259259		0.00	0.00	0.00	0.7	0.58	0.01																																																									
							95	Meas_Overlay	Meas_Overlay		200	0.0		1.089259259		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							123	Meas_Overlay	Meas_Overlay		200	0.0		1.089259259		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							137	Meas_Overlay	Meas_Overlay		200	0.0		1.089259259		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							155	Meas_Overlay	Meas_Overlay		200	0.0		1.089259259		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							170	Meas_Overlay	Meas_Overlay		200	0.0		1.089259259		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							188	Meas_Overlay	Meas_Overlay		200	0.0		1.089259259		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							203	Meas_Overlay	Meas_Overlay		200	0.0		1.089259259		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							221	Meas_Overlay	Meas_Overlay		200	0.0		1.089259259		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							235	Meas_Overlay	Meas_Overlay		200	0.0		1.089259259		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							252	Meas_Overlay	Meas_Overlay		200	0.0		1.089259259		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							266	Meas_Overlay	Meas_Overlay		200	0.0		1.089259259		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							278	Meas_Overlay	Meas_Overlay		200	0.0		1.089259259		0.00	0.00	0.00	0.7	0.57	0.01																																																									
							108	PVD_Ti/Co	PVD_Met		60	1.5		3.204055556		0.00	37214.65	0.00	0.49	1.13	0.02																																																									
							134	PVD_Al/Cu	PVD_Met(C) 		40	1.5		3.204055556		0.00	37145.64	0.00	0.49	1.69	0.03																																																									
							167	PVD_Al/Cu	PVD_Met(C) 		40	1.5		3.204055556		0.00	37058.23	0.00	0.49	1.68	0.03																																																									
							200	PVD_Al/Cu	PVD_Met(C) 		40	1.5		3.204055556		0.00	36971.04	0.00	0.49	1.68	0.03																																																									
							233	PVD_Al/Cu	PVD_Met(C) 		40	1.5		3.204055556		0.00	36884.04	0.00	0.49	1.67	0.03																																																									
							264	PVD_Al/Cu	PVD_Met(C) 		40	1.5		3.204055556		0.00	36802.51	0.00	0.49	1.67	0.03																																																									
							110	RTP_Silicide	RTP_OxAn(C) 		50	0.5		3.204055556		0.00	12403.11	0.00	0.43	1.21	0.02																																																									
							112	RTP_Anneal	RTP_OxAn(C) 		50	0.5		3.204055556		0.00	12401.34	0.00	0.43	1.21	0.02																																																									
							146	Test	Test		25	0.0		1.001944444		0.00	0.00	0.00	0.61	3.52	0.04																																																									
							179	Test	Test		25	0.0		1.001944444		0.00	0.00	0.00	0.61	3.52	0.04																																																									
							212	Test	Test		25	0.0		1.001944444		0.00	0.00	0.00	0.61	3.51	0.04																																																									
							243	Test	Test		25	0.0		1.001944444		0.00	0.00	0.00	0.61	3.50	0.04																																																									
							274	Test	Test		25	0.0		1.001944444		0.00	0.00	0.00	0.61	3.49	0.04																																																									
							283	Test	Test		25	0.0		1.001944444		0.00	0.00	0.00	0.61	3.49	0.04																																																									
							11	Clean_O3	VP_HF_Clean		40	0.3		1.283395062		0.00	7494.65	0.00	0.55	1.93	0.03																																																									
							46	Clean_O3	VP_HF_Clean		150	0.3		1.283395062		0.00	7475.95	0.00	0.55	0.51	0.01																																																									
							107	Clean_O3	VP_HF_Clean		40	0.3		1.283395062		0.00	7443.46	0.00	0.55	1.91	0.03																																																									
							111	Wet_Strip Ti/Co	Wet_Bench		125	0.5		1.393263889		0.00	12402.23	0.00	0.46	0.51	0.01																																																									
							128	Clean_Post_Strip	Wet_Bench		125	0.5		1.393263889		0.00	12387.18	0.00	0.46	0.51	0.01																																																									
							142	Clean_Post_Strip	Wet_Bench		125	0.5		1.393263889		0.00	12374.81	0.00	0.46	0.51	0.01																																																									
							147	Clean_Metal	Wet_Bench		125	0.5		1.393263889		0.00	12370.39	0.00	0.46	0.51	0.01																																																									
							159	Clean_Post_Strip	Wet_Bench		125	0.5		1.393263889		0.00	12359.80	0.00	0.46	0.51	0.01																																																									
							162	Clean_Metal	Wet_Bench		125	0.5		1.393263889		0.00	12357.15	0.00	0.46	0.51	0.01																																																									
							175	Clean_Post_Strip	Wet_Bench		125	0.5		1.393263889		0.00	12345.69	0.00	0.46	0.51	0.01																																																									
							180	Clean_Metal	Wet_Bench		125	0.5		1.393263889		0.00	12341.29	0.00	0.46	0.51	0.01																																																									
							192	Clean_Post_Strip	Wet_Bench		125	0.5		1.393263889		0.00	12330.72	0.00	0.46	0.51	0.01																																																									
							195	Clean_Metal	Wet_Bench		125	0.5		1.393263889		0.00	12328.08	0.00	0.46	0.51	0.01																																																									
							208	Clean_Post_Strip	Wet_Bench		125	0.5		1.393263889		0.00	12316.64	0.00	0.46	0.51	0.01																																																									
							213	Clean_Metal	Wet_Bench		125	0.5		1.393263889		0.00	12312.25	0.00	0.46	0.51	0.01																																																									
							225	Clean_Post_Strip	Wet_Bench		125	0.5		1.393263889		0.00	12301.70	0.00	0.46	0.51	0.01																																																									
							228	Clean_Metal	Wet_Bench		125	0.5		1.393263889		0.00	12299.07	0.00	0.46	0.51	0.01																																																									
							239	Clean_Post_Strip	Wet_Bench		125	0.5		1.393263889		0.00	12289.42	0.00	0.46	0.51	0.01																																																									
							244	Clean_Metal	Wet_Bench		125	0.5		1.393263889		0.00	12285.03	0.00	0.46	0.51	0.01																																																									
							256	Clean_Post_Strip	Wet_Bench		125	0.5		1.393263889		0.00	12274.51	0.00	0.46	0.51	0.01																																																									
							259	Clean_Metal	Wet_Bench		125	0.5		1.393263889		0.00	12271.88	0.00	0.46	0.51	0.01																																																									
							270	Clean_Post_Strip	Wet_Bench		125	0.5		1.393263889		0.00	12262.25	0.00	0.46	0.50	0.01																																																									
							275	Clean_Metal	Wet_Bench		125	0.5		1.393263889		0.00	12257.87	0.00	0.46	0.50	0.01																																																									
							281	Clean_Post_Strip	Wet_Bench		125	0.5		1.393263889		0.00	12252.62	0.00	0.46	0.50	0.01																																																									
							1	Clean_Pre_OxAn	Wet_Bench(I)		125	0.5		1.393263889		0.00	12500.00	0.00	0.46	0.51	0.01																																																									
							12	Clean_Post_Strip	Wet_Bench(I)		125	0.5		1.393263889		0.00	12490.19	0.00	0.46	0.51	0.01																																																									
							15	Clean_Pre_OxAn	Wet_Bench(I)		125	0.5		1.393263889		0.00	12487.51	0.00	0.46	0.51	0.01																																																									
							22	Wet_Strip	Wet_Bench(I)		125	0.5		1.393263889		0.00	12481.27	0.00	0.46	0.51	0.01																																																									
							24	Clean_Pre_OxAn	Wet_Bench(I)		125	0.5		1.393263889		0.00	12479.49	0.00	0.46	0.51	0.01																																																									
							35	Clean_Post_Strip	Wet_Bench(I)		125	0.5		1.393263889		0.00	12469.70	0.00	0.46	0.51	0.01																																																									
							44	Clean_Post_Strip	Wet_Bench(I)		125	0.5		1.393263889		0.00	12461.69	0.00	0.46	0.51	0.01																																																									
							45	Wet_Strip	Wet_Bench(I)		125	0.5		1.393263889		0.00	12460.80	0.00	0.46	0.51	0.01																																																									
							59	Clean_Post_Strip	Wet_Bench(I)		125	0.5		1.393263889		0.00	12448.35	0.00	0.46	0.51	0.01																																																									
							62	Clean_Pre_OxAn	Wet_Bench(I)		125	0.5		1.393263889		0.00	12445.69	0.00	0.46	0.51	0.01																																																									
							71	Clean_Post_Strip	Wet_Bench(I)		125	0.5		1.393263889		0.00	12437.69	0.00	0.46	0.51	0.01																																																									
							78	Clean_Post_Strip	Wet_Bench(I)		125	0.5		1.393263889		0.00	12431.48	0.00	0.46	0.51	0.01																																																									
							79	Clean_Pre_OxAn	Wet_Bench(I)		125	0.5		1.393263889		0.00	12430.59	0.00	0.46	0.51	0.01																																																									
							84	Clean_Pre_OxAn	Wet_Bench(I)		125	0.5		1.393263889		0.00	12426.15	0.00	0.46	0.51	0.01																																																									
							93	Clean_Post_Strip	Wet_Bench(I)		125	0.5		1.393263889		0.00	12418.17	0.00	0.46	0.51	0.01																																																									
							100	Clean_Post_Strip	Wet_Bench(I)		125	0.5		1.393263889		0.00	12411.97	0.00	0.46	0.51	0.01																																																									
							101	Clean_Pre_OxAn	Wet_Bench(I)		125	0.5		1.393263889		0.00	12411.08	0.00	0.46	0.51	0.01																																																									
							106	Clean_Post_Strip	Wet_Bench(I)		125	0.5		1.393263889		0.00	12406.65	0.00	0.46	0.51	0.01																																																									




Expense Cost Calculation

partial cost total				Equipment Cost per wafer								Personnel Coefficients	Level of Automation	(0,0)		(1,1)		(1.5,1.5)		(2,2)			Number of Personnel (fractional tools)	(0,0)		(1,1)		(1.5,1.5)		(2,2)			Number of Personnel (integer tools)	(0,0)		(1,1)		(1.5,1.5)		(2,2)					Space in sq.ft.	Non-manufacturing (sq. ft.)						Coeff for annual space cost	Non-manufacturing (sq. ft.)				Cleanroom(sq.ft.)	non-cleanroom(sq.ft.)		Annual Space Cost (fractional Tools)	Non-manufacturing (sq. ft.)				Cleanroom(sq.ft.)	non-cleanroom(sq.ft.)		Annual Space Cost (fractional Tools)	Non-manufacturing (sq. ft.)				Cleanroom(sq.ft.)	non-cleanroom(sq.ft.)																																																															
							Cost per type of tool						Personnel type	Engineer	Technicians	Engineer	Technicians	Engineer	Technicians	Engineer	Technicians		Personnel type	Engineer	Technicians	Engineer	Technicians	Engineer	Technicians	Engineer	Technicians		Personnel type	Engineer	Technicians	Engineer	Technicians	Engineer	Technicians	Engineer	Technicians					level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)				level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)					level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)					level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)																																																																	
NOTE: 30 working days per month and 360 working days 							Fractional		Integer				Fixed	30	100	32	108	33	120	35	128		Fixed	30	100	32	108	33	120	35	128		Fixed	30	100	32	108	33	120	35	128				Fixed 	15450	16350	17400	18300			Fixed 	880650	931950	991800	1043100				Fixed 	880650	931950	991800	1043100				Fixed 	880650	931950	991800	1043100																																																																	
               per year are fixed in this spreadsheet.					#tools	#tools	tool deprec(frac)	maint(frac)	tool deprec(integ)	mainte(integ)			Per Wafer Start/Month	0.00175	0.00065	0.00185	0.0007	0.0019	0.0009	0.00195	0.00105		Per Wafer Start/Month	43.75	16.25	46.25	17.5	47.5	22.5	48.75	26.25		Per Wafer Start/Month	43.75	16.25	46.25	17.5	47.5	22.5	48.75	26.25				Per wafer	0.34866	0.36183	0.38061	0.39105			Per wafer	19.87362	20.62431	21.69477	22.28985				Per wafer	496840.5	515607.75	542369.25	557246.25				Per wafer	496840.5	515607.75	542369.25	557246.25																																																																	
				Tool Type	fractional	Round Up	$mm	$mm	$mm	$mm			Per Tool Type:										Per Tool Type:										Per Tool Type:												Per Tool							Per Tool								Per Tool								Per Tool																																																																					
				CMP_Ins	2.50	3	1.35	0.349	1.62	0.42			CMP_Ins	0.019792973	0.30161	0.022267014	0.29623	0.022267014	0.29084	0.024741698	0.25314		CMP_Ins	0.049386934	0.752579693	0.0555601	0.739137837	0.0555601	0.725699476	0.061734871	0.631627451		CMP_Ins	0.059378918	0.904841907	0.066801041	0.88868049	0.066801041	0.872523274	0.074225095	0.759418561				CMP_Ins	25.59	25.56	25.15	22.70			CMP_Ins	1458.63	1456.75	1433.73	1293.71	126000	91200		CMP_Ins	3639.54	3634.85	3577.40	3228.04	314392.07	227559.98		CMP_Ins	4375.89	4370.26	4301.19	3881.14	378000.00	273600.00																																																															
				CMP_Ins(C) 	19.84	20	10.72	2.778	10.80	2.8			CMP_Ins(C) 	0.019792973	0.30161	0.022267014	0.29623	0.022267014	0.29084	0.024741698	0.25314		CMP_Ins(C) 	0.392790738	5.985516981	0.441887984	5.878609425	0.441887984	5.77172966	0.490997997	5.023543511		CMP_Ins(C) 	0.395859452	6.032279383	0.445340275	5.924536602	0.445340275	5.816821829	0.494833964	5.062790407				CMP_Ins(C) 	25.59	25.56	25.15	22.70			CMP_Ins(C) 	1458.63	1456.75	1433.73	1293.71	126000	91200		CMP_Ins(C) 	28946.45	28909.20	28452.29	25673.68	2500464.89	1809860.30		CMP_Ins(C) 	29172.59	29135.05	28674.57	25874.26	2520000.00	1824000.00																																																															
				CMP_Ins(I)	2.51	3	1.36	0.352	1.62	0.42			CMP_Ins(I)	0.019792973	0.30161	0.022267014	0.29623	0.022267014	0.29084	0.024741698	0.25314		CMP_Ins(I)	0.049730106	0.757809093	0.055946167	0.744273835	0.055946167	0.730742096	0.062163844	0.636016399		CMP_Ins(I)	0.059378918	0.904841907	0.066801041	0.88868049	0.066801041	0.872523274	0.074225095	0.759418561				CMP_Ins(I)	25.59	25.56	25.15	22.70			CMP_Ins(I)	1458.63	1456.75	1433.73	1293.71	126000	91200		CMP_Ins(I)	3664.83	3660.11	3602.26	3250.47	316576.67	229141.21		CMP_Ins(I)	4375.89	4370.26	4301.19	3881.14	378000.00	273600.00																																																															
				CMP_Met	12.41	13	6.70	1.737	7.02	1.82			CMP_Met	0.019792973	0.30161	0.022267014	0.29623	0.022267014	0.29084	0.024741698	0.25314		CMP_Met	0.245536784	3.74159686	0.276227885	3.674768051	0.276227885	3.607956613	0.306926965	3.140259177		CMP_Met	0.257308643	3.920981599	0.289471179	3.850948791	0.289471179	3.780934189	0.321642076	3.290813764				CMP_Met	25.59	25.56	25.15	22.70			CMP_Met	1458.63	1456.75	1433.73	1293.71	126000	91200		CMP_Met	18094.67	18071.38	17785.76	16048.83	1563061.57	1131358.85		CMP_Met	18962.19	18937.78	18638.47	16818.27	1638000.00	1185600.00																																																															
				CVD_Ins	3.50	4	2.83	0.734	3.24	0.84			CVD_Ins	0.019792973	0.18097	0.022267014	0.17774	0.022267014	0.17450	0.024741698	0.15188		CVD_Ins	0.06922762	0.632952441	0.077880791	0.621647252	0.077880791	0.610345002	0.086536212	0.531226315		CVD_Ins	0.07917189	0.723873526	0.089068055	0.710944392	0.089068055	0.698018619	0.098966793	0.607534849				CVD_Ins	16.54	16.67	16.43	15.10			CVD_Ins	942.87	950.20	936.39	860.84	126000	91200		CVD_Ins	3297.77	3323.42	3275.11	3010.88	440695.81	318979.82		CVD_Ins	3771.48	3800.82	3745.56	3443.38	504000.00	364800.00																																																															
				CVD_Ins(C) 	9.26	10	7.50	1.945	8.10	2.1			CVD_Ins(C) 	0.019792973	0.18097	0.022267014	0.17774	0.022267014	0.17450	0.024741698	0.15188		CVD_Ins(C) 	0.183307882	1.675995389	0.206220623	1.646060369	0.206220623	1.61613313	0.229139321	1.406634679		CVD_Ins(C) 	0.197929726	1.809683815	0.222670137	1.777360981	0.222670137	1.745046549	0.247416982	1.518837122				CVD_Ins(C) 	16.54	16.67	16.43	15.10			CVD_Ins(C) 	942.87	950.20	936.39	860.84	126000	91200		CVD_Ins(C) 	8732.16	8800.09	8672.16	7972.50	1166918.87	844626.99		CVD_Ins(C) 	9428.70	9502.05	9363.90	8608.44	1260000.00	912000.00																																																															
				CVD_Ins(I)	1.08	2	0.88	0.228	1.62	0.42			CVD_Ins(I)	0.019792973	0.18097	0.022267014	0.17774	0.022267014	0.17450	0.024741698	0.15188		CVD_Ins(I)	0.021450702	0.196125101	0.024131952	0.192622103	0.024131952	0.189120015	0.0268139	0.164604492		CVD_Ins(I)	0.039585945	0.361936763	0.044534027	0.355472196	0.044534027	0.34900931	0.049483396	0.303767424				CVD_Ins(I)	16.54	16.67	16.43	15.10			CVD_Ins(I)	942.87	950.20	936.39	860.84	126000	91200		CVD_Ins(I)	1021.84	1029.79	1014.82	932.94	136552.93	98838.31		CVD_Ins(I)	1885.74	1900.41	1872.78	1721.69	252000.00	182400.00																																																															
				CVD_Ins_Thin	1.61	2	0.87	0.225	1.08	0.28			CVD_Ins_Thin	0.019792973	0.30161	0.022267014	0.29623	0.022267014	0.29084	0.024741698	0.25314		CVD_Ins_Thin	0.031833403	0.485091319	0.03581245	0.476427084	0.03581245	0.467765101	0.03979253	0.407128967		CVD_Ins_Thin	0.039585945	0.603227938	0.044534027	0.59245366	0.044534027	0.581682183	0.049483396	0.506279041				CVD_Ins_Thin	25.59	25.56	25.15	22.70			CVD_Ins_Thin	1458.63	1456.75	1433.73	1293.71	126000	91200		CVD_Ins_Thin	2345.94	2342.92	2305.89	2080.70	202648.13	146678.64		CVD_Ins_Thin	2917.26	2913.51	2867.46	2587.43	252000.00	182400.00																																																															
				CVD_Met	1.19	2	1.13	0.293	1.89	0.49			CVD_Met	0.019792973	0.24129	0.022267014	0.23698	0.022267014	0.23267	0.024741698	0.20251		CVD_Met	0.023644309	0.288241854	0.026599752	0.283093554	0.026599752	0.277946594	0.029555963	0.241916529		CVD_Met	0.039585945	0.482582351	0.044534027	0.473962928	0.044534027	0.465345746	0.049483396	0.405023233				CVD_Met	21.07	21.11	20.79	18.90			CVD_Met	1200.75	1203.48	1185.06	1077.28	126000	91200		CVD_Met	1434.39	1437.65	1415.65	1286.90	150517.21	108945.79		CVD_Met	2401.50	2406.96	2370.12	2154.56	252000.00	182400.00																																																															
				CVD_Met(C) 	4.75	5	4.49	1.164	4.73	1.225			CVD_Met(C) 	0.019792973	0.24129	0.022267014	0.23698	0.022267014	0.23267	0.024741698	0.20251		CVD_Met(C) 	0.094025533	1.146241737	0.105778342	1.125768668	0.105778342	1.105300921	0.117534208	0.962021369		CVD_Met(C) 	0.098964863	1.206455877	0.111335069	1.18490732	0.111335069	1.163364366	0.123708491	1.012558081				CVD_Met(C) 	21.07	21.11	20.79	18.90			CVD_Met(C) 	1200.75	1203.48	1185.06	1077.28	126000	91200		CVD_Met(C) 	5704.10	5717.07	5629.57	5117.56	598556.74	433241.07		CVD_Met(C) 	6003.75	6017.39	5925.30	5386.39	630000.00	456000.00																																																															
				CVD_MetW	1.02	2	0.97	0.251	1.89	0.49			CVD_MetW	0.019792973	0.24129	0.022267014	0.23698	0.022267014	0.23267	0.024741698	0.20251		CVD_MetW	0.020265104	0.247046809	0.022798159	0.242634296	0.022798159	0.238222931	0.025331874	0.207342223		CVD_MetW	0.039585945	0.482582351	0.044534027	0.473962928	0.044534027	0.465345746	0.049483396	0.405023233				CVD_MetW	21.07	21.11	20.79	18.90			CVD_MetW	1200.75	1203.48	1185.06	1077.28	126000	91200		CVD_MetW	1229.39	1232.19	1213.33	1102.98	129005.54	93375.44		CVD_MetW	2401.50	2406.96	2370.12	2154.56	252000.00	182400.00																																																															
				CVD_MetW(C) 	4.07	5	3.85	0.998	4.73	1.225			CVD_MetW(C) 	0.019792973	0.24129	0.022267014	0.23698	0.022267014	0.23267	0.024741698	0.20251		CVD_MetW(C) 	0.08058756	0.982422782	0.090660678	0.96487569	0.090660678	0.947333159	0.100736415	0.824530881		CVD_MetW(C) 	0.098964863	1.206455877	0.111335069	1.18490732	0.111335069	1.163364366	0.123708491	1.012558081				CVD_MetW(C) 	21.07	21.11	20.79	18.90			CVD_MetW(C) 	1200.75	1203.48	1185.06	1077.28	126000	91200		CVD_MetW(C) 	4888.88	4899.99	4825.00	4386.17	513012.01	371322.98		CVD_MetW(C) 	6003.75	6017.39	5925.30	5386.39	630000.00	456000.00																																																															
				Dry_Etch	2.35	3	1.59	0.412	2.03	0.525			Dry_Etch	0.039585945	0.18097	0.044534027	0.17774	0.044534027	0.17450	0.049483396	0.15188		Dry_Etch	0.093134049	0.425765206	0.104775427	0.418160597	0.104775427	0.410557965	0.116419831	0.357337561		Dry_Etch	0.118757835	0.542905144	0.133602082	0.533208294	0.133602082	0.523513965	0.148450189	0.455651137				Dry_Etch	19.51	20.01	19.77	18.81			Dry_Etch	1112.10	1140.59	1126.77	1072.39	126000	91200		Dry_Etch	2616.44	2683.47	2650.97	2523.01	296440.82	214566.69		Dry_Etch	3336.30	3421.76	3380.32	3217.16	378000.00	273600.00																																																															
				Dry_Etch(A)	2.60	3	1.75	0.455	2.03	0.525			Dry_Etch(A)	0.039585945	0.18097	0.044534027	0.17774	0.044534027	0.17450	0.049483396	0.15188		Dry_Etch(A)	0.102815181	0.470022803	0.115666661	0.461627707	0.115666661	0.453234793	0.128521482	0.394482216		Dry_Etch(A)	0.118757835	0.542905144	0.133602082	0.533208294	0.133602082	0.523513965	0.148450189	0.455651137				Dry_Etch(A)	19.51	20.01	19.77	18.81			Dry_Etch(A)	1112.10	1140.59	1126.77	1072.39	126000	91200		Dry_Etch(A)	2888.42	2962.41	2926.53	2785.27	327255.36	236870.55		Dry_Etch(A)	3336.30	3421.76	3380.32	3217.16	378000.00	273600.00																																																															
				Dry_Etch(C) 	13.45	14	9.08	2.354	9.45	2.45			Dry_Etch(C) 	0.039585945	0.18097	0.044534027	0.17774	0.044534027	0.17450	0.049483396	0.15188		Dry_Etch(C) 	0.532392571	2.433849224	0.598939479	2.390378147	0.598939479	2.346918369	0.665503691	2.042688629		Dry_Etch(C) 	0.554203232	2.533557341	0.623476385	2.488305373	0.623476385	2.443065168	0.692767549	2.126371971				Dry_Etch(C) 	19.51	20.01	19.77	18.81			Dry_Etch(C) 	1112.10	1140.59	1126.77	1072.39	126000	91200		Dry_Etch(C) 	14956.66	15339.80	15154.01	14422.55	1694577.80	1226551.55		Dry_Etch(C) 	15569.40	15968.23	15774.83	15013.40	1764000.00	1276800.00																																																															
				Dry_Etch(I)	6.95	7	4.69	1.216	4.73	1.225			Dry_Etch(I)	0.039585945	0.18097	0.044534027	0.17774	0.044534027	0.17450	0.049483396	0.15188		Dry_Etch(I)	0.275106601	1.257658395	0.309493808	1.235195308	0.309493808	1.212738061	0.343889956	1.055531492		Dry_Etch(I)	0.277101616	1.26677867	0.311738192	1.244152686	0.311738192	1.221532584	0.346383774	1.063185985				Dry_Etch(I)	19.51	20.01	19.77	18.81			Dry_Etch(I)	1112.10	1140.59	1126.77	1072.39	126000	91200		Dry_Etch(I)	7728.65	7926.63	7830.63	7452.66	875649.97	633803.79		Dry_Etch(I)	7784.70	7984.11	7887.41	7506.70	882000.00	638400.00																																																															
				Dry_Etch_Met	9.67	10	6.52	1.692	6.75	1.75			Dry_Etch_Met	0.039585945	0.18097	0.044534027	0.17774	0.044534027	0.17450	0.049483396	0.15188		Dry_Etch_Met	0.382646783	1.749281691	0.430476077	1.718037702	0.430476077	1.686801834	0.478317806	1.468142638		Dry_Etch_Met	0.395859452	1.809683815	0.445340275	1.777360981	0.445340275	1.745046549	0.494833964	1.518837122				Dry_Etch_Met	19.51	20.01	19.77	18.81			Dry_Etch_Met	1112.10	1140.59	1126.77	1072.39	126000	91200		Dry_Etch_Met	10749.81	11025.18	10891.65	10365.93	1217944.77	881560.02		Dry_Etch_Met	11121.00	11405.88	11267.73	10723.86	1260000.00	912000.00																																																															
				Dry_Strip	1.78	2	0.48	0.124	0.54	0.14			Dry_Strip	0.019792973	0.12065	0.022267014	0.11849	0.022267014	0.11634	0.024741698	0.10126		Dry_Strip	0.035188589	0.214487641	0.03958702	0.210656669	0.03958702	0.206826692	0.043986594	0.180015861		Dry_Strip	0.039585945	0.241291175	0.044534027	0.236981464	0.044534027	0.232672873	0.049483396	0.202511616				Dry_Strip	12.02	12.23	12.07	11.31			Dry_Strip	684.99	696.93	687.72	644.41	88200	63840		Dry_Strip	1217.80	1239.03	1222.65	1145.65	156804.82	113496.82		Dry_Strip	1369.98	1393.86	1375.44	1288.82	176400.00	127680.00																																																															
				Dry_Strip(D)	1.98	2	0.53	0.139	0.54	0.14			Dry_Strip(D)	0.019792973	0.12065	0.022267014	0.11849	0.022267014	0.11634	0.024741698	0.10126		Dry_Strip(D)	0.039172647	0.238771969	0.044069069	0.234507253	0.044069069	0.230243646	0.048966764	0.200397289		Dry_Strip(D)	0.039585945	0.241291175	0.044534027	0.236981464	0.044534027	0.232672873	0.049483396	0.202511616				Dry_Strip(D)	12.02	12.23	12.07	11.31			Dry_Strip(D)	684.99	696.93	687.72	644.41	88200	63840		Dry_Strip(D)	1355.68	1379.31	1361.08	1275.36	174558.29	126346.95		Dry_Strip(D)	1369.98	1393.86	1375.44	1288.82	176400.00	127680.00																																																															
				Dry_Strip(I)	5.32	6	1.44	0.372	1.62	0.42			Dry_Strip(I)	0.019792973	0.12065	0.022267014	0.11849	0.022267014	0.11634	0.024741698	0.10126		Dry_Strip(I)	0.105284695	0.641749687	0.118444855	0.630287371	0.118444855	0.618828034	0.131608436	0.538609695		Dry_Strip(I)	0.118757835	0.723873526	0.133602082	0.710944392	0.133602082	0.698018619	0.148450189	0.607534849				Dry_Strip(I)	12.02	12.23	12.07	11.31			Dry_Strip(I)	684.99	696.93	687.72	644.41	88200	63840		Dry_Strip(I)	3643.66	3707.18	3658.19	3427.81	469161.98	339583.91		Dry_Strip(I)	4109.94	4181.59	4126.33	3866.46	529200.00	383040.00																																																															
				Furn_FastRmp	8.32	9	2.25	0.582	2.43	0.63			Furn_FastRmp	0.019792973	0.12065	0.022267014	0.11849	0.022267014	0.11634	0.024741698	0.10126		Furn_FastRmp	0.164614205	1.003385289	0.185190312	0.985463784	0.185190312	0.967546939	0.205771769	0.84212436		Furn_FastRmp	0.178136753	1.085810289	0.200403124	1.066416588	0.200403124	1.047027929	0.222675284	0.911302273				Furn_FastRmp	12.02	12.23	12.07	11.31			Furn_FastRmp	684.99	696.93	687.72	644.41	75600	54720		Furn_FastRmp	5696.92	5796.23	5719.64	5359.43	628750.12	455095.33		Furn_FastRmp	6164.91	6272.38	6189.49	5799.69	680400.00	492480.00																																																															
				Furn_Nitr	2.31	3	0.62	0.162	0.81	0.21			Furn_Nitr	0.019792973	0.12065	0.022267014	0.11849	0.022267014	0.11634	0.024741698	0.10126		Furn_Nitr	0.045807255	0.27921239	0.051532976	0.274225367	0.051532976	0.26923964	0.057260185	0.234338253		Furn_Nitr	0.059378918	0.361936763	0.066801041	0.355472196	0.066801041	0.34900931	0.074225095	0.303767424				Furn_Nitr	12.02	12.23	12.07	11.31			Furn_Nitr	684.99	696.93	687.72	644.41	75600	54720		Furn_Nitr	1585.28	1612.92	1591.61	1491.37	174962.53	126639.54		Furn_Nitr	2054.97	2090.79	2063.16	1933.23	226800.00	164160.00																																																															
				Furn_OxAn	13.10	14	3.54	0.917	3.78	0.98			Furn_OxAn	0.019792973	0.12065	0.022267014	0.11849	0.022267014	0.11634	0.024741698	0.10126		Furn_OxAn	0.25921006	1.579982489	0.291610265	1.551762359	0.291610265	1.523549565	0.324018894	1.326052671		Furn_OxAn	0.277101616	1.689038227	0.311738192	1.658870249	0.311738192	1.628710112	0.346383774	1.417581314				Furn_OxAn	12.02	12.23	12.07	11.31			Furn_OxAn	684.99	696.93	687.72	644.41	75600	54720		Furn_OxAn	8970.67	9127.05	9006.44	8439.24	990062.53	716616.69		Furn_OxAn	9589.86	9757.03	9628.10	9021.74	1058400.00	766080.00																																																															
				Furn_OxAn(I)	3.94	4	1.06	0.276	1.08	0.28			Furn_OxAn(I)	0.019792973	0.12065	0.022267014	0.11849	0.022267014	0.11634	0.024741698	0.10126		Furn_OxAn(I)	0.078026614	0.475601461	0.087779624	0.467106725	0.087779624	0.458614196	0.097535169	0.39916429		Furn_OxAn(I)	0.07917189	0.482582351	0.089068055	0.473962928	0.089068055	0.465345746	0.098966793	0.405023233				Furn_OxAn(I)	12.02	12.23	12.07	11.31			Furn_OxAn(I)	684.99	696.93	687.72	644.41	75600	54720		Furn_OxAn(I)	2700.32	2747.40	2711.09	2540.35	298025.57	215713.75		Furn_OxAn(I)	2739.96	2787.72	2750.88	2577.64	302400.00	218880.00																																																															
				Furn_Poly	2.31	3	0.62	0.161	0.81	0.21			Furn_Poly	0.019792973	0.12065	0.022267014	0.11849	0.022267014	0.11634	0.024741698	0.10126		Furn_Poly	0.045660338	0.278316875	0.051367694	0.273345846	0.051367694	0.26837611	0.057076535	0.233586662		Furn_Poly	0.059378918	0.361936763	0.066801041	0.355472196	0.066801041	0.34900931	0.074225095	0.303767424				Furn_Poly	12.02	12.23	12.07	11.31			Furn_Poly	684.99	696.93	687.72	644.41	75600	54720		Furn_Poly	1580.20	1607.75	1586.50	1486.59	174401.37	126233.37		Furn_Poly	2054.97	2090.79	2063.16	1933.23	226800.00	164160.00																																																															
				Furn_TEOS	2.30	3	0.62	0.161	0.81	0.21			Furn_TEOS	0.019792973	0.12065	0.022267014	0.11849	0.022267014	0.11634	0.024741698	0.10126		Furn_TEOS	0.045559402	0.277701636	0.051254143	0.272741596	0.051254143	0.267782846	0.056950363	0.233070302		Furn_TEOS	0.059378918	0.361936763	0.066801041	0.355472196	0.066801041	0.34900931	0.074225095	0.303767424				Furn_TEOS	12.02	12.23	12.07	11.31			Furn_TEOS	684.99	696.93	687.72	644.41	75600	54720		Furn_TEOS	1576.71	1604.19	1582.99	1483.30	174015.84	125954.32		Furn_TEOS	2054.97	2090.79	2063.16	1933.23	226800.00	164160.00																																																															
				Implant_HiE	1.87	2	1.52	0.393	1.62	0.42			Implant_HiE	0.07917189	0.30161	0.089068055	0.29623	0.089068055	0.29084	0.098966793	0.25314		Implant_HiE	0.148225084	0.564679659	0.166752618	0.554593894	0.166752618	0.54451075	0.185284969	0.47392612		Implant_HiE	0.158343781	0.603227938	0.17813611	0.59245366	0.17813611	0.581682183	0.197933585	0.506279041				Implant_HiE	34.50	35.58	35.17	33.83			Implant_HiE	1966.32	2027.90	2004.88	1928.34	441000	319200		Implant_HiE	3681.33	3796.62	3753.52	3610.22	825637.26	597604.11		Implant_HiE	3932.64	4055.80	4009.76	3856.68	882000.00	638400.00																																																															
				Implant_LoE	3.29	4	2.67	0.691	3.24	0.84			Implant_LoE	0.07917189	0.36194	0.089068055	0.35547	0.089068055	0.34901	0.098966793	0.30377		Implant_LoE	0.260559833	1.191157395	0.293128754	1.169882086	0.293128754	1.148612307	0.325706143	0.999718324		Implant_LoE	0.316687561	1.447747052	0.35627222	1.421888785	0.35627222	1.396037239	0.395867171	1.215069698				Implant_LoE	39.02	40.02	39.54	37.63			Implant_LoE	2224.20	2281.18	2253.55	2144.77	252000	182400		Implant_LoE	7319.98	7507.50	7416.57	7058.58	829348.37	600290.25		Implant_LoE	8896.80	9124.70	9014.19	8579.09	1008000.00	729600.00																																																															
				Insp_PLY	24.60	25	19.92	5.165	20.25	5.25			Insp_PLY	0.039585945	0.30161	0.044534027	0.29623	0.044534027	0.29084	0.049483396	0.25314		Insp_PLY	0.973628089	7.418285233	1.095327645	7.285786948	1.095327645	7.153323104	1.217058844	6.226041755		Insp_PLY	0.989648629	7.540349229	1.113350687	7.405670753	1.113350687	7.271027286	1.237084909	6.328488008				Insp_PLY	28.56	28.90	28.49	26.41			Insp_PLY	1627.86	1647.14	1624.11	1505.25	37800	27360		Insp_PLY	40037.69	40511.79	39945.51	37022.18	929702.24	672927.33		Insp_PLY	40696.49	41178.39	40602.79	37631.36	945000.00	684000.00																																																															
				Insp_Visual	0.99	1	0.13	0.035	0.14	0.035			Insp_Visual	0.039585945	0.60323	0.044534027	0.59245	0.044534027	0.58168	0.049483396	0.50628		Insp_Visual	0.039042621	0.59494853	0.04392279	0.584322131	0.04392279	0.573698494	0.048804228	0.499330273		Insp_Visual	0.039585945	0.603227938	0.044534027	0.59245366	0.044534027	0.581682183	0.049483396	0.506279041				Insp_Visual	51.18	51.11	50.31	45.39			Insp_Visual	2917.26	2913.51	2867.46	2587.43	37800	27360		Insp_Visual	2877.22	2873.52	2828.10	2551.91	37281.19	26984.48		Insp_Visual	2917.26	2913.51	2867.46	2587.43	37800.00	27360.00																																																															
				Litho_248	3.45	4	8.39	2.174	9.72	2.52			Litho_248	0.039585945	0.30161	0.044534027	0.29623	0.044534027	0.29084	0.049483396	0.25314		Litho_248	0.136615239	1.040901368	0.153691589	1.022309788	0.153691589	1.00372304	0.170772379	0.873610973		Litho_248	0.158343781	1.206455877	0.17813611	1.18490732	0.17813611	1.163364366	0.197933585	1.012558081				Litho_248	28.56	28.90	28.49	26.41			Litho_248	1627.86	1647.14	1624.11	1505.25	157500	114000		Litho_248	5617.91	5684.44	5604.98	5194.79	543548.98	393425.93		Litho_248	6511.44	6588.54	6496.45	6021.02	630000.00	456000.00																																																															
				Litho_I	10.02	11	16.23	4.207	17.82	4.62			Litho_I	0.039585945	0.30161	0.044534027	0.29623	0.044534027	0.29084	0.049483396	0.25314		Litho_I	0.396564953	3.021515062	0.446133961	2.967547662	0.446133961	2.91359429	0.495715858	2.535906661		Litho_I	0.435445397	3.317753661	0.489874302	3.258495131	0.489874302	3.199252006	0.54431736	2.784534724				Litho_I	28.56	28.90	28.49	26.41			Litho_I	1627.86	1647.14	1624.11	1505.25	126000	91200		Litho_I	16307.61	16500.71	16270.06	15079.37	1262245.57	913625.37		Litho_I	17906.46	18118.49	17865.23	16557.80	1386000.00	1003200.00																																																															
				Litho_Iw	10.74	11	14.50	3.760	14.85	3.85			Litho_Iw	0.039585945	0.30161	0.044534027	0.29623	0.044534027	0.29084	0.049483396	0.25314		Litho_Iw	0.42527977	3.240299526	0.478438013	3.182424408	0.478438013	3.124564334	0.531610078	2.719528774		Litho_Iw	0.435445397	3.317753661	0.489874302	3.258495131	0.489874302	3.199252006	0.54431736	2.784534724				Litho_Iw	28.56	28.90	28.49	26.41			Litho_Iw	1627.86	1647.14	1624.11	1505.25	126000	91200		Litho_Iw	17488.42	17695.51	17448.16	16171.25	1353643.34	979779.94		Litho_Iw	17906.46	18118.49	17865.23	16557.80	1386000.00	1003200.00																																																															
				Meas_CD	14.72	15	5.96	1.546	6.08	1.575			Meas_CD	0.039585945	0.18097	0.044534027	0.17774	0.044534027	0.17450	0.049483396	0.15188		Meas_CD	0.582839513	2.66446899	0.655692084	2.616878804	0.655692084	2.569300989	0.728563598	2.236243912		Meas_CD	0.593789177	2.714525722	0.668010412	2.666041471	0.668010412	2.617569823	0.742250945	2.278255683				Meas_CD	19.51	20.01	19.77	18.81			Meas_CD	1112.10	1140.59	1126.77	1072.39	37800	27360		Meas_CD	16373.88	16793.32	16589.93	15789.16	556544.34	402832.09		Meas_CD	16681.49	17108.82	16901.60	16085.79	567000.00	410400.00																																																															
				Meas_Film	11.81	12	2.23	0.579	2.27	0.588			Meas_Film	0.039585945	0.18097	0.044534027	0.17774	0.044534027	0.17450	0.049483396	0.15188		Meas_Film	0.467688936	2.138054541	0.526148153	2.099866665	0.526148153	2.061688715	0.58462257	1.794433138		Meas_Film	0.475031342	2.171620578	0.53440833	2.132833177	0.53440833	2.094055858	0.593800756	1.822604546				Meas_Film	19.51	20.01	19.77	18.81			Meas_Film	1112.10	1140.59	1126.77	1072.39	37800	27360		Meas_Film	13138.92	13475.50	13312.29	12669.72	446588.85	323245.26		Meas_Film	13345.20	13687.05	13521.28	12868.63	453600.00	328320.00																																																															
				Meas_Overlay	10.31	11	2.78	0.722	2.97	0.77			Meas_Overlay	0.039585945	0.18097	0.044534027	0.17774	0.044534027	0.17450	0.049483396	0.15188		Meas_Overlay	0.408050783	1.865416866	0.459055473	1.832098582	0.459055473	1.798788958	0.510073425	1.565612932		Meas_Overlay	0.435445397	1.990652196	0.489874302	1.955097079	0.489874302	1.919551203	0.54431736	1.670720834				Meas_Overlay	19.51	20.01	19.77	18.81			Meas_Overlay	1112.10	1140.59	1126.77	1072.39	37800	27360		Meas_Overlay	11463.49	11757.15	11614.75	11054.12	389641.31	282026.09		Meas_Overlay	12233.10	12546.47	12394.51	11796.24	415800.00	300960.00																																																															
				PVD_Met	1.13	2	1.22	0.315	2.16	0.56			PVD_Met	0.019792973	0.30161	0.022267014	0.29623	0.022267014	0.29084	0.024741698	0.25314		PVD_Met	0.022288444	0.33964106	0.025074409	0.333574718	0.025074409	0.327509952	0.027861099	0.285055017		PVD_Met	0.039585945	0.603227938	0.044534027	0.59245366	0.044534027	0.581682183	0.049483396	0.506279041				PVD_Met	25.59	25.56	25.15	22.70			PVD_Met	1458.63	1456.75	1433.73	1293.71	157500	114000		PVD_Met	1642.53	1640.42	1614.49	1456.82	177357.39	128372.97		PVD_Met	2917.26	2913.51	2867.46	2587.43	315000.00	228000.00																																																															
				PVD_Met(C) 	8.39	9	9.06	2.349	9.72	2.52			PVD_Met(C) 	0.019792973	0.30161	0.022267014	0.29623	0.022267014	0.29084	0.024741698	0.25314		PVD_Met(C) 	0.1660747	2.530718879	0.186833363	2.485517609	0.186833363	2.440328089	0.207597423	2.123989698		PVD_Met(C) 	0.178136753	2.714525722	0.200403124	2.666041471	0.200403124	2.617569823	0.222675284	2.278255683				PVD_Met(C) 	25.59	25.56	25.15	22.70			PVD_Met(C) 	1458.63	1456.75	1433.73	1293.71	157500	114000		PVD_Met(C) 	12238.76	12223.01	12029.83	10855.01	1321517.78	956527.16		PVD_Met(C) 	13127.67	13110.77	12903.56	11643.42	1417500.00	1026000.00																																																															
				RTP_OxAn(C) 	2.42	3	0.98	0.254	1.22	0.315			RTP_OxAn(C) 	0.019792973	0.12065	0.022267014	0.11849	0.022267014	0.11634	0.024741698	0.10126		RTP_OxAn(C) 	0.047851253	0.291671324	0.053832465	0.286461771	0.053832465	0.281253572	0.059815232	0.244794826		RTP_OxAn(C) 	0.059378918	0.361936763	0.066801041	0.355472196	0.066801041	0.34900931	0.074225095	0.303767424				RTP_OxAn(C) 	12.02	12.23	12.07	11.31			RTP_OxAn(C) 	684.99	696.93	687.72	644.41	126000	91200		RTP_OxAn(C) 	1656.02	1684.89	1662.63	1557.92	304616.09	220484.02		RTP_OxAn(C) 	2054.97	2090.79	2063.16	1933.23	378000.00	273600.00																																																															
				Test	21.03	22	5.68	1.472	5.94	1.54			Test	0.098964863	0.12065	0.111335069	0.11849	0.111335069	0.11634	0.123708491	0.10126		Test	2.0814228	2.537410446	2.341592194	2.492089657	2.341592194	2.44678065	2.601829235	2.129605817		Test	2.177226983	2.654202928	2.449371511	2.606796105	2.449371511	2.559401605	2.7215868	2.227627779				Test	23.89	25.59	25.43	26.15			Test	1361.91	1458.46	1449.25	1490.58	37800	27360		Test	28643.59	30674.30	30480.60	31349.70	795007.23	575433.81		Test	29962.01	32086.18	31883.57	32792.68	831600.00	601920.00																																																															
				VP_HF_Clean	4.35	5	0.94	0.244	1.08	0.28			VP_HF_Clean	0.039585945	0.18097	0.044534027	0.17774	0.044534027	0.17450	0.049483396	0.15188		VP_HF_Clean	0.172391235	0.788091899	0.193939439	0.774015759	0.193939439	0.759943277	0.215493245	0.661432247		VP_HF_Clean	0.197929726	0.904841907	0.222670137	0.88868049	0.222670137	0.872523274	0.247416982	0.759418561				VP_HF_Clean	19.51	20.01	19.77	18.81			VP_HF_Clean	1112.10	1140.59	1126.77	1072.39	100800	72960		VP_HF_Clean	4843.04	4967.10	4906.94	4670.09	438969.85	317730.56		VP_HF_Clean	5560.50	5702.94	5633.87	5361.93	504000.00	364800.00																																																															
				Wet_Bench	10.65	11	5.75	1.491	5.94	1.54			Wet_Bench	0.039585945	0.18097	0.044534027	0.17774	0.044534027	0.17450	0.049483396	0.15188		Wet_Bench	0.421469106	1.926759146	0.474151032	1.892345225	0.474151032	1.857940249	0.526846655	1.617096474		Wet_Bench	0.435445397	1.990652196	0.489874302	1.955097079	0.489874302	1.919551203	0.54431736	1.670720834				Wet_Bench	19.51	20.01	19.77	18.81			Wet_Bench	1112.10	1140.59	1126.77	1072.39	157500	114000		Wet_Bench	11840.46	12143.77	11996.69	11417.63	1676892.74	1213750.94		Wet_Bench	12233.10	12546.47	12394.51	11796.24	1732500.00	1254000.00																																																															
				Wet_Bench(I)	9.22	10	4.98	1.291	5.40	1.4			Wet_Bench(I)	0.039585945	0.18097	0.044534027	0.17774	0.044534027	0.17450	0.049483396	0.15188		Wet_Bench(I)	0.365067911	1.668919328	0.410699917	1.639110694	0.410699917	1.609309809	0.456343787	1.400695861		Wet_Bench(I)	0.395859452	1.809683815	0.445340275	1.777360981	0.445340275	1.745046549	0.494833964	1.518837122				Wet_Bench(I)	19.51	20.01	19.77	18.81			Wet_Bench(I)	1112.10	1140.59	1126.77	1072.39	157500	114000		Wet_Bench(I)	10255.96	10518.68	10391.28	9889.71	1452490.16	1051326.21		Wet_Bench(I)	11121.00	11405.88	11267.73	10723.86	1575000.00	1140000.00																																																															
																																																																																																																																									
				Total	289.11	312	180.37	46.76	196.13	50.85													Total Number of Engineer/Technicians	84.33	178.29	90.15	186.43	92.40	202.32	96.98	206.32		Total Number of Engineer/Technicians	85.05	183.09	90.96	191.14	93.21	206.95	97.88	210.35																			Total Annual Space Cost (fractional tools)	1733184.51	1809823.19	1891698.77	1936034.63	29026046.91	21009329.19		Total Annual Space Cost (integer tools)	1759851.76	1836893.95	1918403.32	1960945.65	31676400.00	22927680.00																																																															
																																																												Total Direct					50035376.10			Total Direct					54604080.00																																																																
					Equipment Cost per Wafer																																																																																																																																				
							Fractional Tools		Integer Tools																																																			Space Cost per Wafer	level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)				Space Cost per Wafer	level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)																																																																	
							tool depreciation	tool maintenance	tool depreciation	tool maintenance																																																		Fractional Tools								Integer tools																																																																					
						$/wafer	601.25	155.88	653.76	169.49																																																		Direct Space	170.1883541	170.1883541	170.1883541	170.1883541				Direct Space	185.7281633	185.7281633	185.7281633	185.7281633																																																																	
																																																												Indirect Space	5.895185419	6.155861184	6.434349559	6.585151799				Indirect Space	5.985890338	6.247938604	6.525181374	6.669883166																																																																	
																			Personnel Type					Number of Personnel by type (fractional tools)						Rounding up the Number of personnel (fractional tools)						Annual Cost per Personnel Type																								Total Space Cost	176.0835395	176.3442153	176.6227036	176.7735059				Total Space Cost	191.7140536	191.9761019	192.2533446	192.3980464																																																																	
																		Level (0,0)	Operator	Supervisor	Manager	Overhead staff		Personnel	level 0	level 1	level1,5	level2		Personnel	level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)		Personnel	Salary	level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)																																																																																																
																		Fixed	273	16	15	8		Operator	511	410	366	285		Operator	511	410	366	285		Operator	60000	30660000	24600000	21960000	17100000																																																																																																
																		Per wafer start/month	0.0095	0.00057		0.0002494		Supervisor	30	25	22	17		Supervisor	31	25	23	17		Supervisor	80000	2480000	2000000	1840000	1360000																																																																																																
																		Total Number	510.5	30.25	15	14.24		Manager	15	15	15	15		Manager	15	15	15	15		Manager	125000	1875000	1875000	1875000	1875000																																																																																																
																								Overhead staff	14	13	13	11		Overhead staff	15	14	13	12		Overhead staff	70000	1050000	980000	910000	840000																																																																																																
																								Engineer	84	90	92	97		Engineer	85	91	93	97		Engineer	125000	10625000	11375000	11625000	12125000																																																																																																
																		Level (1,1)	Operator	Supervisor	Manager	Overhead staff		Technicians	178	186	202	206		Technicians	179	187	203	207		Technicians	70000	12530000	13090000	14210000	14490000																																																																																																
																		Fixed	220	13	15	8														Total Direct		45670000	39690000	38010000	32950000																																																																																																
																		Per wafer start/month	0.0076	0.00046		0.00021220														Total Indirect		13550000	14230000	14410000	14840000																																																																																																
																		Total Number	410	24.5	15	13.31														Total Personnel		59220000	53920000	52420000	47790000																																																																																																
																																																																																																																																									
																								Number of Personnel by type (Integer tools)						Rounding up the Number of personnel (integer tools)						Annual Cost per Personnel Type																																																																																																					
																		Level (1.5,1.5)	Operator	Supervisor	Manager	Overhead staff		Personnel	level 0	level 1	level1,5	level2		Personnel	level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)		Personnel	Salary	level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)																																																																																																
																		Fixed	211	13	15	8		Operator	511	410	366	285		Operator	511	410	366	285		Operator	60000	30660000	24600000	21960000	17100000																																																																																																
																		Per wafer start/month	0.0062	0.00037		0.0001874		Supervisor	30	25	22	17		Supervisor	31	25	23	17		Supervisor	80000	2480000	2000000	1840000	1360000																																																																																																
																		Total Number	366	22.25	15	12.69		Manager	15	15	15	15		Manager	15	15	15	15		Manager	125000	1875000	1875000	1875000	1875000																																																																																																
																								Overhead staff	14	13	13	11		Overhead staff	15	14	13	12		Overhead staff	70000	1050000	980000	910000	840000																																																																																																
																								Engineer	85	91	93	98		Engineer	86	91	94	98		Engineer	125000	10750000	11375000	11750000	12250000																																																																																																
																		Level (2,2)	Operator	Supervisor	Manager	Overhead staff		Technicians	183	191	207	210		Technicians	184	192	207	211		Technicians	70000	12880000	13440000	14490000	14770000																																																																																																
																		Fixed	200	12	15	8														Total Direct		46020000	40040000	38290000	33230000																																																																																																
																		Per wafer start/month	0.0034	0.0002		0.0001320														Total Indirect		13675000	14230000	14535000	14965000																																																																																																
																		Total Number	285	17	15	11.3														Total Personnel		59695000	54270000	52825000	48195000																																																																																																
																																																																																																																																									
																																																																																																																																									
																																																																																																																																									
																																																																																																																																									
																																																																																																																																									
																																				Personnel Cost per wafer																																																																																																					
																																						level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)																																																																																																
																																				Fractional Tools																																																																																																					
																																				Direct Personnel		155.34	135.00	129.29	112.07																																																																																																
																																				Indirect Personnel		46.09	48.40	49.01	50.48																																																																																																
																																				total		201.43	183.40	178.30	162.55																																																																																																
																																				Integer Tools																																																																																																					
																																				Direct Personnel		156.53	136.19	130.24	113.03																																																																																																
																																				Indirect Personnel		46.51	48.40	49.44	50.90																																																																																																
																																				total		203.04	184.59	179.68	163.93																																																																																																
																																																																																																																																									


Total Cost

Expense-Related Costs	Cost per Wafer	Levels of Automation(using fractional tools)				Levels of Automation(using Integer tools)								
	Cost Components	level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)	level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)					
	Tool Depreciation	601.25	601.25	601.25	601.25	653.76	653.76	653.76	653.76					
	Tool Maintenance	155.88	155.88	155.88	155.88	169.49	169.49	169.49	169.49					
	Tool Leasing	0.00	0.00	0.00	0.00	0.00	0.00	0.00	0.00					
	Direct Personnel	155.34	135.00	129.29	112.07	156.53	136.19	130.24	113.03					
	Indirect Personnel	46.09	48.40	49.01	50.48	46.51	48.40	49.44	50.90					
	Direct Space	170.19	170.19	170.19	170.19	185.73	185.73	185.73	185.73					
	Indirect Space	5.90	6.16	6.43	6.59	5.99	6.25	6.53	6.67					
	Direct Material	200.00	200.00	200.00	200.00	200.00	200.00	200.00	200.00					
	Indirect Material	0.00	0.00	0.00	0.00	0.00	0.00	0.00	0.00					
	Cost Centers	0.00	0.00	0.00	0.00	0.00	0.00	0.00	0.00					
	Facilities	0.00	0.00	0.00	0.00	0.00	0.00	0.00	0.00					
	CIM System	0.00	0.00	0.00	0.00	0.00	0.00	0.00	0.00					
	Control Units	0.00	0.00	0.00	0.00	0.00	0.00	0.00	0.00					
	Total Cost	1334.64	1316.87	1312.05	1296.45	1418.01	1399.82	1395.18	1379.58					
														
														
Total die produced over the factory life														
	TD=	1410144.617												
														
														
														
Expense Cost per Die														
		Fractional tools				Integer tools								
	Automation Level	level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)	level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)					
	Expense Cost per wafer(worksheet "ExpenseCost")	1334.64	1316.87	1312.05	1296.45	1418.01	1399.82	1395.18	1379.58					
														
	EPY=	400392377.9	395062417.3	393615351.6	388936102.5	425403529.1	419946429.2	418555112.3	413874033					
														
	EPD=	1419.69	1400.79	1395.66	1379.06	1508.37	1489.02	1484.09	1467.49					
														
Delay Cost per Die														
	TDC=	965419560.4												
														
	DCPD=	684.62												
														
TOTAL COST PER DIE														
		Fractional tools				Integer tools								
	Automation Level	level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)	level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)					
	TCPD=	2104.31	2085.41	2080.28	2063.69	2192.99	2173.64	2168.71	2152.11					
														
FINAL RESULT														
														
		Fractional tools				Integer tools								
	Automation Level	level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)	level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)					
	Expense Over Life	2001961889	1975312087	1968076758	1944680512	2127017645	2099732146	2092775561	2069370165					
	EPW=	1334.64126	1316.874724	1312.051172	1296.453675	1418.011764	1399.821431	1395.183708	1379.58011					
	EPD=	1419.69	1400.79	1395.66	1379.06	1508.37	1489.02	1484.09	1467.49					
	Revenue Over Life	6590427149												
	Revenue per Wafer	4393.6181												
	Revenue per Die	4673.58246												
	Total Delay Cost	965419560.4												
	DCPD	684.6245048												
														
			


Number of tools

Tool Requirement						
						
						
			#tools	#tools	tool	tool
		Tool Type	fractional	Round Up	CEE	OEE
		CMP_Ins	2.50	3	0.23	0.191296765
		CMP_Ins(C) 	19.84	20	0.23	0.228217033
		CMP_Ins(I)	2.51	3	0.23	0.192626016
		CMP_Met	12.41	13	0.23	0.21947751
		CVD_Ins	3.50	4	0.64	0.559613727
		CVD_Ins(C) 	9.26	10	0.64	0.592720695
		CVD_Ins(I)	1.08	2	0.64	0.346801092
		CVD_Ins_Thin	1.61	2	0.64	0.514661912
		CVD_Met	1.19	2	0.48	0.28669944
		CVD_Met(C) 	4.75	5	0.48	0.456043229
		CVD_MetW	1.02	2	0.48	0.245724835
		CVD_MetW(C) 	4.07	5	0.48	0.390866292
		Dry_Etch	2.35	3	0.59	0.46269864
		Dry_Etch(A)	2.60	3	0.53	0.45885011
		Dry_Etch(C) 	13.45	14	0.53	0.509141857
		Dry_Etch(I)	6.95	7	0.53	0.526184222
		Dry_Etch_Met	9.67	10	0.59	0.57030747
		Dry_Strip	1.78	2	0.65	0.577795546
		Dry_Strip(D)	1.98	2	0.65	0.643213659
		Dry_Strip(I)	5.32	6	0.65	0.576257152
		Furn_FastRmp	8.32	9	0.5	0.462044474
		Furn_Nitr	2.31	3	0.5	0.385719853
		Furn_OxAn	13.10	14	0.5	0.467716616
		Furn_OxAn(I)	3.94	4	0.5	0.492767152
		Furn_Poly	2.31	3	0.5	0.384482738
		Furn_TEOS	2.30	3	0.5	0.383632812
		Implant_HiE	1.87	2	0.37	0.346355765
		Implant_LoE	3.29	4	0.42	0.34556182
		Insp_PLY	24.60	25	0.3	0.295143567
		Insp_Visual	0.99	1	0.35	0.345196189
		Litho_248	3.45	4	0.8	0.690220928
		Litho_I	10.02	11	0.8	0.728568874
		Litho_Iw	10.74	11	0.8	0.781323717
		Meas_CD	14.72	15	0.35	0.343545887
		Meas_Film	11.81	12	0.35	0.344590163
		Meas_Overlay	10.31	11	0.3	0.281126488
		PVD_Met	1.13	2	0.51	0.287150064
		PVD_Met(C) 	8.39	9	0.51	0.475466715
		RTP_OxAn(C) 	2.42	3	0.57	0.459341718
		Test	21.03	22	0.39	0.37283889
		VP_HF_Clean	4.35	5	0.45	0.391937367
		Wet_Bench	10.65	11	0.54	0.522667868
		Wet_Bench(I)	9.22	10	0.54	0.497996628
		Total Number	289.11	312		0
    
    
    
    
Personnel Requirement    

Personnel Requirement						
						
		Rounding up the Number of personnel (fractional tools)				
		Personnel	level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)
		Operator	511	410	366	285
		Supervisor	31	25	23	17
		Manger	15	15	15	15
		Overhead Staff	15	14	13	12
		Engineer	85	91	93	97
		Techn	179	187	203	207
						
		Rounding up the Number of personnel (integer tools)				
		Personnel	level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)
		Operator	511	410	366	285
		Supervisor	31	25	23	17
		Manger	15	15	15	15
		Overhead Staff	15	14	13	12
		Engineer	86	91	94	98
		Techn	184	192	207	211

    
    
    
    
Phased Capacity    
Expense-Related Costs									
Cost per Wafer		Levels of Automation(using fractional tools)				Levels of Automation(using Integer tools)			
Phase Start Date	Phase InPut	level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)	level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)
0	60000	1406.411547	1383.035715	1379.368285	1364.215912	1543.870298	1520.099925	1516.430435	1501.267988
120	1400000	1334.64126	1316.874724	1312.051172	1296.453675	1418.011764	1399.821431	1395.183708	1379.58011
1800	0								
1800	0								
1800	0								
1800	0								
1800	0								
1800	0								
Sum	1460000	1952882456.16	1926606757.07	1919633737.85	1896888099.60	2077848686.79	2050955998.65	2044243016.75	2021488233.39
									
									
									
Revenue-Related Costs									
									
	Phase Start Date	Capacity	Cycle Time	Output	Revenue				
	0	15000	26.84639237	48086.77044	406057868		Ideal Revenue		7555846710
	120	25000	26.84639237	1330000	5913664036				
	0	0		0	0		Total Delay Cost		1236124806
	0	0		0	0				
	0	0		0	0		Delay Cost Per Die		896.9861929
	0	0		0	0				
	0	0		0	0				
	0	0		0	0				
	Sum	25000		1378086.77	6319721904				
									
									
									
Expense Cost per Die									
									
		fractional tools				Integer tools			
	Automation Level	level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)	level (0,0)	level (1,1)	level (1.5,1.5)	level (2,2)
	Expense Cost per wafer(worksheet "ExpenseCost")	1337.59	1319.59	1314.82	1299.24	1423.18	1404.76	1400.17	1384.58
									
	EPY=	390576491.2	395878100.8	394445288.6	389771527.3	426955209.6	421429314.8	420049934.9	415374294.5
									
	EPD=	1417.10	1398.03	1392.97	1376.46	1507.78	1488.26	1483.39	1466.88
	TCPD=	2314.08	2295.02	2289.96	2273.45	2404.76	2385.25	2380.38	2363.87
    
    
    
    
    
    
    
    





			
