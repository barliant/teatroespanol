# teatroespanol: Spanish Golden Age Drama Analysis

This repository contains experimental, derivative data from some initial analyses into the network structure of Spanish Golden Age drama. Specifically, some data about 10 plays by Tirso de Molina and 10 plays by Calderón de la Barca. 

* "myzf" = Data abstracted from the full plays as data about each speech, in the form of a csv file
* "matrices" = Further abstraction as an adjacency matrix (speaker x speaker) as a csv file
* "graphs" = Same information as in the matrices, but in the gexf (XML) format suitable for networkx
* "plots" = visual representation of the data in "graphs", with a threshold of 100 words for a valid interaction

Python scripts used

* See <https://github.com/cligs/toolbox/tree/master/network>

Methodological note

* Spanish plays from the Golden Age (Siglo de Oro) do not always have act divisions and virtually never have scene divisions. Also, stage directions indicating characters entering or exiting the stage are usually not systematic. As a result, it is not immediately possible to model character interaction on the basis of joint presence on stage in the space of a single scene or configuration. Therefore, character interaction is modelled here as immediately subsequent speech, i.e. focused entirely on who responds to whom. The next step will be to investigate how network characterstics change when a larger moving window of interaction is defined.   
