# Nordic Twitter Network (NTN_2022)

## Overview
The NTN-2022 dataset is a network dataset focused on Twitter users within the Nordic countries between November 2016 and November 2022.
<br />
<br />
Contact: [masoud.fatemi@uef.fi](masoud.fatemi@uef.fi)

## Usage
This dataset is intended for academic research and analysis focused on the empirical structure of social relations within the Nordic Twittersphere. Users are encouraged to cite our paper in any resulting work.

## Cite
M. Fatemi, S. Sieranoja, M. Laitinen, and P. Fränti, "Cluster Analysis of Nordic Social Media Users Based on Connection", *JOURNAL NAME and INFORMATION HERE*, 2024.

## Dataset Creation Process
The dataset was developed in 4 steps: **user extraction**, **labelling**, **filtering**, and **tweet collection** across the entire network. Here is a brief overview of the steps involved:
<br />
  1. **User Extraction:** Initially, all Twitter users with tweets in the [Nordic Tweet Stream (NTS)](https://erepo.uef.fi/handle/123456789/6697) from November 2016 to November 2022 were extracted.
  2. **User Labeling:** Users were then labelled based on the country from which they tweeted, focusing exclusively on the five Nordic countries. Users tweeting from more than one country (travellers) were excluded to maintain geographical consistency.
  3. **User Filtering:** This step involves filtering out users based on several criteria: <br />
    - Exclusion of users with uncertain locations or whose self-reported location did not match their tweet locations. <br />
    - Remove verified accounts to focus the dataset on regular users. <br />
    - Filtering based on the network size, excluding users with more than 500 contacts, the top 1% most active, and the bottom 1% least active accounts. <br />
  5. **Tweet Collection:** For the final user list, we collected up to 3,200 of the latest messages per user, excluding retweets.
<br />
Once these steps finished, directed links were established based on interactional relationships, and only the largest connected component was retained.

## Dataset Composition
The NTN-2022 dataset comprises XXX nodes and XXX directed edges, representing user interactions. The dataset includes detailed country labels for each node, indicating the user's location among the five Nordic countries(FI=Finland, SE=Sweden, NO=Norway, DK=Denmark, IS=Iceland), with Finland and Sweden being the most represented.
<be />
**NOTE**: For privacy reasons, the collected tweets will not be made public, and user IDs have been anonymized.

## Files Included
- **network.txt:** Contains all nodes and directed edges from each node to others, detailing the user interactions within the network.
- **labels.txt:** Includes node IDs and their corresponding country labels, identifying the Nordic country each user is associated with.

## Statistical Summary
**Nodes:** XXX <br />
**Links:** XXX <br />
Country Distribution: Most users are from Finland (37%) and Sweden (43%), with Iceland being the least represented (2%).




