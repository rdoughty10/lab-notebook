This sheet describes work and methods relating to our work in response to work done in industry on biothreats detection. This includes a description of the initial problem, an overview of the problems we were having, and the efforts to solve such issues.

### Background + Overview of the challenge
USENIX is a security conference, and an industry competitor (Raytheon) was developing a new tool to rival seqscreen. They developed a dataset in which they took bacterial toxins and split them, in a way that could be used to realistaclly develop a bioweapon. More biological details aren't particularly necessary, but in short, they describe a scenario in which one could splice a toxin and insert a benign sequence such that the sequences passes security checks. This benign sequences could then be cut out using some form of restriction enzyme and then become toxic once again. 

They tested their tool, as well as seqscreen and a few others, on this dataset, and returned results to us that showed seqscreen was performing really poorly (70-80% sensitivity). In short the reason this was happening was twofold:
-  They used seqscreen incorrectly (not up to sequences screening guidelines)
- Sometimes seqscreen would not correctly identify the toxin (specifically in ONT mode)


#### Daily Notes Information
[[2025-01-02]] Updates on full runs of seqscreen on toxin datasets, including how and where things were run. Also includes early detail about the outcomes of the k=4 run. 
[[2025-01-03]] Updates on the results of the full runs on toxin datasets with windowed mode and the ONT k=4 run. 
