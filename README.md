# Alluvial Plot
Alluvial plots, also known as Sankey diagrams, are powerful data visualization tools that allow for the clear representation of flows or movements between different states or categories. These diagrams employ a streamlined visual metaphor akin to flowing liquids, where the width of the paths (known as "streams") is proportional to the quantity being represented.
In the context of microbial ecology and microbiome research, alluvial plots can be particularly useful for visualizing the distribution and flow of microbial species across different hosts or environments. For instance, the study by Liang et al. (2023) utilized an alluvial plot to illustrate the flow of known, novel, and novel without reference species across various hosts, including gorillas, humans, cattle, and goats. This approach provided a clear and intuitive representation of the microbial diversity and species distribution patterns observed in the study.
Similarly, the work by Jian et al. (2018) employed Sankey diagrams to visualize the flow of microbial communities between different environmental compartments, such as soil, air, and water. This type of visualization can help researchers identify potential sources, sinks, and pathways of microbial dispersal, which can be crucial for understanding the dynamics of microbial ecosystems.
According to the data visualization expert Cole Nussbaumer Knaflic, Sankey diagrams are particularly effective when the goal is to show the flow of a quantity from one set of nodes to another set of nodes, with the width of the streams representing the magnitude of the flow. This makes alluvial plots an ideal tool for representing the distribution and movement of microbial species across different hosts or environments, as they can clearly depict the relative abundances and transitions between different categories.
This Python code creates an alluvial plot, also known as a Sankey diagram, using the Plotly library. An alluvial plot is a type of flow diagram that visualizes the flow of data from one set of nodes to another set of nodes. In this particular example, the plot shows the flow of known, novel, and novel without reference species across four different hosts (Gorillas, Humans, Cattle, and Goats).

## Dependencies

The code requires the following Python libraries:

- `plotly.graph_objects`: This module from the Plotly library is used to create the alluvial plot.
- `plotly.io`: This module from the Plotly library is used to save the plot as a PDF file.

## Data

The code uses the following data:

- `hosts`: A list of host names (Gorillas, Humans, Cattle, and Goats).
- `known_species`: A list of known species counts for each host.
- `novel_species`: A list of novel species counts for each host.
- `novel_species_without_ref`: A list of novel species without reference counts for each host.

## Functionality

The code performs the following steps:

1. Import the required modules from the Plotly library.
2. Define the data (hosts and species counts).
3. Create the alluvial plot using the `go.Sankey` function from `plotly.graph_objects`. The plot shows the flow of known species, novel species, and novel species without reference from the hosts to three separate nodes.
4. Customize the plot layout by setting the title, font size, font family, and plot dimensions.
5. Save the plot as a PDF file named `alluvial_plot.pdf` using the `pio.write_image` function from `plotly.io`.
6. Display the plot using the `fig.show()` function.

### Customization

You can customize the plot by modifying the data and the plot layout in the script. The data is defined in the following variables:

- `hosts`: A list of host names.
- `known_species`: A list of known species counts for each host.
- `novel_species`: A list of novel species counts for each host.
- `novel_species_without_ref`: A list of novel species without reference counts for each host.

You can modify these variables to visualize different data.

The plot layout can be customized by modifying the `fig.update_layout` function call. You can change the title, font size, font family, and plot dimensions according to your preferences.

## License
This code is provided under the MIT License. Feel free to use and modify it according to your needs.


