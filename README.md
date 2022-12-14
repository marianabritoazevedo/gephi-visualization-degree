# Fifa World Cup 2022 - Degree Visualization

## About this repository
This repository aims to build an interactive page for viewing a network referring to Wikipedia searches related to the `2022 FIFA World Cup`.

For this, the [Gephi](https://gephi.org/) software was used, responsible for the construction and styling of the network, as well as the production of files related to the interactive page, through the `SigmaExporter` plugin of this tool.

This repository represents only a part of the final work developed in the Data Structure II discipline, done by [Mariana Azevedo](https://github.com/marianabritoazevedo), [Morsinaldo Medeiros](https://github.com/Morsinaldo) and and [Thaís Medeiros](https://github.com/thaisaraujo2000). The complete work can be checked at [this link](https://github.com/marianabritoazevedo/data-structure-ii).

:mag_right: You can check the interactive page with [this link](https://marianabritoazevedo.github.io/gephi-visualization-degree/network/).

![Img copa](https://mundoconectado.com.br/uploads/chamadas/copa-2022_2.jpg)

## About the network

This network was built using the Python `wikipedia` library, using the term `2022 FIFA World Cup` as the search root, and then searching all links related to that term on Wikipedia pages.

The original network had approximately 79.000 nodes and 214.000 edges, so this network was too large to produce a good visualization. In this way, a filtering was carried out, keeping only the nodes with degree greater than or equal to 100, and thus, the final network had 460 nodes.

Then, using the `pandas` library, the data was divided according to the degree into 5 different groups:

*  $Group 1: 100 \leq degree \leq 199 $
*  $Group 2: 200 \leq degree \leq 299 $
*  $Group 3: 300 \leq degree \leq 499 $
*  $Group 4: 500 \leq degree \leq 699 $
*  $Group 5: 700 \leq degree \leq 1369 $
