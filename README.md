# Link-Prediction-In-Bipartite-networks
Link Prediction
Introduction
In this project, four Link Prediction algorithms, namely Common neighbors (CN), Jaccard (JC), Preferential attachments (PA), and Adamic Adar (AA), have been implemented to predict new links in bipartite networks. My article entitled "Computational Prediction of Probable Single Nucleotide Polymorphism-Cancer Relationships" explains more detailed explanations about these algorithms and their application in.
Dataset
The extension of the dataset file should be .xlsx and contain two columns. The first column is the first part of the network and the second column is the second part of the network.
How to use
Using these algorithms is very simple. First, the openpyxl package must be downloaded and installed. Then an object of the Link_Predition class must be created. In the next step, to read the dataset, the read_xlsx() method should be called, and the address of the desired dataset should be given to it. Then, to work with any of the above algorithms, you can call any of the PA() or CN() or JC(), or AA() methods. Finally, to write and save the results in the file, the write() method should be called, and the address of the storage location should be given to it.
Example
As an example, to predict the new links of the miRNA-Cancer bipartite network using the PA algorithm, we act as follows:
lp = Link_Prediction()
lp.read_xlsx(“C:\\ miRNA-Cancer.xlsx”)
lp.PA()
lp.write(“C:\\ predicted.xlsx”)
