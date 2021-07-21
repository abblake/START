# SMART Dynamic Strategy Tool ALPHA

**Welcome to SMART Github page!**  
Our intention in creating this Github page is to enable users to provide feedback about the SMART Tool. This includes but is not limited to additional variables, reporting known database issues, and/or reporting issues with the tool itself. Additionally, this Github page provides the R scripts for everything we use in the implementation  of the tool.   

  
  
Thank you!  
-Andrew, Oleg, Tim, and Aaron

**Notes on release:**  
The tool supports sample selection based on firms on the New York Stock Exchange. Future releases will support other stock exchanges based on need.  
**Notes on output:**  
The script will output two files. One file is a large dataset that includes ALL variables from the WRDS databases accessed. The second file will end with **_small** which includes the variables selected, firm information, and date information only.


## **DISCLAIMER**  
While the goal of this project is to standardize the data collection process for management students and scholars, the reality is that these archival datasets and methods for calculating some variables are not perfect. Below we list the known issues we are aware of as a word of caution. We also hope that you (the user or collaborator) can tell us about additional issues you've found in the data, suggest possible solutions, or provide even patches to the data (even a single line!). 

1. The CEOANN flag which indicates the executive is the CEO is sometimes blank or inaccurate.
2. The method for identifying CEO duality can sometimes be inaccurate (about 4% based on a sample of 2910 manually coded CEO duality variables). We are working on a method for flagging these for manual correction.
3. Duplicate records are removed using the gvkey and year variables (all databases). 
