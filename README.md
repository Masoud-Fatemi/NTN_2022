# Nordic Twitter Network Dataset (NTN_2022)

## Overview
The NTN-2022 dataset is a comprehensive network data collection focused on Twitter user activities within the Nordic countries between November 2016 and November 2022.<br />
Contact: masoud[dot]fatemi[at]uef[dot]fi

## Usage
This dataset is intended for academic research and analysis focused on the empirical structure of social relations within the Nordic Twittersphere. Users are encouraged to cite our paper in any resulting work.

## Cite
M. Fatemi, S. Sieranoja, M. Laitinen, and P. Fränti, "Cluster Analysis of Nordic Social Media Users Based on Connection", *JOURNAL NAME and INFORMATION HERE*, 2024.


## Dataset Creation Process
The dataset was developed in 4 steps: user extraction, labelling, filtering, and tweet collection across the entire network. Here is a brief overview of the steps involved:
User Extraction: Initially, all Twitter users with tweets in the Nordic Tweet Stream (NTS) from November 2016 to November 2022 were extracted.
User Labeling: Users were then labelled based on the country from which they tweeted, focusing exclusively on the five Nordic countries. Users tweeting from more than one country (travellers) were excluded to maintain geographical consistency.
User Filtering: This step involves filtering out users based on several criteria:
Exclusion of users with uncertain locations or whose self-reported location did not match their tweet locations.
Removal of verified accounts to focus the dataset on regular users.
Filtering based on the network size, excluding users with more than 500 contacts, the top 1% most active, and the bottom 1% least active accounts.
Tweet Collection: For the final user list, we collected up to 3,200 of the latest messages per user, excluding retweets.
Once these steps finished, directed links were established based on interactional relationships, and only the largest connected component was retained.

## Dataset Composition
The NTN-2022 dataset comprises 15,794 nodes and 54,027 directed edges, representing user interactions. The dataset includes detailed country labels for each node, indicating the user's location among the five Nordic countries, with Finland and Sweden being the most represented.
A sample graph from the NTN-2022 dataset, featuring 3,273 nodes and 13,483 edges.

## Files Included
network.txt: Contains all nodes and directed edges from each node to others, detailing the user interactions within the network.
labels.txt: Includes node IDs and their corresponding country labels, identifying the Nordic country each user is associated with.

## Statistical Summary
Nodes: 15,794
Links: 54,027
Country Distribution: Most users are from Finland (37%) and Sweden (43%), with Iceland being the least represented (2%).




