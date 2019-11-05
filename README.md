# PoetaQuae
Latin text classification

By Mackenzie Mitchell and Brendan Gilroy

## Overview

The goal of this project is to create a machine learning program to categorize what poet/author wrote a
given classic Latin text.

## Data
Data was web scraped using BeautifulSoup from:
-  http://rudy.negenborn.net/catullus/catullus2.htm
-  https://www.sacred-texts.com/cla/virgil/
-  http://www.perseus.tufts.edu

#### As observed, Cicero has many more data points (or documents) than the other poets. This would highly bias our classifier so we decided to remove Cicero to create more balanced classes:
![AuthorDistribution](https://github.com/mackenziemitchell6/PoetaQuae/blob/mackwip/Visuals/distributionWCic.png "Author Distribution")

#### Once Cicero was removed from the dataset, the classes were much more balanced:
![AuthorDistributionNew](https://github.com/mackenziemitchell6/PoetaQuae/blob/mackwip/Visuals/distributionNew.png "Author Distribution New")
 

The dataset contains:
- 118 personal/lyrical poems by Catullus (84-54 BC)
- 3 epic poems by Virgl (70-19 BC)
- 16 satirical poems by Juvenal (Late 1st Century-Early 2nd Century AD)
- 2 lyrical peoms by Horace (65-8 BC)
- 1 mythological peom by Ovis (65-8 BC)
- 1 historical prose piece by Caesar (100-44 BC)

#### Looking at the most frequenty used stop words in all of our corpus:
- -que : and
- -ne: negates statement and turns sentence into a question
- ex: Est Catullus: Catullus is here.
- ex: Estne Catullusque Cicero: Are Catullus and Cicero not here?
![StopCloud](https://github.com/mackenziemitchell6/PoetaQuae/blob/mackwip/Visuals/cloud.png "Stop Cloud")
