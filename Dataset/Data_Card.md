    library(tidyverse)

## Dataset title:

Tick collection summary per plot across habitat types

## Principal Data set Curator:

Gerardo Ramos

## Data statement author: Gerardo Ramos, MS graduate student, Swei Lab, Department of Biology, San Francisco State University

## Dataset Summary:

THE “Tick collection summary per plot across habitat types”, contains 63
observations each one representing a nymphal a plot where ticks were
collected. Ticks samples were collected from three natural protected
areas in the San Francisco Bay Area including Edgewood Park & Natural
Preserve (EW), China Camp State Park (CCSP), and Marin Municipal Water
District (MMWD) (San Mateo and Marin counties respectively). Within each
park there were plots set up along an oak woodland and annual grassland
gradient where ticks were collected using standard tick drags.
Occurrence data includes date suveyed, plot ID, site, replicate, hatitat
type, total larvae count, total nymph count, total adult count, count
for each life stage an species found (***Ixodes pacificus, Ixodes
spinipalpus, Dermocentor occidnetalis, Dermocentor similis,
Haemaphysalis leporispalustris***), average canopy percent cover,
average leaf litter depth, average grass height, and ***Ixodes
pacificus*** infection prevalence with ***Borrelia burgdorferi***.

## Languages:

English

## Data Instances:

A data point is composed of an individual plot where ticks were
collected using standard tick drags and includes tick count summaries
and environmental meta data. An entry would include the following
information:

    # Load dataset
    Tick_data<- read.csv("Plot_Data copy.csv",header=TRUE, stringsAsFactors = TRUE)

    # View the column names
    colnames(Tick_data)

    ##  [1] "Person.Doing.ID" "Date"            "Plot"            "Site"            "Replicate"       "Habitat"        
    ##  [7] "replicate"       "L"               "N"               "A"               "Field.notes"     "IPAC_L"         
    ## [13] "IPAC_N"          "IPAC_A"          "DEOC_L"          "DEOC_N"          "DEOC_A"          "DEVA_L"         
    ## [19] "DEVA_N"          "DEVA_A"          "HELP_L"          "HELP_N"          "HELP_A"          "ISPIN_L"        
    ## [25] "ISPIN_N"         "ISPINA"          "site"            "canopy"          "canopy..."       "leaf.litter"    
    ## [31] "grass.height"    "Plot.label"      "nymph_count"     "infected_nymphs"

## Curation Rationale:

Vector borne disease including Lyme disease are increasing at increasing
rate. There is a need to understand how Lyme disease is spread and
maintained in reservoir hosts and across the environment. Investigating
habitat edges is particularly important because they experience unique
environmental conditions that allow for unique reservoir host
communities which can structure a unique disease landscape.
Understanding this landscape is critical for the implementation of
mitigation techniques like acaricides and vaccines. It is also critical
for understand disease risk to humans in the future as land use change
and habitat fragmentation continues.

## Annotations:

The tick specimen, were collected from the field (China Camp State Park,
Edgewood Park and Preserve, and Marin Municipal Water District) and
brought back to Andrea Swei’s Lab at San Francisco State University for
identification to species, life stage and sex.

# Annotation process:

In lab, ticks were identified to life stage, species and sex for adults
using dichotomous keys unique for each life stage. The raw data was then
used to create a summarized version by plot.

# Who are the annotators?

Original collectors were graduate (MS) students while identifiers were a
combination of graduate and undergraduate students from at San Francisco
State University in Dr. Andrea Swei’s Lab.

# Personal and Sensitive Information:

Data set contains initials of people who curated the specimens.

# Social Impact of Dataset

Understanding disease risk across habitat edges is important for
creating a greater understanding about the transmission of vector borne
diseases. As land use change continues it is projected that humans will
be increasingly exposed to habitat edges and wildlife. For this reason
it is important to study these systems now, so that we can predict how
human communities will be impacted in the future.

Further understanding the disease dynamics in the environment through
this data set can also help inform tick control efforts like acaricide
and vaccine deployment.

# Discussion of Biases

Questing ticks are highly variable across the landscape meaning there is
a lot of zero counts in our data set.

Resources were limited, equal amounts of effort were put at collecting
samples at each park and habitat type. However sample sizes were of
nymphal ***Ixodes pacificus*** were limited.

# Other Known Limitations

Species identification may be inaccurate for some of the samples
especially between those species of the same genus because they have
similar morphological features.

# Dataset Curators

Swei Lab, Department of Biology, College of Science and Engineering, San
Francisco State University. Gerardo Ramos (Masters Student) is the main
point of contact for this data set.

\#Citation Information This work is licensed under a Creative Commons
Attribution 4.0 (CC BY 4.0)

# Contributions

Funding for this project came from Student Enrichment Opportunities
(SEO) at San Francisco State University and the National Institutes of
Health. Field work, data transcription, and infection testing was made
possible by Swei Lab graduate and undergraduate students.
