# Amplicon Checker
Purpose: To check for amplicon coverage dropouts

# Goals:

Expected inputs:
* bam file
* primer scheme file --> determine amplicons based on it
* bam files of old samples to compare against (to set regional thresholds rather than a generic constant value)

What to base thresholds on:
* exact minimum coverage threshold
* minimum coverage as a percent of sample's highest coverage regions
* observed typical coverage in region based on older data

Potential outputs:
* list of regions (based on windows) with lower than threshold coverage
* List of amplicons (based on primers) containing any dropouts (by windows)
* List of amplicons (based on primers) fully dropped out
* pass/fail boolean