# convert-rds-to-csv-in-R
#exporting ASVs table
````
setwd("D:/Marine_Iguanas_Project/MARINE_IGUANAS/NGS/RBCLbigdata/")
list.files()
table = readRDS("RBCL_merged_trans.rds")
write.table(table, "ASVs_RBCL_gemapisr_table.csv", sep = ",", quote = F, col.names = NA)
#this produces a csv table that appears saved in Documents, 
#open an excel book and use the option get data from text/csv, 
#the sequences will be in columns and the samples in rows
#select the sequences paste them transposing to another sheet
#then select the samples and number of reads and copy transposing to the other sheet
````
