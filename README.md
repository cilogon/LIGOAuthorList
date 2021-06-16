# LIGO AuthorList COmanage Registry Plugin

### Background
Twice per year, LIGO produces a list of authors that will be assigned to papers over the coming six months. There is a specific set of requirements that must be met to be eligible to be on the author list that involves the LIGO research percentage and the Total Work Contribution (TWC) of the person. LIGO research percentage and TWC are captured or calculated for each LSC member by the effort plugin and are defined in the LSC bylaws (https://dcc.ligo.org/DocDB/0008/M050172/021/LSC_Bylaws_v21.pdf). The requirements are:

 1) The person must be or have been a member of the LSC.
 2) The person must have a TWC of 0.2 or greater.
 3) The person must not be a short-term undergraduate student
 4) For the February list the person must additionally:
    a)  have joined the LSC prior to June 15 of the previous year and devoted at least 50% of their research effort toward LIGO since that date, or
    b) have been a past LSC Members who had earned authorship but has left the LSC (or have a LIGO research effort fell below the 50% level) after February 15 of the previous year.
 5) For the August list the person must additionally:
    a) have joined the LSC prior to December 15 of the previous year and devoted at least 50% of their research effort toward LIGO since that date, or
    b) have been a past LSC Members who had earned authorship but has left the LSC (or have a LIGO research effort fell below the 50% level) after August 15 of the previous year.
 6) An LSC member of former LSC member may petition to the spokesperson to be on the authorlist or may have their MOU PI do so on their behalf even if they do not meet requirements 2), 3) or 4).

### User story: Manage Author List for COU
COU Group Managers (MOU group managers) will go to an "authorlist management" interface in COmanage. If the current date is between Feb 15 and Aug 15, the interface will show all current members of the MOU group and past members of the MOU group who left the group after August 15 of the previous year. If the current date is between Aug 15 and Feb 15, the interface will show all current member of the MOU group and past members of the MOU group who left the group after February 15 of the previous year. In either case, those who are currenty projected to be eligible to be authors for the upcoming author list will be indicated. Projected eligibility for the next authorlist will be calculated as follows:
 - The person's current status (e.g. position), TWC and and LSC Research % will be assumed to be unchanged through to the date of the next author list
 - The average TWC over the appropriate period must be 0.2 or greater
 - If it is between August 15 and February 15
   - the person must have joined prior to June 15 of the previous year
   - the person must have an average LSC research percentage of at least 50% since June 15 of the previous year
 - If it is between February 15 and August 15
   - the person must have joined prior to December 15 of the previous year
   - the person must have an average LSC reserach perscentage of at least 50% since December 15 of the previous year
 
As well as projected eligibility, for each person listed the start date, end date (if they have left the LSC), current Resaerch Hours, LSC Research %, and TWC will be shown. For each person, there should be a button/checkbox/interface element that allows the COU group manager to petition to have the person added to the author list if they are not currently projected to be eligible and/or to be dropped from the author list if they are currently eligible. There should also be an indication of whether the petition is pending, rejected or successful.
 
 The Publications and Presentation Committee chair and those delegated by them as Author List Managers should have a different interface. 
 - should be able to handle add/drop petitions
 - should be able to order insitutions
 - should be able to generate a the required CSV files 
 - shoud be able to preview the authorlist
 
### User Story: Generate Author List
The CO or platform manager will generate a text report of all eligible members indicating authorship status. The user will indicate the end date of the time period in question (typically Feb or August 15) as well as options for sorting (by institution, by name, by authorship status), if non-authors should be included, and if verbose institution information should be included. 
The body of the report will include the following columns:
 
## Open questions
 1) Over what period is the TWC required to be 0.2? Averaged over the period since June 15 of the previous for the February list and over the period since Dec. 15 of the previous year for the August list? 
 2) Report output - what mechanism? Future reporting functionality in COmanage? Restful query?
