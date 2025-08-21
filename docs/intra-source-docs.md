---
title: "INTRA - Source Docs"
permalink: /intra-source-docs/
site_title: "Training Site"
generated: 2025-08-21T18:39:41Z
---
Non-Controllable Fittings – Elbows
Field = Required Field = Not or Rarely Populated
In the Non-Controllable Fittings feature, elbows are defined by “SubType = Elbow”.
Inlet Diameter Inlet Wall Thickness
Outlet Diameter Outlet Wall Thickness
Branch Diameter – no branch on elbows Wall Thickness – Only Required if not a reducing elbow
Style: 3-R, 5-R, Long Radius, Short Radius, Unknown
Heat Number: If you have the MTR, the Heat Number from the MTR should be put here. For those with no
MTR’s, unknown is good.
Angle: If a segmented elbow, put cut angle here. Otherwise, it is 45 or 90.
Radius: 3-D, 3-R, 5-R, 7-R, LR, SR; Please enter as shown. Do not add spaces, etc.
Roll Angle – A “rolled” elbow occurs when the elbow is not in a straight line with the pipe. When looking at a
plan view (looking down from the top), the elbow would be the turning point on the pipe. It is “rolled”
left, right, up, or down. These are also called “combo” elbows. It means that they are both a left or right
elbow as well as a down or up.
Orientation: Up, Down, Left, Right, Ahead
Length – should be filled out. If you are calculating pipe lengths for as-builting, this should be filled in. Length
is in FEET. One other note - - if the VTC on your line will be yes, this should be filled in correctly.
Specification: We have choices that are all over the place right now. Here are some guidelines:
Pipe Valves Fittings Invalid
API 5L API 6D ASME B 16.5 – Flanges ASTM A3816
ASTM A-53 MSS SP 70 ASME SA350 - Flanges ASTM D25L3
ASTM A-106 ASTM A-105 CS A234 (use ASTM A-234)
ASTM A-135 ASTM A-234 EYS
ASTM A-333 ASTM A-537 – Pressure Vessel WPHY-52
ASTM A-672 ASTM A-537 – Pressure Vessel WPHY-56
ASTM A-691 ASTM A-572 – Pressure Vessel WPHY-65
ASTM D2513-12 ASTM D2513-12 F-42 (is not a GRADE)
GR3PSL ASTM A-860 X-52 (is not a GRADE)
PSL1 ASTM A1018 F-52 (is not a GRADE)
PSL2 MSS SP 44 – Flanges X-60 (is a GRADE)
MSS SP 60 – Flanges
MSS SP 75
MSS SP 97
SA105N – Flanges but should
use ASTM A-105
ARC_Fittings_2024_Rev 2.docx (S. Schlesener) June 2024 Page 1


---


Grade: Gr. A, Gr. B, Unknown, WPB, WPHY-, X-, Y-, HDPE, MDPE, WPL6, 316L
WPHY and Y are sometimes used interchangeably. Best practice is to use the Grade shown on the MTR (if it
says WPHY, use that instead of Y). WPHY means Wrought Pipe High Yield. Any time you see “WP”, it means
“Wrought Pipe”, so WPB is just Wrought Pipe Grade B.
As a rule right now:
Interstate uses “Unknown”, “WPB” or “WPHY” designations
Intrastate uses all “Y” designations. Any MTR or material list, etc with a WPHY should be treated as “Y”
Liquids uses “Unknown”, “WPB” or “WPHY” designations
Comment – format is CL (OD) (Style) Ell (or Elbow) (degree w/orientation)
Interstate: CL 16” 45^ Left OR CL 10” 53^ Right - - Do not use Radius and do not abbreviate orientation
Intrastate: CL 24in Elbow. All other details – Style, Angle Radius – will be field notes.
Liquids: CL 24” 3-R Ell 90^ Rt.
RouteID, Status, Measure, Material, Installation Date, In Service Date, Work Order and Project Number are all
things that you know must be filled out.
Details
ANSI B16 or ASME B16 or both?
Many suppliers and manufacturers talk about ANSI fittings, ANSI flanges, etc. Just do a search on any standards providers website for
ANSI B16.5, ANSI B16.9, etc. You will not find those standards because they do not exist. Many years ago, there was an ANSI B16.5
standard. In 1998, it became ANSI/ASTM B16.5 and I 1996 it became ASME B16.5 However, there are still many suppliers and
manufacturers that refer to ANSI or ANSI/ASME. It is not necessarily correct.
What is the MSS standard?
The MSS SP standards are a set of standards developed by the Manufacturers Standardization Society of the Valve and Fitting
Industry.
What is the difference between 5D and 3D bend ?
A 3D bend is a bend in which the radius of the curve is equal to 3 times the diameter of the pipe. It is a smoother bend than a 1.5D
bend, which looks almost like a regular 90-degree right angle, but it is a sharper bend than a 5D bend, which looks like a smooth arc
between two perpendicular pieces.
A 5D bend allows for a bend radius that is equal to five times the amount of the pipe's diameter. This is one of the greatest bends
there are and goes beyond a 3D or 4D bend.
If you have a 10″ diameter pipe, the radius of the centerline of the bend would be 50 inches.
In our database, some domains are shared. First you must know that there are “domains” for many of other fields.
For instance, the ‘Outside Diameter’ field is shared by many features. That field is on Pipes, Fittings, Casing, etc.
The ”domain” is the list you see when you click on the drop-down arrow next to Outside Diameter.
I mention this because the “Specification” domain has values for a few different features. You can see that some of
the selections apply to different features. Even though you are working on/in the Non-controllable Fittings
table/feature, there ARE selections that do not apply. That is because it is shared. The Pipes, Non-Controllable
Fittings and Controllable Fittings all use the same domain for “Specification”.
ARC_Fittings_2024_Rev 2.docx (S. Schlesener) June 2024 Page 2


---


MAOPMOP
Field = Required Field = Not or Rarely Populated
It is strongly recommended that users rearrange the fields in the Valve table with the “Required” Fields
showing first. Those fields not used and or not populated should be at the end.
MAOP is for GAS lines and refers to the Maximum Allowable Operating Pressure.
MOP is for LIQUIDS lines and refers to the Maximum Operating Pressure.
From Measure: Stationing where MAOP/MOP starts on the line
To Measure: Stationing where MAOP/MOP ends on the line
From RouteID: Pressure System GlobalID or Facility Line GUID where MAOP/MOP record starts
To RouteID: Pressure System GlobalID or Facility Line GUID where MAOP/MOP record ends
Status: This should match the status on the pipe. Auto-populates with In-service.
Pressure Type: Design, Certificate, Grandfather, Special Permit, Other, Pressure Type, Unknown, Operator
Assigned, Historical, Strength Test
Pressure Value: Reported pressure for MAOP or MOP from an Establishment form (B.10/7T-234, etc.)
Unit of Measure: Auto populates with PSI
DetFactorMethodology: Auto-populates with Unknown. This comes straight from the Code of Federal
Regulations (CFR) and can be accessed here: https://www.ecfr.gov/current/title-49/subtitle-B/chapter-
I/subchapter-D/part-192 and here: https://www.ecfr.gov/current/title-49/subtitle-B/chapter-I/subchapter-
D/part-195
The 192 designation should ONLY be used for Gas lines.
The 195 designation should ONLY be used for Liquid lines.
Typically when the line is built (design). Use this when there is not a
192.619(a)(1) Design Pressure
form showing the pressure.
After the line is built and a hydro has been performed; Uses the test
192.619(a)(2) Post-Constr. Pressure
pressure to calculate MAOP.
192.619(a)(3) High Actual Oper. Highest Actual Oper Pressure during 5 yrs preceding date; Mostly
Pressure when (a)(1) or (a)(2) can not be used; this is NOT Grandfathered Clause
192.619(a)(4) History of Pipe History of Pipe (corrosion and actual operating pressure)
MAOP of a pipe segm at the highest actual oper pressure to which it
192.619(c)(Grandfathered) had been subjected to during the five years preceding July 1, 1970, as
long as the pipe segment is in good condition
MAOP determined using a different design factor than that used in
192.619(d) Alternative MAOP (192.620)
192.619(a)(1) or 192.619(a)(2)
192.619(d) Alternative MAOP (192.620) MAOP where transmission pipe has a waiver or Special Permit from
– Special Permit PHMSA
192.619 Other If MAOP is NOT based on any paragraph within 192.619
195.406 Maximum Operating Pressure For Liquids, this is what you will choose 95% of the time.
ARC_MAOPMOP_Rev2.doc (S. Schlesener) February 2024 Page 1


---


195.406(a)(2) Component Design Used when no MOP Establishment form is available, and components
Pressure installed are designed to run below a specified pressure
A calculation of 80% of the hydrotest pressure for any part of the line
that has been tested under subpart E (found here:
195.406(a)(3) 80% Test Pressure Part E
https://www.ecfr.gov/current/title-49/subtitle-B/chapter-
I/subchapter-D/part-195/subpart-E)
Used for instances not established in 192.619 options. Mostly in
Safe Operating Pressure
conjunction with Gathering Compliance forms
MAOP Establishment Date: Date on the MAOP/MOP Establishment document (B.10/7T-234, etc.)
MAOP Establishment Report No:
Date Determined: Date on the MAOP/MOP Establishment document
Verified By: Name on the MAOP/MOP Establishment document
Pressure Test Verified: Yes, No, Unknown. Were you able to verify the pressure test? Whatever is on the
‘Pressure Test’ for VTC should be shown here. It should be the same.
Materials Verified: Yes, No, Unknown. Were you able to verify the materials on the line? Whatever is on the
‘Pipes’ for VTC should be shown here. It should be the same.
Comments: various
Comment Text: various
MLVS: Pressure System (Valve Section) that this MAOP or MOP applies to
TempPressureRestriction: This is populated with the temporary MAOP/MOP value when a Temporary
Pressure Restriction has been placed on the line.
TempPressureExpiry: This is populated with the expiration date when a Temporary Pressure Restriction has
been placed on the line.
GRANDFATHERED: NULL, 0, 1, 1813.5, 18135, 18164, 18165, 18166, No, Yes, Unknown
Date Reviewed:
VSMNOP: various numbers 0 to 1286
From Date: Date
To Date: Date
DEFICIENCY: NULL, 500, F, T. Do not populate.
EventID: NULL, 02/02/2021, 1, 13004, 3511, 6288, 09/20/2016, MOC 6263, MOC 6265, MOC 6266. Do not
populate.
Scab: varoious numbers 0 to 741. Do not populate.
Location Error: Do not populate
Legacy ID: Do not populate
Historic_Begin_Station: Only populate with former stationing when a line stationing reversal occurs.
Historic_End_Station: Only populate with former stationing when a line stationing reversal occurs.
Historic_Begin_Series: Do not populate.
Historic_End_Series: Do not populate.
Beg_X_Loc: Do not populate
Beg_Y_Loc: Do not populate
End_X_Loc: Do not populate
End_Y_Loc: Do not populate
ARC_MAOPMOP_Rev2.doc (S. Schlesener) February 2024 Page 2


---


Valve Data
Field = Required Field = Not or Rarely Populated
It is strongly recommended that users rearrange the fields in the Valve table with the “Required” Fields
showing first. Those fields not used and or not populated should be at the end.
Measure: Stationing where the valve is installed on the line
RouteID: Pressure System GlobalID or Facility Line GUID
Type: There are 25 TYPES of Valves listed. You should only need to use one of the following:
Ball Valve Control Valve Needle Valve (for Regulator
Butterfly Gate Valve small OD pipe) Swing Valve
Check Valve Globe Valve Plug Valve
Status: Valves auto-populate with “Proposed” status. This should match the status on the pipe.
Inlet Diameter: Wall thickness of the valve on the inlet side (the side product is flowing in to)
Outlet Diameter: Wall thickness of the valve on the outlet side (the side product is flowing out of)
Bore Diameter: Wall thickness of the valve on the inside
Branch Diameter: Do not populate with “Unknown”. If there is no Branch, use “N/A”
Material: This should match the material on the pipe.
Remote Operated: Unknown, Yes, No
Manufacturer: On Mill Test or Material List
Rating Class: Shown on Valve Cert as “600” or “900”; Should be enter as “ANSI ###”
(Can not list all of the entries—There are over 100 entries to choose from)
*** A NOTE about Rating Class and Pressure Rating ***
Below are the entries seen most often in work orders for Steel Valves. These increase proportionally by Rating
Class, so you should be able to determine any ANSI Rating Classes that are not in the table below. For
example: Rating Class ANSI 300 has a Pressure Rating of 720#, therefore a Rating Class ANSI 900 has a Pressure
Rating of 2160#. ANSI 300 x 3 = ANSI 900, Pressure Rating If you have any other than these, ask for help.
Rating Class: ANSI 150 is Pressure Rating: 360#
Rating Class: ANSI 300 is Pressure Rating: 720#
Rating Class: ANSI 400 is Pressure Rating: 960#
Rating Class: ANSI 600 is Pressure Rating: 1440# or 1480#
Rating Class: ANSI 900 is Pressure Rating: 2160#
Rating Class: ANSI 1500 is Pressure Rating: 3600#
Pressure Rating: Should choose number with # after it (ex: 300#, 600# or 1960#). The choices with a range
(ex: 0-20 or 0-1500) should not be used.
End Connect Inlet: You should only need to use WE or FE. All other fall into these 2 categories.
Choices: Unknown, ACEW, ARCW, FE, PE, SE, SW, WE, WxF, WxRTJ
End Connect Outlet: You should only need to use WE or FE. All other fall into these 2 categories.
Choices: Unknown, ACEW, ARCW, FE, PE, SE, SW, WE, WxF, WxRTJ
End Connect Branch: If no Branch (99% of the time), should be left blank.
ARC_Valves_Rev1.doc (S. Schlesener) January 2024 Page 1


---


Installation Date: Date the valve was installed
Inservice Date: Date the valve was put in service
Work Order ID: The WO that installed the valve
Project Number: The WO that installed the valve or an alternate WO#
Length: Length of the valve in FEET.
Asset Unit Code: The Valve Number ASSIGNED to your valve. For some companies, these are on the VLM, the
PLD/P&ID or EAM. For other companies, a field person will have to give the Valve Number that is assigned to
you. If you are not sure of the valve number, please ask. It is very important that you ALWAYS populate this
field!
Facility ID: SCADA code for the facility where the valve is located. This could be found on a Gate Setting
Boundary, Site Boundary, or Station Boundary (in SCADANAME field).
Comment Text: The correct format for all valves is CL OD (in or “) Valve Type (e.g. CL 12” Gate Valve or CL 12in
Gate Valve).
Valve Use: What purpose does the valve serve? Is it used to Isolate the line (like a Mainline Valve), is it on a
Bypass line, is it a Blowoff, or is it used to Purge the line (connected to a tank or other equipment)? Bypass,
Blowoff and Purge are more-than-likely only on Detail Piping.
Normal Position: <Null>, Open, Closed. This is auto-populated with OPEN.
Present Position: <Null>, Open, Closed. This is auto-populated with OPEN.
Examples: Launcher/Receiver Valves = CLOSED
Kicker line valves = CLOSED
Blow off valves = CLOSED
Auto Close Ind: Unknown, Yes, No. This field means the same thing as Remote Operated.
RMV Type: RC (Remote Controlled), ASV (Automatic Shut-off), EFRD (Emergency Flow Restriction Device).
Location Description: Where the valve is located (e.g. Suction Line #1 at the Longville Pump Station).
Manufacture Date: On Mill Test
Manufacturer Model: On Mill Test
Manufacture Lot No: Sometimes on Mill Test
Barcode (Serial #): Serial Number (If given in work order)
Oper Manufacturer: Manufacturer of the Actuator/Operator
Oper Serial Number: Serial Number of the Actuator/Operator
Oper Model Number: Model Number of the Actuator/Operator
Oper Date Manufactured: Date Manufactured of the Actuator/Operator
Oper Type: Unknown, Electric, Gas, Hand Wheel, Manual, Motor, Lever
**Valve Operator Notes: Most Valves have an operator except Check Valves. However, fill this part
out only if you have the information in your work order. Also – Manufacturer of operator may NOT be
the same as the Valve Manufacturer.
ARC_Valves_Rev1.doc (S. Schlesener) January 2024 Page 2


---


If Operator is listed as: Gear Operated, MGO, or MOV – use Motor
Hand – use Hand Wheel
Wrench – use Lever
Actuator – use Gas
Inlet Pressure: Same as pressure rating unless it is a Regulator
Outlet Pressure: Same as pressure rating unless it is a Regulator
Set Pressure: Do not populate
VTC Material Verified: Yes, No, Researching
VTC Date Verified: The date you were able to verify (or not verify) the record.
VTC Comments: Why you were able to verify (or not verify) the record.
VTC Verified By: Your username
VTC Method: Documentation and Records, NDE Test, Destructive Test, Test Sampling, Expanded Sampling
EAM Valve ID:
EAM Entity Name:
EAM Valve Comment:
Gas Trace Weight:
Bonded Indicator: Unknown, Yes, No
Clockwise to Close: Unknown, Yes, No
Turns to Close: How many turns of the hand wheel it takes to close the valve
Depth:
Depth to Nut:
Insulated Indicator: Unknown, Yes, No
Operating Classification: Non-Critical, Critical Inspection Required, Critical Inspection Not Required
CP System GlobalID:
Valve Section Source: Yes or No. This auto-populates to No.
Ancillary Role: None, Source, Sink. This auto-populates to None.
https://images.app.goo.gl/EYDnrh9X2kBvRVaM9
https://images.app.goo.gl/bzwxMGsEzbWuewJx8
ARC_Valves_Rev1.doc (S. Schlesener) January 2024 Page 3


---


Comments on Point Features (Intrastate)
• Flanges:
o CL 4in RFWN Flange
o CL 4in Blind Flange
o CL 4in Anchor Flange
• Cap/Closure:
o CL 4in Cap/Closure
• Reducers:
o CL 4in x 2in Conc Reducer
o CL 4in x 2in Ecc Reducer
o CL 4in x 2in Nipple Swage Reducer
• Elbows:
o CL 4in Elbow
• Tees/Saddle Taps:
o CL 4in Tee Right to Sation Piping #1
o CL 4in x 4in Tee Up to Blowoff Piping #1
o CL 4in Tee Right Rolled 45^ Up to Meter Run Bypass
o CL 30in x 4in Saddle Tap Left to Crossover #1
o CL 4in Tee Ahead Rolled 45^ Left to Bypass Piping #1, Up to Continue
o CL 4in Tee Back Rolled 45^ Right to Bypass Piping #1, Up to Continue
• Valves:
o CL 4in Ball Valve (Asset Unit Code)
• Regulator:
o CL 4in Regulator (Asset Unit Code)
• Meters:
o CL 4in Ultra-Sonic Meter (Meter Number/ Asset Unit Code)


---


Field Notes (Intrastate)
• OVB – CL 5^ Overbend
• SAG – CL 8^ Sag
• PIL – PI 10^40’42” Lt.
• PIR – PI 24^15’22” Rt.
o Note: These must be entered in this EXACT format, if you only have 10^24’ listed on the
alignment sheet, make sure to add the 00” at the end. Format = XX^00’00” Rt. or Lt.
• STQ – Ahd.=XXX Bk. ***STATION EQUATION***
o Note: The station equation field note should be entered on the ahead (existing) station
series. Enter as noted above with 5 spaces BEFORE AND AFTER stars and only 3
stars.
• COL – Leave Lake Co., Enter Polk Co.
• RL – Leave R-15-E, Enter R-16-E
• TWP – Leave T-8-S, Enter T-7-S
• SL – Leave Sec. 32, Enter Sec. 33
• STL – Leave Texas, Enter Louisiana
Construction Notes
• At TEE/TAPS: Begin Line 1015 Region Lateral or End of line depending on Flow ...... @ 30+55
on Line 3016(MAINLINE).
• Begin WO- End WO: On Mainline for
o Replacements
 Begin Replacement (WBS or AFE) (Number)
 End Replacement (WBS or AFE) (Number)
o Recoats
 Begin Recoat (WBS or AFE) (Number)
 End Recoat (WBS or AFE) (Number)
o Re-routes
 Begin Re-Route (WBS or AFE) (Number)
 End Re-Route (WBS or AFE) (Number)
o Sleeves
 Begin Sleeve (WBS or AFE) (Number)
 End Sleeve (WBS or AFE) (Number)


---


INTRASTATE Boundary Naming Process
Types of Boundaries
Gate Setting Boundary – used for MLVs, Launchers, Receivers, Dual Trap Sites
Site Type: MLV is Valve Setting, Launcher is for launcher, Receiver is for receiver and
Launcher/Receiver is for dual trap sites. Do not use Launcher/Receiver at sites where there is
only one or the other
• May or may not have detail piping associated
M&R Boundary – Meter stations
Site Type: M&R Station
• May or may not have detail piping associated
Site Boundary – Used for lateral Take-offs (The tap site of a line as it “takes-off” from the
originating line), Wells at the end of a line
Site Type: Lateral Take-Off or Wells (Do not use any other site types unless advised to do so)
• May or may not have detail piping associated
Station Boundary – Compressor Station, Pump Station, Booster Station, Processing Plant
Site Type: As noted above (Do not use any other site types unless advised to do so)
• Does not have any pipes associated
Naming Conventions – Name is a Required Field
Site names should begin with the line number and name and then follow with a description of the site
No diameters should be included in the site name
Launchers / Receivers / Dual Trap Sites
Example: System Name: 1234 West Texas Hot Shot 4in Lateral
Site Name: 1234 West Texas Hot Shot Launcher
Site Name: 1234 West Texas Hot Shot Receiver
If there is more than one launcher or received on a line, you will number them. Duplicate site names are
not allowed
Site Name: 1234 West Texas Hot Shot Launcher 1
Site Name: 1234 West Texas Hot Shot Receiver 1
Site Name: 1234 West Texas Hot Shot Launcher 2
Site Name: 1234 West Texas Hot Shot Receiver 2
04/22/20


---


If the middle set of traps is a dual trap site, you will only create one site boundary for BOTH the launcher
and receiver and name it like the example below
Site Name: 1234 West Texas Hot Shot Launcher
Site Name: 1234 West Texas Hot Shot Dual Trap Site
Site Name: 1234 West Texas Hot Shot Receiver
If there are individual site names identified for each site, those will in place of numbering as long as
there is a name for each site. Do not mix and match numbers with site names.
Site Name: 1234 West Texas Hot Shot Green Plant Launcher
Site Name: 1234 West Texas Hot Shot Perryton Compressor Receiver
Main Line Valve Sites
Example: System Name: 1234 West Texas Hot Shot 4in Lateral
Site Name: 1234 West Texas Hot Shot Valve Setting 1
Site Name: 1234 West Texas Hot Shot Valve Setting 2
The same rules apply for is there is a site name identified
Site Name: 1234 West Texas Hot Shot Green Plant Valve Setting
Site Name: 1234 West Texas Hot Shot Perryton Valve Setting
Meter Stations
Example: System Name: 1234 West Texas Hot Shot 4in Lateral
M& Boundary Name: 1234 West Texas Hot Shot Meter Station
*Always spell out “Meter Station”
04/22/20


---


Question: What if you have a launcher or receiver at the same location as meter piping?
Answer: You will create a boundary for each, covering the entire location, but not overlapping. Make
sure to snap them together so that there are no gaps between the two. When you have a drawing that
shows the fence, cover the entire fence area with boundary / boundaries. You will associate the proper
pipes to each boundary and related facility lines.
See example below:
This is the exact site in the DB with a gate setting boundary in blue and M&R boundary in red. It is highly
recommended that when setting up boundary display options in your MXD, you use an outline only and
a border. If you use a solid polygon, you may not see boundaries that could potentially currently exist
under other boundaries.
04/22/20


---


Do not stack boundaries like this example:
NOTES:
1. You may have overlapping boundaries only when there is a large site like a compressor station
(station boundary/site ) and multiples lines that go into it with launchers or receivers or meter
stations (gate setting boundary or M&R boundary). You will have one large station boundary for
the entire facility and then smaller gate setting or M&R boundaries for each of the traps or
M&Rs.
2. When creating well sites, you will use a 10’ square site boundary at the end of the line. This
applies to all sites where a fence or property line cannot be seen, and there is no detail pipes.
Wells, MLVs
3. All boundaries will be drawn in with squared corners where applicable. Do not free hand a
boundary that is a square or rectangle. Make sure to draw it with 90-degree corners. If a
boundary already exists, you should use a sketch tool to sketch a new shape and then snap the
existing boundary to it.
04/22/20


---


Valve Names
Main Line
–
V-100 - Mainline Valve
V-100-CK - Mainline Check Valve
Detail Piping
(Mainline Valve ID must be placed before each valve on detail pipe) Below are
examples of what to call a Valve to their corresponding Facility Line when Valve
ID’s are NOT provided.
K- Kicker
EQ - Equalizer
XO – Crossover
KXO – Kicker Crossover
BT – Blind Tap
USBO – Upstream Blowoff Piping
DSBO – Downstream Blowoff Piping
IC – Interconnect
PG - Power Gas
BY – By-pass
HV – Heater piping
RGP - Inlet & Outlet Regulator Piping
A1 – Regulator Run #1
RGA1 – Regulator #1
A2 – Regulator Run #1
B1 – Regulator Run #2


---


RGB1 – Regulator Run #2
B2 – Regulator Run #2
C1– Regulator Run #3
RGC1 – Regulator Run #3
C2 – Regulator Run #3
BO – Blow-off Piping
BO1 – Blowoff Piping #1
BO2 – Blowoff Piping #2
BD – Blowdown
BL – Bleeder Line
RFV – Valve Before Relief Valve
RV – Relief Valve
OMV – Outlet Meter Run
IMV – Inlet Meter Run Piping
CSA – Compressor Station Piping #1
CSB - Compressor Station Piping #2
CSC - Compressor Station Piping #3
CSUA – Compressor Suction #1
CSUB – Compressor Suction #2
CSUC – Compressor Suction #3
SU – Suction
DS – Discharge Piping #1
FV - Filter Piping #1
SP - Station Piping
SBY – Station By-Pass
ISP – Inlet Station Piping
OSP- Outlet Station Piping


---


DL – Drain Line
SB- Scrubber Line
HD – Header Piping
Meter ID must be placed before each valve on Meter detail piping. Below are
examples of what to call a Valve to their corresponding Facility Line. USE actual
Meter ID provided.
M-19-1 - Meter Run #1 (Valve on Meter Run)
M-29-1 - Meter Run #2 (Valve on Meter Run)
M-39-1 - Meter Run #3 (Valve on Meter Run)
M1 – Meter (Actual Meter)
M2 – Meter (Actual Meter if provided)
