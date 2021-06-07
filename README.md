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

### User story
COU Group Managers (MOU group managers) will go to an "authorlist management" interface in COmanage. If the current date is between Feb 15 and Aug 15, the interface will show all current members of the MOU group and past members of the MOU group who left the group after August 15 of the previous year. If the current date is between Aug 15 and Feb 15, the interface will show all current member of the MOU group and past members of the MOU group who left the group after February 15 of the previous year. In either case, those who are currenty eligible to be authors for the upcoming author list will be indicated. Eligibility for the next authorlist will be calculated as follows:

## Open question
1) Over what period is the MWC required to be 0.2? Averaged over the period since June 15 of the previous for the February list and over the period since Dec. 15 of the previous year for the August list? 
