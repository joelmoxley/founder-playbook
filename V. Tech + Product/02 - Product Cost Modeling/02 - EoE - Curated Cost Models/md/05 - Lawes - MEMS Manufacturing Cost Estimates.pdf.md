Here's an example of a description that appears under a link.

15 MIN READ || Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Credit: [R. A. Lawes]

{! search-content: !}

Microsyst Technol (2007) 13:85–95
DOI 10.1007/s00542-006-0252-6
TECHNICAL PAPER
Manufacturing costs for microsystems/MEMS using high aspect ratio microfabrication techniques
R. A. Lawes

Received: 11 June 2006 / Accepted: 14 August 2006 / Published online: 22 September 2006
 Springer-Verlag 2006


Abstract The emphasis on high aspect ratio micromachining techniques for microsystems/MEMS has been mainly to achieve novel devices with, for example, high sensing or actuation performance. Often these utilize deep structures (100–1,000 lm) with vertical wall layers but with relatively modest spatial resolution (1–10 lm). As these techniques move from research to industrial manufacture, the capital cost of the equipment and the cost of device manufacture become important, particularly where more than one micromachining technique can meet the performance requirements. This paper investigates the layer-processing costs associated with the principal high aspect ratio micromachining techniques used in microsystems/MEMS fabrication, particularly silicon surface micromachining, wet bulk etching, wafer bonding, Deep Reactive Ion Etching, excimer laser micromachining, UV LIGA and X-ray LIGA. A cost model (MEMS COST) has been developed which takes the financial, operational and machine-dependent parameters of the different manufacturing techniques as inputs and calculates the layer-processing costs at the wafer and chip level as a function of demand volume. The associated operational and investment costs are also calculated. Cost reductions through increases in the wafer size and decreases in chip area are investigated, and the importance of packaging costs demonstrated.

R. A. Lawes (&)
Optical and Semiconductor Devices Section,
Department of Electrical and Electronic Engineering,
Imperial College, Exhibition Road,
London SW7 2BT, UK
e-mail: ronlawes@sachseln.plus.com

1 Introduction

Thin film techniques are currently being used to fabricate the sensors and actuators made possible by microsystems design. Such devices, while often limited in performance, have the significant advantages of using well-established and cost-effective manufacturing techniques, derived directly from the semiconductor industry and based predominately on silicon. As the semiconductor industry investment cycle seeks improvements in performance and functionality through reduced feature size and larger wafers to spread the fabrication costs over more devices, high quality equipment and often whole facilities become obsolescent. Yet these are more than adequate for MEMS device manufacture. For example, as the semiconductor industry moves from 0.35/0.25 lm processes on 150 mm diameter wafers to sub-100 lm processes on 300 mm wafers, the MEMS industry builds mixed MEMS/CMOS devices using sub-micron processes on 150 and 200 mm wafers.

However, these techniques are effectively planar and many advanced sensor designs require thicker structures to get adequate sensor sensitivity or actuator force. Microsystems are not only being fabricated from thin film techniques at thicknesses of a few microns in silicon but also from deep structures of several hundreds of microns, with high aspect ratios greater than 10:1. These are often made from materials other than silicon (for example polymers, metals and ceramics).

Little work has been published to compare MEMScost models with the robust models that have been developed and verified for semiconductor technology. The introduction of high aspect ratio microengineering techniques will require a different cost structure.

86 Microsyst Technol (2007) 13:85–95

A MEMS cost model (MEMSCOST) has been developed to examine different aspects of microfabri cation. It assumes each machine processes one layer of a wafer per sequence and includes exposure, alignment, wafer loading and other overheads. Costs for masks and resist processes (consisting of resist spinning, pre-bake, development and post-bake) are included, where appropriate, as part of the process. The results presented in this paper concentrate on high aspect ratio lithography techniques and exclude the cost of using the patterned resist structures. However, the model may be readily extended to include various forms of material deposition. Batching of wafers for resist processing is assumed when sufficient volume is demanded. Direct- and indirect-fixed and variable costs are included in the model parameters.

The capital investment required will influence strongly the cost-of-entry for a manufacturing facility and will depend on the output capacity required of the various high aspect ratio equipments. Capital investment will increase as the number of machines required to meet the production requirements rises. As expected, the initial equipment cost will be high, while the unit costs per wafer and hence per chip will fall with volume. 

The model enables the effect of larger wafer sizes and smaller chip areas on manufacturing costs to be estimated. The overall cost of a device will include test (not addressed in this paper) and packaging. There is a brief analysis of packaging costs, although packaging technology for MEMS is still embryonic with little standardization. A typical calculation shows that packaging can be greater than 50% of the cost of a device, even using standardized packages from the semiconductor industry.

The selling price of a device will depend not only on the technology but also the accounting methods used to take account of R&D, marketing and sales, build ings and profit. These costs are not included in the model but may be introduced from available data as fixed cost overheads.

The performance and cost estimates for the various technologies presented in this paper are based on the author’s 27 years experience in constructing and oper ating the Central Microstructure Facility (Lawes 2003) at the Rutherford Appleton Laboratory in the UK. 2 Cost model for microfabrication The manufacturing algorithm within MEMSCOST has been developed on a conventional fixed plus a demand-dependent variable cost basis. The model inputs machine-dependent, operational and financial data to determine the output costs as a function of the number of wafer layers and the number of chips per layer. The manufacturing cost of a complete multilayer wafer or device chip may be calculated from the sum of the layer-processing steps and the overall yield of the processes. The model typically inputs:

Device data
* Number of different designs/year and the number of layers processed with a given technology (hence the number of masks/year).
* Depth of a given high aspect ratio layer.
* Device dimensions (mm · mm) 

Wafer data
* Wafer diameter (e.g. 150 mm)
* Batch size for processes such as resist processing and wet etching (e.g. 20)
* Cost of blank wafer (e.g. $25) Operational details
* Hours/year for facility operation (e.g. 6,000) per operator (e.g. 1,600).
* Number of machines/operator (e.g. 5)

Financial assumptions
* Amortization period (e.g. 5 years)
* Mask cost (each) (e.g. $700)
* Salaries/operator (e.g. $56K)

Layer processing technology
* Cost of capital equipment including cost-of-own ership items such as care and custody, maintenance, consumables and manpower.
* Exposure/etching rate of the process for a given material (wafers/h).
* Cost/h of a particular technology to process a layer, hence the cost/wafer.
* The maximum number of exposed layers/year per machine.
* The yield of good chips for each layer from a given process technology.

The cost to process a layer for each technology is calculated, where relevant, from the exposure or etching process, the resist processing (spinning, prebaking, development and post-baking) and any optical lithography. The cost of masks, any thin layer optical lithography, the high aspect ratio layer-processing steps and the number of machines required to meet the output demand can be summarized to produce the average manufacturing costs for a varying number of wafers/year for a given technology. The algorithms used to calculate the results are:

Microsyst Technol (2007) 13:85–95 87


CL = CF + CVNL (1)
where
CL cost to process a layer ($ per layer)
CF fixed cost ($ per annum)
CV variable cost ($ per wafer layer)
NL number of wafer layers per year, i.e. number of wafers · number of layers/wafer.

The unit cost to process a layer will be
CL = CF/NL + CV: (2)

The fixed costs/year are calculated from the capital cost of the relevant machines (CM), the period (Y) over which amortization is calculated and the annual cost of any scheduled maintenance periods and stand-by consumables (MF), i.e.

CF = CM/Y + MF (3)

The variable costs/year are calculated from the hourly cost of operating the equipment (COP), the time to process a layer (TL) and the cost of throughput dependent consumables (c) per wafer.

CV = COP TL + c (4)

TL is strongly dependent on the physical mechanisms of resist exposure and material etching for a given technology, as well as the method of covering the substrate with adequate exposure, e.g. full wafer projection, wafer scanning or step-and-repeat:

TL = NF(TEXP + TSR) + TO; (5)

where
NF number of fields/wafer (depends on field size and wafer size)
TEXP exposure/etch time depending on the depth (H) of the layer being processed
TSR step-and-repeat time per field
TO other overheads, e.g. load/unload time.

For full wafer projection or wafer scanning, NF = 1, TSR = 0.


3 High aspect ratio machine performance

High aspect ratio microfabrication technologies operate by different physical mechanisms, offer a different quality of micromachining (such as wall angle and roughness), expose resist at significantly different speeds and may machine material directly. Some techniques are more suitable for, or only applicable to, certain materials.

The techniques investigated in this paper are shown in Fig. 1, and the major features, affecting the cost of manufacture, discussed below. Note that high aspect ratio processes such as Deep Reactive Ion Etching (DRIE) and Bulk micromachining can produce structure in the wafer layer itself, whereas X-ray LIGA and UV LIGA require a resist intermediary. Excimer laser machining might do either, depending on the material. All these processes require some form of mask to define the device’s design features. The time to process a wafer layer to the required depth depends on the machine technology and the degree of automation in substrate handling. Many of the machines process a whole wafer simultaneously, as sub-micron resolution and alignment are rarely required. The exposure time algorithm depends on time taken for the exposing radiation to interact with either the resist or the substrate material. Typical data is shown in Table 1.

Bulk micromachining relies upon the wet chemical etching of materials with preferential crystallographic planes (Elwenspoek and Jansen 1998), such as silicon, and can produce relatively simple devices at very low cost. Inflexibility, due to the few fixed planes and low resolution (50–100 lm) are the main limitations. Cost of ownership is low as the equipments required are simple mask aligners, resist-handling tools and wet etching baths.

Laser micromachining and DRIE are two well established techniques that do not require deep resist exposure and development to form a high aspect ratio structure.

An excimer laser produces a high flux, demagnified optical image of a conventional chrome-on-quartz mask, which normally structures the layer material directly by ablation. Each laser pulse removes an image of part of the mask to a depth of a fraction of a micron, depending on the material being machined (Gower 2001). The area of the mask can then be covered by a synchronized mask-wafer motion to expose the whole wafer surface. The wall angles and roughness in the substrate can be controlled by the illumination flux. However, the maximum exposure rate and flux is set by the maximum energy (Rumsby et al. 1997) and power that the mask can absorb (0.1 J/cm2 and 20W/cm2). Note that laser micromachining can be used both to manufacture deep resist moulds and to directly micromachine a variety of materials.


Fig. 1 High aspect ratio
microfabrication techniques
Table 1 Production throughput for some manufacturing technologies (for H = 200 lm)
Exposure
method
Exposure time TEXP (s) TOH (s) Total Output
(wafers/h)
Maximum
(wafers/year)
X-ray LIGA PMMA Scan wafer T = 46.1 · H0.68 a 1,692 30 1,722 2.09 10,000
X-ray LIGA SU-8 Scan wafer T = 0.06 · H + 2.6a 15 30 45 80 384,000
UV LIGA SU-8 Full wafer T = 1.8 · H – 37 323 30 353 10.2 49,000
Excimer laser (depth/pulse
0.2 lm; laser rate 200 Hz)
Scan wafer T = HÆW2/20,000 400 30 430 8.4 40,000
DRIE (etch rate 10 lm/min) Full wafer T = 6H 1,200 30 1,230 2.9 14,000
Surface micromachining
(lithography only)
Full wafer T = 120 120 10 130 27.7 133,000
Wet bulk micromachining (expose;
wet etch 100 lm/h)
Full wafer T = 120; T = 36H 120; 360 10; 10 160; 370 27.7; 9.7 133,000; 47,000
Wafer bonding Full wafer T = 1,000 1,000 30 1,030 3.5 17,000
Resist processing (deep; thin) Batch; batch T = 9,600; T = 3,600 – – 9,600; 3,600 7.5 20 36,000; 96,000
a Calculated from Lawes and Arthur (2004)



Deep reactive ion etching is a form of plasma etching that requires a conventional lithography step to define features in a masking layer on the surface of the wafer, followed by an alternating series of vertical, submicron etching and sidewall passivation steps (known as the Bosch process) to the required layer depth. The reactive etchant is a fluorine radical, typically derived from a SF6 + O2 gas mixture (Laermer and Urban 2003) followed by a passivation plasma from C4F8 to deposit a protective polymer coating to the previously etched steps.

LIGA using X-rays from a synchrotron (Ehrfeld and Schmidt 1998) was one of the first truly high aspect ratio techniques developed. LIGA utilizes the ability of intermediate energy X-rays (3–10 keV) to penetrate deep resist layers without significant absorption or scattering. While the performance is excellent, offering very high aspect ratios (e.g. 100:1) and deep resists (500–2,000 lm) with good resolution (1–5 lm), the cost is generally prohibitive. LIGA operates by conventional resist exposure through a special mask, and the exposure time is dominated by the type and thickness of the absorbing resist layer. Initially, the LIGA resist was mainly PMMA (poly-methyl-methacrylate), which required 5–10 h exposure at a synchrotron. This has prevented X-ray LIGA becoming a cost-competitive microfabrication technique, but the advent of SU-8 resist, which is 100 times more sensitive to X-rays than PMMA, has reduced the exposure time from hours to minutes. In all cases the X-ray mask is typically gold-on-beryllium, expensive ($7,000–10,000) and available mainly from R&D institutes. For LIGA, the exposure time for a given resist depth is derived from the software used (Lawes and Arthur 2004) and depends on the synchrotron, the beamline design and type of resist to be exposed.

It was soon realized that the SU-8 resist was sensitive to UV radiation (g-line, h-line and i-line) and hence usable with a conventional mask aligner and conventional, commercially available chrome-on-quartz masks (Lee et al. 1995). This has given rise to a cost-competitive technique, commonly known as UV LIGA, which is not only ideal for R&D applications but has also found its way into industrial production. The physical processes and manufacturing performance of UV LIGA (Lawes 2005; Zhang et al. 2004; Chuang et al. 2002) and X-ray LIGA (Griffiths 2004) are now reasonably well understood.

Surface microengineering (Linder et al. 1992) is similar to conventional semiconductor fabrication in that thin films (1–5 lm) of polysilicon are deposited on a silicon dioxide sacrificial layer that can be selectively removed to leave a free-standing structure. Commercial foundry processes exist with up to 3–5 layers of polysilicon. It should be noted that relatively modest, sub-micron semiconductor plants can be adapted or built to produce large MEMS device volumes at minimal cost. Strictly, surface microengineering does not produce a high aspect ratio structure, and device designs must be limited to near-planar options. However, it is useful to compare the costs with those of the high aspect ratio techniques.

Wafer bonding (Schmidt 1998) is included in the cost model as a high aspect ratio process, as it is often used to join several layers of a device. Wafer bonding, using pressure and high temperature, is probably the cheapest way in which two structured layers, typically silicon and/or quartz, can be bonded together, e.g. to form a buried microchannel as part of a device.

The cost of thin film lithography is available in the model to calculate the cost of devices where CMOS like manufacturing processes are included, e.g. where an expensive but high throughput optical stepper is used. An example of such a device is a thin film accelerometer where the electronic signal processing is manufactured on the chip and the proof mass fabricated by a suitable high aspect ratio process, such as DRIE.

A general schematic of the various layer-machining techniques is shown in Fig. 1. Note that the difference in resist thickness can be of the order of 500:1, and that the resist-handling and development times will vary accordingly. The maximum layer thickness that each technique can micromachine is determined by the wall angle (which may be non-vertical by a few degrees) and the tolerances required for the top and bottom dimensions of the microstructure.

The choice of each machining technology will depend on the materials used, the tolerances required for the top and bottom dimensions of different microstructures and the roughness quality of the deep walls. 

Table 1 shows the various aspects that make up the total time to process a wafer layer for the different technologies. Typical values have been chosen to demonstrate the technology, taking into account the operation of the exposure machine and the associated resist technology. The maximum number of wafers per year is calculated, assuming 4,800 h/year are available after maintenance and unscheduled machine break down periods.


4 Financial data

The fixed costs are related to the capital cost of the machine, including amortization, a fixed percentage annual cost for electricity, etc. and annual care and maintenance costs, assuming no output. The variable costs include the manpower cost to convey and monitor wafer processing through the manufacturing facility plus the output-dependent consumables and maintenance.

The cost of masks required per year will depend on the number of different devices manufactured and the number of layers per device. It is assumed that the masks are purchased from commercial mask makers, and hence the cost of masks (CMSK) is a fixed cost in the current model. For small annual volumes of multiple designs, the mask costs will be relatively high and the batch sizes for resist processing less than the maximum.

The cost of resist processing can be treated in an identical manner to the equipment, with fixed and variable components but with the costs based on a batch rather than individual wafer basis. 

As synchrotrons cost $100–500M, are paid for from public funds and are usually owned by academic institutions, special financial costing is necessary if a commercial operation is to be established. Conventional amortization calculations alone are likely to prohibit ‘‘commercial’’ use of a synchrotron, whereas treating the X-rays offered to industry as ‘‘spare capacity’’ can yield a commercially acceptable hourly rate. Such an arrangement will be assumed in the model but with the wafer scanner and clean room subject to normal capital expenditure and amortization.

The commercial rates offered are critical to industry’s ability to use X-ray LIGA and rates between $150 and 1,000 have been quoted. $500/h will be assumed in this cost model. 


5 Microfabrication costs per layer

The cost model requires a number of financial parameters as data input. These include the cost of the machine, the amortization period, fixed and variable costs of both consumables and maintenance to operate the equipment and manpower hourly rates.

Machine-dependent performance parameters include the total time to expose a wafer layer, the wafer diameter, the yield of the process and associated mask costs (optical or X-ray). The maximum number of wafers per annum is then calculated in order to determine the necessary capital investment as demand increases. Device-dependent parameters include the area of the device, the number of layers of a particular technology, and the depth of any high aspect ratio process. Some of these costs will depend on the number of different devices to be fabricated per annum (hence the number of different masks).

For each technology, the costs consist of the fixed and variable costs of the exposure machine, the resist processes and the mask costs. Note that resist costs do not apply to the excimer laser and wafer bonding techniques and mask costs do not apply to wafer bonding.

The annual costs may now be calculated from Equation 1 and the annual unit costs from Eq. 2, by substituting values from Tables 1 and 2 into Eqs. 3–6.

The cost of microfabricating a single layer of a wafer, for a given technology, is shown in Fig. 2, assuming 200 mm diameter substrates and ten different designs per annum (which determines the total annual fixed mask cost).

N.B. for clarity, graph markers above 10,000 wafer layers have been omitted.

As the demand for devices increases, the number of wafer layers that must be processed increases and eventually approaches the maximum number that a single machine can output. There are two consequences.

Firstly, the average time a wafer is queued waiting for machine access increases, until it reaches unacceptable levels. Secondly, in order to avoid this eventuality, an additional machine must be purchased, thus increasing the unit costs in a ‘‘saw tooth’’ manner (often referred to as ‘‘granularity’’). Note that, for the assumptions made for synchrotron costs, X-ray LIGA with SU-8 resist can be cost competitive with DRIE for output in excess of 10,000 wafer levels per year.

Figure 3 illustrates the incremental nature of the necessary capital investment in equipment for each processing technology as the annual demand increases. Even X-ray LIGA with SU-8 resist can require less capital investment for large volumes. Similarly, UV LIGA costs are comparable to silicon surface micro engineering until larger volumes are required, when UV LIGA requires more wafer aligners.

Figure 4 (derived from Eq. 3) shows the reduction of wafer layer-processing costs with volume for the various processing techniques. It is noticeable that the reduction in unit costs is much less significant after about 10,000 wafer layers per year. Figure 4 also illustrates why R&D costs are so high, for example at $1,000–3,000/wafer layer, compared with a high production rate of $6–30/wafer layer.

The number of chips per wafer NW will depend on the wafer area (W) and the device area (A). The unit cost (CUDL) to process an individual layer of a device will then be:

CUDL = CF/NSL + CV / Nchip / QL (6)

Nchip number of chips/wafer (W/A approximately)
QL net yield of good chips for a layer

Figure 5 plots the unit cost per good device layer from Eq. 7 for A = 25 mm2 and the yield QL = 100%, i.e. 1,145 chips on a 200 mm wafer. Figure 5 is perhaps the most important result from the cost model, as it ultimately determines the cost of manufacturing complete, multilayer working devices.

Not surprisingly, the costs for X-ray LIGA with PMMA resist are dominated by the cost of using the expensive synchrotron for several hours to obtain one exposed layer of a wafer. Use of SU-8 resist reduces this component by 85% and enables X-ray LIGA to be more cost effective. Note that, in the cases of UV LIGA, DRIE, Bulk and Surface Micromachining, reducing resist-processing costs would significantly reduce costs. 

The variation in the cost/wafer level is weakly proportional to the depth of the high aspect ratio structure, as shown in Fig. 6. The relative expense depends not only on the capital cost of the equipment but on the exposure rates and ancillary processes (e.g. resist technology) that are required.


6 Device costs

The unit manufacturing cost for a device (CUD) can be estimated by summing the processes for each of the (N) layers that make up the device, taking into account the yield at each layer (which may differ). From Eq. 2, for all layers of a device, 

CUD = 1/Nchip/QNPN 1 ðCULÞN ; (7)


Table 2 Fixed and variable costs for some microfabrication technologies
Technology $ to process a single layer
Fixed costs (CF) Variable costs (CV)
Capital ($) Amortized
(5 years; $/year)
Annual cost
(4% · capital; $/year)
Annual maintenance
(0.05MY; $/year)
Annual total
(cost; $/year)
$/h $/wafer Total (inc. $2/wafer
consumables; $/wafer)
X-ray LIGA PMMA (Scanner only) 1,050,000 210,000 42,000 2,800 254,800 507 242.6 244.6
X-ray LIGA SU-8 (Scanner only) 1,050,000 210,000 42,000 2,800 254,800 507 6.3 8.3
UV LIGA SU-8 218,750 43,750 8,750 2,800 55,300 7 0.68 2.68
Excimer laser 875,000 175,000 35,000 2,800 212,800 7 0.84 4.34a
DRIE 700,000 140,000 28,000 2,800 170,800 7 2.39 5.89a
Surface micromachining
(lithography only)
218,750 43,750 8,750 2,800 55,300 7 0.25 2.25
Wet bulk micromachining 236,250 47,250 9,450 2,800 59,500 7 0.97 2.97
Wafer bonding 134,750 26,950 5,390 2,800 35,140 7 2 4
Resist processing
(deep; thin)
210,000 42,000 8,400 14,000 64,400 7 7 0.93; 0.35 0.93b; 0.35b
Mask costs
Optical aligner 700
Optical stepper 1,500 Per mask – – –
X-ray 3,500
Number of machines = demand/maximum wafers/year
MY man years
a £3.5 additional costs for special gases
b 20 wafers/batch
1


10,000
100,000
1,000,000
10,000,000
100 1,000 10,000 100,000
Number of wafers layers per year
Annual Costs ($)
X-ray LIGA (PMMA) X-ray LIGA (SU-8)
DRIE Excimer
Bulk UV LIGA
Silicon Surface Wafer Bonding
Fig. 2 Cost of microfabrication as output increases (H = 200 lm
for HAR processes)
100,000
1,000,000
10,000,000
100 1,000 10,000 100,000
Number of wafer layers per year
Capital Investment ($)
X-ray LIGA (PMMA) X-ray LIGA (SU-8)
DRIE Excimer
Bulk UV LIGA
Silicon Surface Wafer Bonding
Fig. 3 Capital investment ($) versus annual wafer layer production


where
N number of layers per device
QD probability that a device has all good
layers = Q1Q2Q3ÆÆÆQN = QN
when all layer yields are equal.

Consider a ‘‘three-layer polysilicon’’ surface microengineered technology where the main processes are photolithography with associated resist processing (eight masked layers), deposition of polysilicon, oxide and metal interconnect (ten steps) and pattern etching.

Using Eq. 7, the model predicts a manufacturing cost of $652/wafer, for an output of 10,000 processed wafers/year. Typical chip dimensions of 5 mm · 5 mm enable 1,145 chips to be manufactured at a cost of $0.57/chip at 100% yield or $0.81/chip at 70% yield.


m
n
1
10
100
1,000
10,000
100 1,000 10,000 100,000
Number of wafer layers per year
Cost per wafer layer ($)
X-ray LIGA (PMMA) X-ray LIGA (SU-8)
DRIE Excimer
Bulk UV LIGA
Silicon Surface Wafer bonding
Fig. 4 Fabrication costs ($) per wafer layer versus annual
substrate production (H = 200 lm for HAR processes)
0.001
0.010
0.100
1.000
10.000
100 1,000 10,000 100,000
Number of wafer layers per year
Cost per chip layer ($)
X-ray LIGA (PMMA) X-ray LIGA (SU-8)
DRIE Excimer
Bulk UV LIGA
Silicon Surface Wafer Bonding
Fig. 5 Fabrication costs ($) per device layer (H = 200 lm, chip area = 5 mm · 5 mm) as wafer production increases

These costs may be compared with those for a commercial CMOS/MEMS accelerometer, where the processing electronics and the MEMS device are integrated into a single silicon chip.

For the CMOS process, the masked lithography steps are typically 30% of the total chip manufacturing cost. Assuming a 150 mm wafer line using optical stepper lithography, a chip area of 4.5 mm2, a multilayer CMOS process and large-scale volume (for MEMS at 10,000 wafers/year), the cost model estimates $750/wafer for the signal processing electronics. Introduction of a DRIE process to fabricate the proof mass of the accelerometer is calculated to cost $30 which, along with a blank silicon wafer cost of $20, brings the estimated total processing cost to $800/wafer.

The number of chips (3,697) is calculated by accurately fitting the chip dimensions to the available wafer area. Thus, the cost of the fabricated chip at 100% yield is $0.22/chip and $0.31/chip with 70% yield.

10
100
0 100 200 300 400 500
Height of Microstructure (H mm)
Cost per wafer Layer ($)
X-ray PMMA X-ray SU-8 DRIE
Excimer BULK UV LIGA
Fig. 6 Layer manufacturing costs as a function of the depth of the microstructure at 10,000 wafer levels/year



7 Cost reduction by increasing wafer diameter and reducing chip area

The effect of increasing wafer diameter and decreasing the chip area can be illustrated using the silicon surface microengineered device and the MEMS/CMOS accelerometer outlined in Sect. 6. From a priori reasoning:

Cost=chip ¼K A=WD x (8)

where A = area of the chip (mm2), WD = diameter of the wafer (mm) and K and x are constants, depending on the number of layers, the technology used, financial and operational costs and the annual demand for the device.

According to a report from International Sematech (Goodall et al. 2002), when the wafer area increases by >2, the cost of equipment increases by 30–40% for the same number of wafer starts, i.e. taking into account that newer machines generally have higher throughput. This will be assumed when moving from 150 to 200 mm and from 200 to 300 mm wafer diameters. The exact fitting of the chip dimensions to the available wafer area gives the number of chips/wafer as proportional to WD 2.06 and inversely proportional to the area of the chip (A).

The constants for Eq. 8 are shown in Table 3 for the two worked examples in Sect. 6. Note that the values of K and x are strongly dependent on the cost and performance assumptions. This is illustrated in Fig. 7, where the cost/chip as a function of chip area and wafer diameter, are plotted for the ‘‘30%’’ and ‘‘40%’’ assumptions.

The methodology may be extended to any MEMS device by using the cost model to provide data to Eq. 8 to determine the constant K and x.

Assuming a 30% cost progression with wafer diameter, there is a 20% reduction in $/cm2 from 150 mm wafers (4.5 $/cm2) to 200 mm (3.6 $/cm2) wafers and 33% from 200 to 300 mm (2.4 $/cm2). 

The effect of defect densities on MEMS device yields has not yet been satisfactorily analysed, as it has for semiconductor manufacturing. Neither a suitable model nor the data for a model are available from the literature; hence it will be assumed that the defect density is invariant with wafer diameter.

Table 3 Constants for Eq. 8
Process/device Percentage increase in wafer
cost with WD
30% 40%
K x K x
Three-layer polysilicon 9.9 1.10 4.1 0.92
CMOS/MEMS accelerometer 14.7 1.14 5.8 0.95
5 0
10
15
20
25
30
35
40
45
50
150 200 250 300
Wafer diameter (mm)
Cost per Chip (cents)
2 sq. mm 4.5 sq. mm 10 sq mm
Fig. 7 Cost/chip as function of wafer diameter and chip area for a MEMS/CMOS accelerometer; solid line 30%, dashed line 40% (see text)



8 Device packaging

Packaging presents a problem for microsystem/MEMS devices. Unlike semiconductors that need permanent protection from the environment, many MEMS devices (e.g. pressure and temperature sensors) require exposure to the environment, albeit through specially constructed connections, in order to function. Currently this has led to nonstandard and relatively expensive packages.

Alternatively, devices such as accelerometers are hermetically sealed, using standard ceramic packages developed by the IC industry, e.g. 4.5 · 5 mm, 8-Terminal Ceramic Leadless Chip Carrier (CLCC). With the increasingly low cost of manufacturing the MEMS chips in large volumes, packaging can be the dominant factor in the final cost of the device.

Considering the silicon micromachined, integrated electronics sensor as before, the chip may cost $0.30 on a 150 mm line and the packaging a similar amount. Thus, for a device costing $0.60 to manufacture, excluding testing and other overheads, 50% of the cost lies in packaging. As the cost reductions arising from increasing wafer diameter and decreasing die area accrue, the proportion spent on packaging will rise (on the assumption that packaging costs are relatively insensitive to such dimensional changes). This is demonstrated in Fig. 8, for the same wafer and chip area reductions illustrated in Fig. 7.

0
10
20
30
40
50
60
70
80
90
150 200 250 300
Wafer diameter (mm)
Ratio Packaging /Chip Cost %
2 sq. mm 4.5 sq. mm 10 sq mm
Fig. 8 Relative cost of packaging as a function of wafer diameter and chip area


In this example, if commensurate cost reductions are not made even with standard semiconductor packages, the relative packaging costs will rise from 50 to 70% of the total if a 4.5 mm2 chip area is reduced to 2 mm2 and to 75% if manufacture is moved to a 200 mm line.

Whilst not within the scope of this study, it is likely that costs for nonstandard packages will remain at several times that of standard packages, and hence packaging costs could approach 90% of total cost, at least for high volume CMOS/MEMS.


9 Discussion

A wafer layer-by-layer cost model has been developed for the manufacture of microstructures, including those with high aspect ratios. Summation of the costs for each layer enables an estimate to be made for the unit cost of a multilayer device.

The MEMSCOST model enables all key parameters to be varied, including wafer diameter and chip area, and their effect on wafer layer-processing costs to be assessed. A particular set of assumptions have been made for the figures shown, for example, a micro structure depth H = 200 lm and an annual output of 10,000 wafers. Under these conditions, several of the high aspect ratio techniques can process a wafer layer for $20–30 and the attractiveness of UV LIGA is apparent, as the model shows that a similar cost level can be achieved. Even the cost of X-ray LIGA with SU-8 resist is significantly reduced (from $275 to 40 per wafer layer).

X-ray LIGA using a synchrotron, for the same application, with a sensitive resist and assuming a commercially attractive contract with a synchrotron owning institute, costs around $50–60 per wafer layer. At first analysis this precludes X-ray LIGA as a cost effective manufacturing technique. However, when consideration is given to the need for very high precision microstructures, that can be reproduced in an embossing or injection moulding replication process, the tool cost-performance results are more favourable.

The capital cost of the different technologies is strongly affected by the maximum output of each machine. For example, when demand exceeds this maximum, additional machines must be purchased and the capital cost escalates rapidly. The example of DRIE suggests that UV LIGA and even X-ray LIGA, with a resist such as SU-8, could be a less capital-intensive route to manufacture, even though the relative operational costs are different.

The results currently show general trends only, and costs may vary considerably depending on the design of the device, the depth of any high aspect ratio layers, the quality of finish required, e.g. wall angle or pattern tolerances and particularly the materials involved. Even the purchase price of the equipment can be negotiable, depending on the state of the equipment market.

If the wafer fabrication costs are to be reduced further, for example close to $1/wafer layer, then attention must be given to machine design parameters such as higher flux radiation and high speed wafer handling.

MEMS/microsystem devices are particularly cost sensitive to the packaging interface with the environment, which is often an essential part of their operation. In contrast, a semiconductor device requires permanent exclusion of the environment. Standard, low cost packages for MEMS have yet to be established and this makes accurate cost modelling difficult. It is likely that packaging will remain a significant (>50%) proportion of the cost of a manufactured chip.

The cost/wafer is inversely proportional to the demand for devices (Eq. 2); hence low unit costs can only be achieved by large production runs of the same device and/or a large number of devices/wafer. Fortunately, this latter requirement is met by the relatively small size of a MEMS device compared with the wafer area.

A few devices meet the large volume condition where a dedicated production facility is appropriate, such as silicon accelerometers and ink jet printer heads, e.g. 50–200 · 106 devices/year. The cost problem lies with MEMS devices where the demand can be met by a few thousand wafers.

Over 30 MEMS foundries now exist, each offering its own version of a business plan to avoid the problems described above. For example, techniques such as multi-project wafers, where the fixed costs are shared across many devices or where only a few compatible processes, such as multilevel, silicon surface microengineering, are offered.

Once the microfabrication technology, performance and cost parameters for each layer have been identified, the cost model will give a good estimate of the wafer- and device-processing costs as a function of demand. This will help to determine whether it would be economical to build an in-house capability for the device manufacture, or to use foundry services.


References
Chuang YF, Tseng FG, Lin WK (2002) Reduction of diffraction effect of UV exposure on SU-8 negative thick photo resist by Air- gap elimination. Microsyst Technol 8:308–313
Ehrfeld W, Schmidt A (1998) Recent developments in deep X ray lithography. J Vac Sci Technol B 16(6):3526–3534
Elwenspoek M, Jansen H (1998) Silicon Microengineering Cambridge Studies in Semiconductor Physics and Microelectronics Engineering No. 7
Goodall R, Fandel, Allan A, Landler P, Huff H (2002) Long term productivity mechanisms of the semiconductor industry. In: Semiconductor silicon 2002 proceedings, 9th edn. Electrochemical Society
Gower MC (2001) Laser micromachining for MEMS devices. Proc SPIE 4559:53–59
Griffiths SK (2004) Fundamental limitations of LIGA X-ray lithography: sidewall offset, slope and minimum feature size. J Micromech Microeng 14(7):999–1011
Laermer F, Urban A (2003) Challenges, developments and applications of silicon deep reactive ion etching. Microelectron Eng 67–68:349–355
Lawes RA (2003) The central microstructure facility. http://www.cmf.rl.ac.uk
Lawes RA (2005) Manufacturing tolerances for UV LIGA using SU-8 Resist. J Micromech Microeng 15:2198–2203
Lawes RA, Arthur GG (2004) LIGA for boomerang. Device and process technologies for microelectronics, MEMS and photonics. SPIE 5276:307–317
Lee K et al (1995) Micromachining applications of high resolution ultra-thick resist. J Vac Sci Tech B 13(6):3012–3016
Linder C, Jaecklin V, de Rooij NF (1992) Surface micromachining. J Micromech Microeng 2:122–132
Rumsby P, Harvey E, Thomas D, Rizvi N (1997) Excimer laser patterning of thick and thin films for high density packaging. Proc SPIE 3184:176–185
Schmidt MA (1998) Wafer-to-wafer bonding for microstructure formation. Proc IEEE 86(8):575–1585
Zhang J, Chan Park MB, Connor SR (2004) Effect of exposure dose on the replication fidelity and profile of very high aspect ratio microchannels in SU-8. Lab Chip 4:646–653
