---
title: "LIQUIDS - Source Docs"
permalink: /liquids-source-docs/
site_title: "Training Site"
generated: 2025-08-21T18:39:43Z
---
Process for As-Builting Liquids Lines
***You will need to turn in a weekly report on all work completed***
 Records and documents for as-builting:
o IMU/ILI/Survey Data: IMU or survey data is accurate to sub-meter GPS and
should be used to correct the centerline. Do not adjust to ILI unless you are SURE
it is sub-meter accurate. ILI can be used to check lengths of pipe, wall thickness,
long seam, and presence of fittings.
o Historic Construction Documents: Historic documents pertaining to original
construction of the line
o Alignment Sheets: These are historic alignments, which will be used to enter any
missing data in the database
o Maintenance Records (MRs): Maintenance which has been performed on the
line (Foreign Line Crossings and Pipe Repairs)—these need to be both installed,
and checked for presence in the database
o Accompanying materials: Hydro tests (Splint Hydro records), Mill Test Reports,
ILIs, Engineering drawings, Line Histories, GForms, Assessable Segments list, etc.
o Field Note Guidelines: Instructions for correcting existing Field Notes (See
separate Word Document)
o Pipe Crossing Guidelines: Instructions for correcting existing Pipe Crossings as
well as installing new Pipe Crossings from MRs (See separate Word Document)
 You will be installing and changing several things when as-builting, including:
o Pipe records (Spec, Grade, Coating, Manufacturer, Installation date, Longitudinal
Seam Type, etc.)
 You may need to split existing pipe by weld, pipe manufacturer, or
coating (for sleeves). Make as few pipe segments as possible while still
retaining that information (i.e. if you have two pipe segments next to
each other with the same Manufacturer, Grade, Coating, Wall Thickness,
and Installation date, the segments don’t have to be split at the weld, and
can be merged).
 When doing a replacement, you will not break the pipe for the transition
coating change at the start and end of the replacement; add it as a
comment in the replaced pipe records (i.e. “3ft of tape coat extends past
replacement”). The old pipe record must be copied into Pipes_Arch and
commented as “Removed per MR XXX”.
 NOTE: Any ERW pipe with an installation date before 1980 will be
entered as ERW-LF. Post-1980 ERW pipe is ERW-HF, unless otherwise
stated.
1


---


o Fittings (Elbows, Flanges, Tees, and Reducers). The pipe WILL be split at the
fitting, so take that into account when you calculate stationing. See examples on
Page 13.
 Non-Controllable Fittings should be installed with the following format in
the Comments field:
 For Flanges: “CL” followed by the size of the flange, type of flange,
and then fitting type. In the example below, this is a 12” Raised
Face Weld Neck Flange. If the type of flange is unknown, simply
use “CL 12” Flange”.
CL 12” RFWN Flange
 For Elbows: “CL” followed by the size of the elbow, fitting type,
the degree bend followed by ^, and the direction of the bend. Use
LT, RT, UP, DN. Make sure these are fittings and not field bends.
CL 12” 3-R ELL 45^ LT
 For Reducers: CL followed by the sizes (there should be TWO), and
then the fitting type.
CL 12”x10” Conc. Reducer
 For Tees: CL followed by the sizes (if it reduces), fitting type, and
then the direction.
CL 12”x10” Reducing Tee Left
 REMEMBER: ANYTHING YOU WRITE IN COMMENTS WILL SHOW
UP ON THE ALIGNMENT SHEET! Make it as short and easily
understandable as possible.
o Pipe Crossings. See the Pipe Crossing Guidelines Word document for information
on installing and correcting these.
o Field Notes. See the Field Note Guidelines Word document for information on
correcting these. ***See this document for adding equations***
o Valves. The pipe will be split at all the Mainline Valves, and the Pressure System
changes at each MLV. If you come across multiple Valves in one location (either
stacked or next to each other on the Mainline), and the valves do not specify
what is MLV and what is Bypass, ask your Team Lead what should be done. ***If
you move a Valve, make sure you use the Shorten/Lengthen Pressure System
tool on the Toolbar***
 The Pressure System on the Valves will ALWAYS be the Ahead Pressure
System. Make sure you check each of your valves to ensure that the
Pressure System matches the Pressure System on the pipe that
immediately follows.
2


---


o Pressure systems. Pressure Systems must be unique after each MLV and Station
Equation. They should be named according to the upstream mainline valve
number and have a lowercase letter starting with “a” (i.e. MLV-1402 =
downstream valve section 1402a). If there is an equation, a new pressure system
is installed at the equation and the Pressure System Name downstream of the
equation is 1402b; if multiple equations exist between valve sections, the
Pressure System Name will remain 1402 with the letter changing to the next in
series (see diagram below).
1402 1403 1404
PS =1402a PS =1402b PS =1402c PS=1403
a
EQ EQ
o Sleeves (in the database under UPDM.Sleeve). These are versioned and DO need
to be installed according to the MR. Fill in the attributes as best as you can from
the details on the MR. Many of the repairs done are Clock Springs, which are
considered Sleeves.
o Casings (in the database under UPDM.PipeCasing). These are versioned and DO
need to be installed according to the MR or historic document. They are usually
installed under roads and railroad tracks on older lines. Fill in the attributes as
best as you can from the details on the MR or historic document. Ask your Team
Lead if you have questions.
o Welds (in the database under UPDM.WELD). These are non-versioned, and DO
need to be installed according to the MR. They are installed any time a pipe is
replaced. ***Do not attempt to go back through the MRs and add historic welds
or add them from alignment sheets. Only install Welds as you add MRs.***
Below is a sample of fields that need to be filled in as well as the format which
each field should take:
XRAY
NUM HEATNUM COATINGCOATING SPECIFIC INSTALLATION
STATUS MEASURE TYPE BER BER REMARKS COMMENTTEXT TYPE MATERIAL ATION WORKORDERID DATE ROUTEID
SOURCE: Maintenance Record;
COMMENTS: Replaced BV24 (Duffers {4f220325-dfbc-44cb-
Active 109309.56Unknown TI-1 131878<Null> Tavern Valve) and removed 2 taps. Tapecoat Wax Tape ERW ICA-2208-14 5/15/2014b727-97d216ee61bd}
Heat #: 131878 Bk. / 111398-N Ahd.;
SOURCE: Maintenance Record;
COMMENTS: Replaced BV24 (Duffers {4f220325-dfbc-44cb-
Active 109312.56Unknown FB108 111398-N <Null> Tavern Valve) and removed 2 taps. Tapecoat Wax Tape ERW ICA-2208-14 5/15/2014b727-97d216ee61bd}
Heat #: 111398-N Bk. / 131878 Ahd.;
SOURCE: Maintenance Record;
COMMENTS: Replaced BV24 (Duffers {4f220325-dfbc-44cb-
Active 109314.86Unknown FB107 131878<Null> Tavern Valve) and removed 2 taps. Tapecoat Wax Tape ERW ICA-2208-14 5/15/2014b727-97d216ee61bd}
Heat #: 131878 Bk. / 131882 Ahd.;
SOURCE: Maintenance Record;
COMMENTS: Replaced BV24 (Duffers {4f220325-dfbc-44cb-
Active 109319.86Unknown XR-1 131882<Null> Tavern Valve) and removed 2 taps. Tapecoat Wax Tape ERW ICA-2208-14 5/15/2014b727-97d216ee61bd}
Heat #: 131882 Bk. / 922221-N Ahd.;
SOURCE: Maintenance Record;
COMMENTS: Replaced BV24 (Duffers {4f220325-dfbc-44cb-
Active 109322.86Unknown FB115 922221-N <Null> Tavern Valve) and removed 2 taps. Tapecoat Wax Tape ERW ICA-2208-14 5/15/2014b727-97d216ee61bd}
Heat #: 922221-N Bk. / 131878 Ahd.;
SOURCE: Maintenance Record;
COMMENTS: Replaced BV24 (Duffers {4f220325-dfbc-44cb-
Active 109325.16Unknown FB116 131878<Null> Tavern Valve) and removed 2 taps. Tapecoat Wax Tape ERW ICA-2208-14 5/15/2014b727-97d216ee61bd}
3


---


 XRAYNUMBER is the weld number on MRs.
 HEATNUMBER is the heat number of the Ahead pipe segment or fitting.
 WORKORDERID is the Tracking ID of the MR or GForm #.
o Pressure Verification. Many of these lines have Hydro Test records, but the
Pressure Verification has not been installed in the database. When installing,
ensure that both the vertices and the attribute table have been filled in
correctly. A new Pressure Verification must be installed for each pipe
replacement. NOTE: You will not be able to search for the Pressure Verification
in the database using related tables; you will have to query by RouteID to see
any Hydros for that line. Splint hydro records need to be searched for each line
using the Master List (Splint_HydroTest_ProductionData), and any found Hydros
added to the database.
 If adding a new Hydrotest for an entire line (there is not an existing
hydrotest for the line), follow these steps to quickly import a hydro for
the line:
 Make sure you have a definition query on Pipes for your line only,
you are NOT editing, and nothing is selected in your map
 Right click the Pipes layer in the Table of Contents
 Select Data > Export Data > All Features > This Layer’s Source
Data > Click the folder icon to save your shapefile
 When prompted to add the layer to your map, select Yes
 Start editing the shapefile you added
 Right click the shapefile and click Selection > Select All
 In the Editor toolbar, select Merge and be sure that “Preserve
Overlapping Segments” is NOT selected
 Stop editing and save edits
 Be sure that your Pressure Verification layer is turned on
 Start editing your version
 Right click the shapefile you edited and click Selection > Select All
 Right click the map and click Copy > Paste
 When prompted for the layer, select Pressure Verification
 Fill in all of the missing attributes for the hydrotest
 Pressure Test is the test record number—this can ONLY be a numerical
value!
 Min Design Pressure is the targeted minimum test pressure
 Min Adjusted Pressure is the actual minimum test pressure
 Unit of Measure will always be PSIG or psi
 Test Type will be Strength
 TVC Material Verified will always be YES if you have the hydrotest record
 TVC Date Verified is the date that you verified the record
4


---


 TVC Comments will be any relevant information listed on the record
about the test (from station to station, line size, was this the result of a
line failure, etc.)
 If adding a hydrotest for a pipe replacement, you must add the hydrotest
manually. Make sure that you have filled out BOTH your vertices and
attribute table with the correct measures.
 Hydrotests can span multiple Pressure Systems, but they CANNOT span
multiple Systems. You need a new hydrotest for each System record.
o MAOP/MOP. Unless a new MOP has been established by the Integrity group,
ONLY correct the geometry of the existing MOP centerline. If you have an MOP
document, you may install a missing MOP.
 If you are installing a new MOP for an entire line, you may follow the
same directions as above to import the line to the MAOPMOP layer
 Make sure you have your MAOPMOP layer turned on
 You can use the same shapefile for your hydrotest line to import
the MOP line
 Make sure you have filled out BOTH your vertices and attribute
table with the correct measures.
 Pressure Type will almost always be Strength Test
 Date Determined is the date on the hydrotest or MOP document
 Verified By is the person who signed off on the MOP document
 Comments will be any relevant information about the MOP
determination
 Det Factor Methodology is the Determining Factor Methodology. This
will usually be 195.406.
 Fill out any other relevant data in the table
 MOPs can span multiple Pressure Systems, but they CANNOT span
multiple Systems. You need a new MOP for each System record.
NOTE: When searching the System table for the correct line, make sure you select the correct
line. Sometimes there is more than one record for the System. In the example below, the
second record is Abandoned Pipe.
5


---


Do not assume anything on these records! There is no default
coating, pipe spec, or grade!
The order of operations for your work should be:
1) Update Piggable/Assessable Segments (THIS STEP SHOULD HAVE ALREADY BEEN
COMPLETED FOR ALL LINES)
 If the line has more than one launcher or receiver valve, you must update the
Piggable Segments in the System table. See the SXLAssessableSegmentList
Excel file to update SXL Lines
oTo create a new Piggable segment, you should create a new System
using the System Split tool and update with the data from the existing
System. Check the SXLAssessableSegmentList spreadsheet to
determine what to name your segments. ONLY USE THE BOLT
TOOLBAR TO CREATE NEW SYSTEMS!!!
 Your Proper Name will change to the line number followed by
a period and a two-digit number (i.e. 12124.01, 12124.02, etc.)
 Your SYSTEMNAME will change to the line number followed
by a period and a two-digit number, and the name of the
Piggable Segment (i.e. 12124.01 – Montello-Mt. Union)
oExample: The Piggable Segments for the line below would be
12124.01 – Montello-Mt. Union, 12124.02 – Mt. Union-Altoona,
12124.03 – Altoona-Delmont. This example has 3 Piggable Segments
because there is a launcher/receiver at each of these Pump Stations
***NOTE: If your line has only one launcher and receiver, NOTHING
needs to be done with Systems***
Montello Mt. Union Altoona Delmont
2) Adjust the line according to the survey data or IMU
 You will need to import the survey data or IMU from the Excel spreadsheet
provided. Each file contains lat/long data that will appear as points and will
aid you in adjusting the line. It may help to run the Points To Line tool in
ArcToolbox which connects the survey or IMU points into a line to adjust the
centerline. Ask your Team Lead if you have questions.
 The survey/ILI has features listed—pay close attention to those when moving
the line. The survey may be calling out a fence, property line, PI, or water
crossing. These may already exist as Field Notes or Crossings, which can help
in determining where the line moves. The major features you will want to
6


---


snap the line to are: Welds, AGMs, Fittings, Casings, Sleeves, Taps, and
Valves.
 Make sure to check for other features when you move the line, as they may
have stayed behind (Casings, Sleeves)
3) Check Casings, Sleeves, Field Notes, and Pipe Crossings
 Are Casings and Sleeves installed at the correct stationing on the line? If not,
move them to the correct stationing. Is the diameter, type, material, install
date, crossing type, and wall thickness filled in for casings?
o REMEMBER: Casings WILL NOT be installed around bends. If you find
a Casing that covers a bend, move it so that it is on a straight section
of pipe.
 Are Field Notes and Crossings in the correct format on the entire line? Has all
information been filled in? CHECK the Process Document for Field Notes and
Crossings if you are unsure.
 Inactivate Field Notes if they meet these criteria:
o Duplicate field notes (EXCLUDING PIs on EQUATIONS)
o Hazards and Trench Breakers
o PIs with angles under 5°
o Notes relating to replacements (i.e. “begin/end replacement”)—DO
NOT confuse these with “begin/end relocation”, which are needed
4) View and enter historic document information in database (PigData), and add
missing data from historic alignment sheets
 Work from most current backwards to oldest
 Documents will mostly consist of pipe data, coating, installation year, in-
service date, and hydro information
 Check Adept for other historic documents (e.g. relocation drawings, SunMap
and original alignment sheets)
 Crossings, Sleeves, Casings, Field Notes, Fittings, and Valves are usually
displayed on old alignments; install anything you notice is missing including
test stations, rectifiers, and magnets
oSome road names have changed since historic alignments were
generated. Check the name against Google to be sure you have the
most current road name; enter the old road name from the alignment
sheets in the Comments field, and the new one in Remarks
 Install any missing coatings, pipe data, replacements, re-routes, and
equations (Re-routes and replacements must be verified with supporting
documents such as MRs or drawings).
5) Install Maintenance Records
 Look in all three drive locations for MRs: Maintenance_Records>Historic,
Maintenance_Records>Pipeline, and MR_Processing>03_MR_GIS_Inbox.
Also look in the ETIH drive for any records that were scanned in by Erin
7


---


(\ETIH\Apps\caddata\asbuilt\PA Icedale Eng Records\Erin) and Jennifer
(\ETIH\Apps\caddata\asbuilt\PA Icedale Eng Records\Jennifer).
 Check the database for each record. If you don’t see it, it needs to be
installed. ***Make sure to check the lat/long AND the
stationing—sometimes the lat/long does not match stationing or is not near
the line***
 Instructions for completing Pipe replacement MRs are below. See Pipe
Crossing Guidelines Word Document for installing Foreign Line Crossings.
 For records that have already been “completed”, there are three
designations at the end of the file name: V, F, and R. V is for Visual
Inspection, and nothing needs to be installed for the record, but other
information can be verified (such as coating information). F is for Foreign
Line Crossing, and it means that a Pipe Crossing needs to be installed. R is for
Repair, and it means that a Pipe has been repaired or replaced and needs to
be installed. Check each record to verify it is in the database regardless of
“completed” status.
 Check GForms for Pipeline Inspections, Foreign Line Crossings, or Repairs
that have been performed on the line. These may have been completed in
GForms and we may not have copies of the repairs in MR form.
o Navigate to Project Pulse > GForms.
o Under Document Hierarchy, fill in the first four fields to get Discharge
to populate.
8


---


o Click on each GForm to view it. Install GForms that are not in the
database. You will be looking for Valve Maintenance Reports, Pipeline
Inspections, and Foreign Line Crossings. ***You will not install new
Foreign Line Crossings from GForms! You will only check the ones
that have already been installed***
6) Update/fix Valve Sections
 Use the Bolt toolbar to update, split, and sync the Pressure Systems
oPressure Systems need to be split at Valves and Equations.
oReview the Appendix to the UPDM As-Built Procedures Manual
discussing the new Bolt Toolbar
 This may also entail removing valves from the mainline and moving them to
new Detail Pipe. Use imagery, the Comments field in the Valve table, and the
Valve diameters to determine which Valves belong on the mainline and
which belong on Detail Pipe. ***Don’t be afraid to email or call someone
from the area to ask them to verify!!!*** Mark any Mainline Valves as
“Isolation” under Valve Use.
 See example on Page 2 above for how Pressure Systems should be split
 If you come across a Pressure System that is not associated to any Pipes or
Archived Pipes, put “_Not_Used” at the end of the existing Pressure System
Name, and in the Pressure System COMMENT_TEXT field, add a comment
to the existing field saying “Not used – (Month & Year)”.
 If the Pressure System ONLY has Archived Pipes associated with it, change
the Pressure System Name to “0a_Archive”, and in the Pressure System
COMMENT_TEXT field add a comment to the existing field saying “Archived
– (Month & Year)”. BE VERY CAREFUL to check the OPERDIVISION field and
make sure it doesn’t say 04-Archive, 08-Historic, or 09-Abandoned. IF YOU
CHANGE THESE RECORDS, YOU WILL NOT BE ABLE TO REC & POST!
7) Hydro correction/installation and MAOP correction
 Add new Hydros from pipe replacements, verify historic Hydros are installed,
and check for MAOP
8) Check the As-built List spreadsheet (Transmission Tracker tab, second-to-last
column) for comments from contractors
 Review the comments and make sure that any issues found by the
contractors have been resolved in your QC of the line. If so, change the fill
color of the cell to No Fill.
9) Regenerate alignment sheets
 Remember: there is an overnight delay on HelloSheets for versioned
features. If you post today, your changes will not show up on alignments
until tomorrow (unless ONLY editing non-versioned features).
10)Notify Team Lead that alignments for your line are ready for Field Ops and Integrity
group to review
9


---


 Track date completed on As-built List spreadsheet in Metrics tab and
Transmission Tracker tab
 Track date completed on Line Assignment Tracker spreadsheet (Transmission
Metrics tab) and record the hours worked on line as well as any issues you
had with completion
***If working on a Deferred or Idle line, please check the system table and make sure that the
Pipe Status and Product Type are correct!!
 If Pipe status says IDLE, it needs to be changed to Deferred. IDLE is not a valid status
and should NOT be used.
 If Product Type is Nitrogen, the Product Type and Product Group need to be changed to
reflect what was in the pipe before it was Deferred. If you have a line deactivation
GForm, DO NOT change the Product Type to Nitrogen!
10


---


Below is a two-page example of an MR which has already been completed, and how these
inputs appear in the database.
BLUE BOX: The SCADA name and Line number you’re working on
RED BOXES: The lat/longs you will use to find your work area in the database; if no
lat/long is provided on the MR, you can use the Linear Referencing tool to locate your
work area. If you need assistance, ask your Team Lead.
YELLOW BOXES: The comments you will use to fill out the COMMENTS field for Pipes
and Welds in the database
PURPLE BOX: The Record Tracking ID number you will use in place of WorkOrderID in
the database
11


---


12


---


GREEN BOXES: Information you will enter in the database for Pipe records
ORANGE BOXES: Information you will enter in the database for Weld records and for
Heat number on Pipe records
GREY BOXES: Information you will use to ensure your MR is installed in the correct
location with the correct length
PURPLE BOX: The same Record Tracking ID number from the first page
BLACK BOXES: Weld X-Ray numbers
 Notice that this MR has two different heat numbers on it and has already been labeled
with the Pipe manufacturers. Your MRs will not be labeled with Manufacturer
information.
 The tie-in stationing from the grey boxes has also been filled in on the diagram. These
may not appear on all of your MRs, but it is your responsibility to CHECK the stationing
on the diagram—it might not always be correct!!
13


---


Below is how this MR should appear in the database.
BLUE BOXES: Use your Go To XY Tool to find your lat/long.
GREEN BOX: There are TWO pipe records here, as per the MR. All of the information from
the second page of the MR has been filled in.
BLACK BOXES: There are THREE welds here, as per the MR. All of the information from the
first and second pages of the MR has been filled in.
14


---


Below is a more complicated example of a MR, where the pipe is split by Fittings as well as
Welds and Pipe Manufacturer.
GREY BOXES, STATIONING AND LINES: Where the pipe will be split due to the Fitting. Since
Fittings are point files, everything up to the grey line will be the Pipe Manufacturer before the
line.
GREEN LINES AND ARROWS: Where the pipe will be split due to Pipe Manufacturer change.
BLACK BOXES: Weld X-ray numbers. Notice that this is also where the pipe is split when there is
a Pipe Manufacturer change.
RED CIRCLES: Heat numbers for Pipe and Fittings.
Note: There are instances on this MR where the heat number changes, but the Pipe
Manufacturer does not change. If all of the information for the Pipe is the same except for the
Mill Test date, you can still merge the Pipe records in the database. Choose the OLDEST Mill
Test date from all of the MTRs and use that.
15


---


Fitting example: The first fitting is an ELL (Tectubi) at station 2715+63.75. The Hyundai Pipe is 6’
long between Welds TI-1 and XR-33. The Tectubi ELL is 1.5’ long between Welds XR-33 and XR-
34. Since the Pipe is split at the fitting, your Tectubi ELL length is split in half to account for the
Fitting point (1.5’/2=0.75’). So, the stationing for the Hyundai Pipe will extend from station
2715+57 to station 2715+63.75 where the first Tectubi ELL is (2715+57 + 6’ = 2715+63 and
2715+63 + 0.75’ = 2715+63.75).
Pipe and weld example: The first time the Pipe is split by Manufacturer is at Weld XR-37 (station
2715+78.9), when the Pipe transitions from Nexteel to Hyundai. ***THE STATIONING ON THIS
DIAGRAM IS NOT ACCURATE—ALWAYS CHECK!!*** The Nexteel Pipe begins at station
2715+73.85 with the Tectubi Fitting and extends to station 2715+78.9 at Weld XR-37. The
Hyundai Pipe begins at the same Weld (XR-37), and extends to station 2716+21 at Weld XR-29.
This example appears in the database as below.
GREEN ARROWS: Pipe split due to Manufacturer Change at Welds.
GREY ARROW: Pipe split due to Fitting (ELL).
16


---


Field Note Guidelines
 Make as short as possible so the Alignment Sheet isn’t cluttered.
 Use “RouteID”, “Measure”, “Status”, “TYPE”, “DESCRIPTION”, and “SURVEYBOOK”.
 “Active” and “In-Service” are both valid domains, but you will only be able to choose “In-
Service” if you are adding new Field Notes or changing the status of existing Field Notes.
 When installing Field Notes from GForms or Maintenance Records, use the SURVEYBOOK
field to fill in the MR Tracking Number or GForm number so the source can be referenced.
For all PIs:
RouteID Measure Status TYPE DESCRIPTION LOCATEBY SURVEYBOOK
{d4d46d5a- 374231 In-Service PI ANGLE: LT 10d <Null> <Null>
6731-42e4- 57m 10s;
90c2- BEARING: N
d7141747266f} 10d 57m 10s
W;
DESCRIPTION:
PI Left;
 DESCRIPTION shows in HelloSheets exactly as typed, so it needs to be as short as
possible. We only need the Angle and direction, not anything else after that. The edited
Description should follow this format:
DESCRIPTION
ANGLE: LT 10^ 57’ 10”
o You should use ^ for your degree symbols. Although both ° and ^ will show as a
degree symbol on HelloSheets, ^ will cause fewer errors in Reports.
 IF YOU HAVE AN ELBOW ON THE LINE, YOU WILL NOT HAVE A PI AT THAT LOCATION!
Delete the PI from that measure so that both do not show up on alignment sheets. Only
use PI if you are not sure that the bend is a fitting, and use either a Field Note or a
Fitting, NOT BOTH. The sheet notes will look like this if you have both a PI and a fitting,
which is confusing:
3742+31 ANGLE: LT 10^ 57’ 10”; CL 12” ELL 10^ LT
 Pay extra attention to records such as these:
RouteID Measure Status TYPE DESCRIPTION LOCATEBY SURVEYBOOK
{7c3947be- 399241.4 In- Unknown ANGLE: RT <Null> <Null>
3223-485b- Service 14d 52m 48s;
8fa0- BEARING: N
897001360d5f} 14d 52m 48s
E;


---


{434c1759- 399230.2 In- Unknown ANGLE: RT <Null> <Null>
b87b-4060- Service 14d 52m 48s;
8711- BEARING: N
bb10ceb2dd17} 14d 52m 48s
E;
o There are two different RouteIDs, two different Measures, the TYPE is Unknown,
but the DESCRIPTION is the exact same Angle and direction. If these Field Notes
are in the same location in Arc, it means this is a STATION EQUATION.
 You will need to add another Field Note at this location for your station
equation if it is not present already. The comment format is as follows:
AHD = 3992+41.4 BK ***STATION EQUATION***
 There are five spaces between “BK” and “***”. Your created Field Note
record should appear as follows:
RouteID Measure Status TYPE DESCRIPTION LOCATEBY SURVEYBOOK
{434c1759- 399230.2 Active Equation AHD = <Null> <Null>
b87b-4060- 3992+41.4 BK
8711- ***STATION
bb10ceb2dd17} EQUATION***
 The Measure field will always be the Ahead measure, and the RouteID
(Pressure System GlobalID) will always be the Ahead RouteID.
 There will be three records at this location in Arc. They will appear this
way:
RouteID Measure Status TYPE DESCRIPTION LOCATEBY SURVEYBOOK
{7c3947be- 399241.4 Active PI ANGLE: RT 14° <Null> <Null>
3223-485b- 52’ 48”
8fa0-
897001360d5f}
{434c1759- 399230.2 Active PI ANGLE: RT 14° <Null> <Null>
b87b-4060- 52’ 48”
8711-
bb10ceb2dd17}
{434c1759- 399230.2 Active Equation AHD = <Null> <Null>
b87b-4060- 3992+41.4 BK
8711- ***STATION
bb10ceb2dd17} EQUATION***
 Notice that the Field Note Type has been changed from “Unknown” to
“PI” for the two angles.


---


For all “Markers”:
RouteID Measure Status TYPE DESCRIPTION
{d4d46d5a-6731-42e4- 369600 In-Service Marker Description: AERIAL MARKER 70;
90c2-d7141747266f} Marker Type: Aerial Marker;
{d4d46d5a-6731-42e4- 381276 In-Service Marker Marker Type: Magnet;
90c2-d7141747266f}
 “Marker” is not a valid domain in TYPE, so Aerial Markers will be identified as Sheet
Notes.
 The DESCRIPTION for Aerial Marker is redundant. Remove all duplicate information.
 “Magnet” is a valid domain, so you will change TYPE to “Magnet”.
 All of the trailing semicolons need to be removed. The edited output will look like this:
RouteID Measure Status TYPE DESCRIPTION
{d4d46d5a-6731- 369600 Active Sheet AERIAL MARKER 70
42e4-90c2- Note
d7141747266f}
{d4d46d5a-6731- 381276 Active Magnet Magnet
42e4-90c2-
d7141747266f}
For all Sags and Overbends:
RouteID Measure Status TYPE DESCRIPTION
{B36793C4-3E43- 225213 In-Service Overben Overbend 5^
4F21-BFDC- d
5AF5D91D62DF}
{B36793C4-3E43- 137969 In-Service Sag Sag 7^
4F21-BFDC-
5AF5D91D62DF}
 Sometimes these will have degree values for the bend, and sometimes they won’t. If
they have degree values, make sure they have ^ after them.
 To shorten the Overbend Description, make it “OB”.
RouteID Measure Status TYPE DESCRIPTION
{B36793C4-3E43- 225213 In-Service Overben OB 5^
4F21-BFDC- d
5AF5D91D62DF}
{B36793C4-3E43- 137969 In-Service Sag Sag 7^
4F21-BFDC-
5AF5D91D62DF}


---


For all Township Line, Property Line, County Line:
RouteID Measure Status TYPE DESCRIPTION
{d4d46d5a-6731- 373139 In- Sheet Note Description: Franklin Township; Sheet
42e4-90c2- Service Type: Township Line;
d7141747266f}
{d4d46d5a-6731- 377819 In- Sheet Note Description: PROPERTY LINE; Sheet Type:
42e4-90c2- Service Property Line;
d7141747266f}
{d4d46d5a-6731- 373290 In- Sheet Note Description: Somerset County; Sheet
42e4-90c2- Service Type: County Line;
d7141747266f}
 All of these are currently in the database as “Sheet Notes”. They need to be changed to
their correct TYPE, and their descriptions shortened. Remove redundant information
and keep what is useful. The edited output should look like this:
RouteID Measure Status TYPE DESCRIPTION
{d4d46d5a- 373139 Active Townshi Township Line: Franklin Township
6731-42e4- p Line
90c2-
d7141747266f}
{d4d46d5a- 377819 Active Property PL
6731-42e4- Line
90c2-
d7141747266f}
{d4d46d5a- 373290 Active County County Line: Somerset County
6731-42e4- Line
90c2-
d7141747266f}
For all “Relocation”:
RouteID Measure Status TYPE DESCRIPTION
{7c3947be-3223- 398985.9 In- Relocation Description: BEGIN RELOCATION; Sheet
485b-8fa0- Service Type: Relocation;
897001360d5f}
{a6f99c51-5fe3- 393193 In- Relocation Description: BEGIN RELOCATION; Sheet
40b2-a92c- Service Type: Relocation;
493f5f4d6b05}
 “Relocation” is not a valid domain in TYPE, so Relocations will be identified as “Sheet
Notes”. The edited output should look like this:


---


RouteID Measure Status TYPE DESCRIPTION
{7c3947be-3223- 398985.9 Active Sheet Note BEGIN RELOCATION
485b-8fa0-
897001360d5f}
{a6f99c51-5fe3- 393193 Active Sheet Note BEGIN RELOCATION
40b2-a92c-
493f5f4d6b05}
 If you have Horizontal Drilling stationing for the beginning or end of HDD, they need to
be entered in the database as Field Notes.
o Type will be Construction Note
o Description will be Begin HDD or End HDD
For all Edge of Pavement, Edge of Water:
RouteID Measure Status TYPE DESCRIPTION
{7c3947be-3223- 188811 Active Sheet Note Description: Edge of State Highway 123
485b-8fa0-
897001360d5f}
{a6f99c51-5fe3- 196021 Active Sheet Note Description: Edge of Cuyahoga River
40b2-a92c-
493f5f4d6b05}
 These may not be in the database at all. If you have alignment sheets that include Edge
of Water or Edge of Pavement, they need to be installed in the database.
 The examples above have Type as Sheet Note. This needs to be changed accordingly.
 Shorten the Description as much as possible
RouteID Measure Status TYPE DESCRIPTION
{7c3947be-3223- 188811 Active Edge of Edge of SH 123
485b-8fa0- Pavement
897001360d5f}
{a6f99c51-5fe3- 196021 Active Edge of Edge of Cuyahoga River
40b2-a92c- water
493f5f4d6b05}
For any miscellaneous or odd Field Notes, use your best judgment. If you’re unsure, ASK!


---


Liquids Standard for how sites should be labeled
Station Boundaries :
 Company Name - Site name – Station type
o Example: Centurion Pipeline L.P. - Andrews - Pump Station
Site Boundaries:
 Line Number - Location – site type
o Example: C24001.01 - Monroe - Injection Site
Gate Setting Boundaries:
 Line Number- Site type (Valve Number)
o Example: C580001 - Valve Site (V-300)
o Example: C580001 - Receiver Site (V-400)
M&R Boundaries:
 Line Number - Location – Site Type (Meter Number)
o 26001.01 – Ringgold - Meter Station (No: 45-43552)


---


Pipe Crossing Guidelines
“REMARK” shows in HelloSheets, not “Comments”
 Make as short as possible so the Alignment sheet isn’t cluttered
 Use “Comments”, “CROSSINGSIZE”, “Crossing Feature Type”/“Crossing Type”, “Material”, “Line
Clearance”, and “DEPTHOFCROSSINGFEATURE” to populate REMARK
 You will not be installing GForms for Foreign Line Crossings—only check the ones that have
already been installed and make sure all information is filled in.
NOTE: Line Clearance is in Inches, DEPTHOFCROSSINGFEATURE is in Feet, but both need to be in Inches
in REMARK
Fill out the following fields where information is given:
Status Measure RouteID Crossing Feature Type
Crossing Type Crossing Location Position Line Clearance
Depth of Pipe Depth of Crossing Feature Comments
Remarks From Date Owner Crossing Size
Material Angle Clearance
o Crossing Feature Type and Crossing Type should match
o Crossing Location and Position should match
o Line Clearance is in INCHES
o Depth of Pipe is in FEET
o Depth of Crossing Feature is in FEET
o From Date is the date of Installation of the Crossing. If the installation took more than one
day, you can use the To Date
o Crossing size is in INCHES
o Clearance is in FEET
For all “Foreign” Lines, Drain Tile, Fiber Optic/Power/Telephone/Television Cable, Sewer Line, and
Water Line:
Comments CROSSING Crossing Material Line Clearance DEPTHOFCROSSING
SIZE Feature FEATURE
Type
Description: 12” Water 12 Water Plastic 38 4.17
Line encased in plastic Line
sleeve; Source:
Maintenance Record
REMARK
12” Plastic Water Line (50” Cover, 38” CLR)
 If CROSSINGSIZE is <Null>, your REMARK should say
Unk Plastic Water Line (50” Cover, 38” CLR)


---


 If Material is <Null>, your REMARK should say
12” Water Line (50” Cover, 38” CLR)
 If you have information for Cover, but not Clearance, your REMARK should say
12” Plastic Water Line (50” Cover)
 If Line Clearance and/or DEPTHOFCROSSINGFEATURE are <Null>, your REMARK should say
12” Plastic Water Line
 If everything is <Null> except Crossing Feature Type, your REMARK should say
Unk Water Line
***If the Crossing is inside a casing, the Casing size and material should be in the Remark***
Example: 10” Water Line encased in 14” Concrete casing
14” Concrete Water Line (50” Cover, 38” CLR)
For Roads, Driveways, State Highways, Interstate Highways, Creeks, Rivers, Trails, and Railroads:
Comments CROSSING Crossing Material Line Clearance DEPTHOFCROSSING
SIZE Feature FEATURE
Type
Description: Barlow Rd.; <Null> Road <Null> <Null> <Null>
Source: Original LS;
Comments: Centerline
calc. from Edge of Road.;
Road Type: Road
Centerline
REMARK
CL Barlow Rd
 If the crossing is not located at the centerline of the River, Creek, etc., use “Edge of XX Creek” or
“West Bank XX River”
 If you have the name of the Creek, River, Trail, or Railroad, include that information in the Remark.
REMARK
CL Burlington Northern RR
REMARK
CL Cuyahoga River


---


For all Maintenance Records:
 Fill in as much information from the MR as possible. If a field is not filled in on the sheet, it can be
left blank in Arc
MR Field Arc Field
Depth of SPLP Depth of Pipe (in Feet)
Foreign Line Depth DEPTHOFCROSSINGFEATURE (in Feet)
Crossing Diameter CROSSINGSIZE (in Inches)
Clearance CLEARANCE (in Feet) / Line Clearance (in Inches)
Foreign Line Crossing Owner Owner
Crossing Type + Crossing Product Crossing Type / Crossing Feature Type
NOTE: DEPTHOFCROSSINGFEATURE is what will go in your REMARK for Cover, in INCHES
 Once the Pipe Crossing has been installed in Arc, mark it on the Tracking spreadsheet as Completed.
 If no stationing is provided or the lat/long does not fall in the right location, the MR can be marked
to be sent back to the author.
 When installing a Pipe Crossing, please enter the source and comments in the Comment field
o Example: Per MR IC-123-15, installed 12” Plastic Water line below
 As you’re installing Pipe Crossings, please check the crossings on the rest of the line to ensure all of
the existing records follow this format.
 The GIS File # naming format in the Tracking spreadsheet is:
Line number_beginning station (seven digits)_F (for Foreign Line Crossing)
Example: 12345_0123456_F
o If your stationing is less than 7 digits long, use zeroes before your station number
Example: Station 12+34 = 0001234
SAMPLE MAINTENANCE RECORD:


---


Boxes in Blue: Information used in the Tracking spreadsheet
Boxes in Orange: The lat/long you will use to find your crossing
Boxes in Green: Information you will enter into Arc
Boxes in Yellow: Information you can fill out in Comments in Arc


---


Please don’t leave the material field as “NULL or Unk”
PIPES/DETAIL PIPES (defaults):
Material – steel always, sometimes it changes on mainlines/detail to Poly or Flexsteel.
Pipe Grade - Unknown
SMYS - 24000
Wall Thickness - STD for the indicated OD
Pipe Specification - Unknown
Long Seam Type - Unknown (Pipe 4 in or less) or Unknown (Pipe over 4 in)
Installation Method - Trench (Mainline) or Insertion – on detail pipe we don’t really fill that out.
Girth Weld Type – SMAW – can change depends on the material
Heat Number – NULL -You may have the HEAT#, but not the MTR.
Manufacturer - Unknown
Mill Location - Unknown
Mill Test Pressure - NULL
Non-Controllable Fittings (defaults ): Dont including flanges.
Material - Unknown (match pipe) – correct, always steel, don’t leave that as unk
Heat Number - NULL
Manufacturer - Unknown
Subtype - always filled in
Style - Unknown
Angle - always filled in for elbows (otherwise NULL)
Roll Angle - filled in for elbows as applicable (otherwise NULL) – 90^ or 45^
Radius - NULL
Orientation - should always be Up, Down, Left or Right for elbows and reducers (Ahead only for
Flanges, Reducers, Caps) - correct
Rating Class - always NULL for elbows, tees, reducers and caps (Unknown for flanges)
Pressure Rating - always NULL for elbows, tees, reducers and caps (Unknown for flanges)
Grade - Unknown
Yield Strength – 24000


---


Specification - Unknown
Inlet/Outlet/wall Thickness - STD for the indicated OD
This is only for Flanges. Please check the fittings manual:
RATING CLASS: needs to populate (ANSI 600)
PRESSURE RATING: needs to populate (#1480)
The rest Null.
Controllable Fittings (defaults):
Material - Unknown (match pipe)
Heat Number - NULL
Manufacturer - Unknown
Subtype - always filled in
Tap Type - Unknown
Tapping Method - Unknown
Normal Position - Unknown
Present Position - Unknown
Pressure Rating - Unknown
Specification - Unknown
Valves (defaults): not for valves.
Barcode - NULL
Manufacturer - Unknown
Material - Unknown (match pipe) steel
Valve Type – Unknown - check the P&IDS if you recognize the symbols.
Asset Unit Code - always filled in
Operator Type - Unknown
Operator Model Number/Serial Number - NULL


---


Operator Manufacturer - Unknown
Rating Class - Unknown (only as a default)
Pressure Rating - Unknown (only as a default)
Inlet Pressure/Outlet Pressure (same value as Pressure Rating - otherwise NULL)
End Connect Inlet/End Connect Outlet - Unknown
Valve Use - Unknown
Normal Position - auto populates to Open (leave as default)
Present Position - same as Normal Position
Remote Operated - Unknown
Auto_Close_Ind - same as Remote Operated
Valve Section Source - Yes or No
Ancillary Role - Source if Valve section Source is Yes; otherwise Sink
Valves default:
Valve example
