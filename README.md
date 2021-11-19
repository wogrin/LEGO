## Low-carbon Expansion Generation Optimization (LEGO) model

![LEGO's logo.](LEGO_Logo.png)

LEGO is a mixed integer quadratically constrained optimization problem and has been designed to be a multi-purpose tool, like a Swiss army knife, that can be employed to study many different aspects of the energy sector. Ranging from short-term unit commitment to long-term generation and transmission expansion planning. The underlying modeling philosophies are: modularity and flexibility. LEGO is also composed of thematic modules that can be added or removed from the model easily via data options depending on the scope of the study. You can use this code freely, but please cite our paper [1] if you do.

![LEGO's architecture.](LEGO_Module.png)

This version of Low-carbon Expansion Generation Optimization (LEGO) has been extended and includes:
* Freely available and code (and data examples) shared on Github. And there are some novelties.
* Flexibility:  1) operation only / TEP / GEP / GEPTEP ; 2) rMIP / MIP / MIQCP; 3) chronological hours / representative periods / load blocks
* Modularity:   1) considering/relaxing unit commitment decisions; 2) single-node / DC-OPF / AC-OPF (SOCP); 3) consider battery degradation via cycle aging costs; 4) rate of change of frequency system inertia constraints; 5) demand-side management (via load shedding and load shifting); 6) hydrogen sector
* Unique and versatile combinations of modules.

Its unique temporal structure allows LEGO to function with either chronological hourly data, or all kinds of representative periods. LEGO allows for modeling short- and long-term storage technologies with representative periods, e.g., long-term operation of large hydro reservoirs can be represented without having to renounce computational advantages of representative periods. Temporal flexibility and modularity of the model is something quite unique (that enables a plethora of many different studies) with one single model.

# Case Studies
* **LEGO-Base-Case-Study-7LRP**: Base case study for the model with stylized power system and 7 representative days.
* **LEGO-Base-Case-Study-Hourly**: Base case study for the model with stylized power system and chronological hourly representation of time horizon of one year.
* **EnStOpInvMo-7LRP-kmeans-net.xlsm**: Case study used in paper [[2]](https://doi.org/10.1016/j.apenergy.2020.115925) [This data file belongs to a preliminary version of the code and is no longer compatible with the current LEGO.gms file].

# References
[1] [S. Wogrin, D. Tejada-Arango, U. Bachhiesl, B.F. Hobbs, The full Low-carbon Expansion Generation Optimization (LEGO) model, available at arxiv http://arxiv.org/abs/2109.01368, and submitted to Applied Energy.]

[2] [S. Wogrin, D. Tejada-Arango, S. Delikaraoglou, A. Botterud, Assessing the impact of inertia and reactive power constraints in generation expansion planning, Applied Energy,
Volume 280, 2020, 115925, ISSN 0306-2619.](https://doi.org/10.1016/j.apenergy.2020.115925)
