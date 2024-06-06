# VolmemAnalyzer
VolMemLyzer (Volatility Memory Analyzer) is a feature extraction module which use Volatility plugins to extract memory features to generate a CSV file for each memory snapshot.


Steps to install volatility3:

1. Download zip file using https://github.com/volatilityfoundation/volatility3  then unzip it.
2. ==> sudo apt install volatility3 
3. ==>  pip3 install -r requirements-minimal.txt
   in the volatility folder
4. ==> python3 setup.py build 
5. ==> python3 setup.py install
6. ==> pip3 install -r requirements.txt


Quick Start 
1. python3 vol.py -h
2. python3 vol.py -f /home/user/samples/cridex.vmem windows.info 

Other Pre-requisites
Out of all libraries used, only pandas library is not part of the Python standard library and must be installed separately using pip via:

  =>  pip install pandas

memory sample file link:
https://github.com/volatilityfoundation/volatility/wiki/Memory-Samples

Deployment
Step 1:
Complete pre-requisites and download the VolMemLyzer script from above to the desired folder. Navigate to the folder where the script was downloaded and initiate terminal/powershell in the folder.

Step 2:
Use the command given below:

==>   python3 VolMemLyzer-V2.py -f <Path to Memory Dump Folder> -o <Path to Output Folder> -V <Path to Volatility3>

The Placeholders should strictly follow:

Path to Memory Dump Folder - This should be an absolute path to the folder containing memory dump files. Ex: /home/user1/Desktop/MemoryDumps

Path to Output Folder - This should be an absolute path to the folder where the output.csv is to be stored. Ex: /home/user1/Desktop/VolMemLyzerOutput

Path to Volatility3 - This should be an absolute path to the vol.py file in the downloaded volatility folder from official Volatility3 Github. Ex: /home/user1/Desktop/Volatility3/vol.py



