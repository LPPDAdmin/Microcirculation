S1. Synthetic model "S1" for the somatosensory cortex with 66090 nodes and 70800 edges
<img width="2062" height="2242" alt="S1_graph" src="https://github.com/user-attachments/assets/da8004ef-4a79-4061-a220-ab94c7d9e3a8" />
Load dataset in MATLAB, instantiate as graph, and visualize with the script "demo_load_S1.m"  
References for the mouse cortical vascular networks  
1.	Jamshidi, M., T. Ventimiglia, P. Sudres, C. Zhang, F. Lesage, W. Rooney, D. Schwartz, and A A. Linninger. "Impact of stalling events on microcirculatory hemodynamics in the aged brain." Microcirculation, 31 (3) (2024), e12845. PMID: 38265175  

Data files  
.pMx = size N x 3 point coordinate matrix where N is the number of graph nodes. First, second, and third columns are x, y, and z coordinates in µm respectively.  
.fMx = size M x 5 face connectivity matrix where M is the number of faces (graph edges). The first column contains positive integers indicating anatomical edge labels according to the following key:  
	150 = pial arteries  
	151 = penetrating arterioles  
	152 = pre-capillary arterioles  
	153 = artery-side capillaries  
	154 = arterio-venous closure  
	250 = pial veins  
	251 = ascending venules  
	252 = post-capillary venules  
	253 = venous-side capillaries  
The second and third columns contain indices to rows of the .pMx file and refer to the initial and terminal points of each edge in the (directed) graph respectively. By default, the fourth and fifth columns are all zeros. 
dia = size M x 1 vector of vessel diameters in µm where M is the number of graph edges.  

Updated by TV/AL 9/18/2026
