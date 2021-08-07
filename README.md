# BenchmarkNetworkSynthesis

Scenario definition based on which 500 networks were generated automatically.

## Description

The scenario-folder contains several files ending in .snippet, one ending in .header and, most importantly, the main.scenario file. The main.scenario file is the central point where the scenario is defined and other files are being included. The files ending in .snippet are frequently needed code fragments that are included at various occasions. The .header file contains configurational information for all executable actions.
Furthermore, a folder named "lib" is included. This folder contains all template files, that are used for element instantiation upon network generation. For better readability, all available actions have been grouped according to their purpose in the scenario. In this regard, all defenses are defined in the file "defender.template". All legitimate actions are defined in the file "default.template". While these would usually be defined in the context of the application that they belong to, this would require the interested reader to scan through all files. However, from a technical perspective, the benchmark network generator does not care where an action definition is located, so that definitions have been moved there. Similarly, all exploits that the attacker may use are defined in the file "attacker.template". All other files contain state descriptions and the high-level language instructions that take care of auto-diversification and the conditional upscaling that has been outlined in the dissertation.
