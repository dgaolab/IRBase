# IRBase    
IRFinder Results for ~1500 Public-available RNASeq    

## Data Location:     
Please download the IRBase data from the following Google Clould Bucket: 
gs://irbase/IRBase.tar.gz
Then decompress it by: `tar -zxvf IRBase.tar.gz`
    
## File Description:    
1. "chrom.sizes" records human chromosome sizes.    
2. "known-genes.txt" records genes available in IRBase.    
3. "sample-tissue-list-clean.txt" records the tissue types of RNASeq libraries in IRBase.    
4. Each folder starting with "ERR" or "SRR" represents an RNASeq library. Note: there are 1483 RNASeq samples. But "sample-tissue-list-clean.txt" only annotates the cell types of partial of all samples. This is because some cell type information cannot be precisely extracted from SRA description. User needs to find their own way for enquiring the missing ones.    
    
## How to use:    
Inside each RNASeq library folder, there are 26 gzip files by alphabets. Each gzip file records IR of genes starting with that letter.     
For example, look for "B.gz" if you want to examine the IR value of an intron of BRCA.    
