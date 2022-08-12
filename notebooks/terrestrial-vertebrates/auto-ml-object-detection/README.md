Owner [Adam McSorely](mailto:adam.mcsorley@environment.nsw.gov.au)

#### Description

28 classes of fauna from eastern NSW. 
Some class are amalgumations of species that are morphological inseperable on camera traps such as Common brush-tailed possums and mountain brush-tailed possums.
Images were collected from two NSW NPWS camera trapping projects. Wildcount and Vertebrate Pest Monitoring. 

#### Labeling Guide
All species identification were by expert staff. 
Bounding boxes were applied using the mega detector set at 90% confidence interval. 
A visual curation step was applied to removed images unsutable for training such as single legs in the bottom of frames

### Attribution

### Data Acquisition
Download [azcopy](https://docs.microsoft.com/en-us/azure/storage/common/storage-use-azcopy-v10) and decompress

Open a Command Prompt and change to the directry containg ```azcopy```

```
azcopy copy "https://ecoflow.blob.core.windows.net/public-terrestrial-vertebrates" "C:\Ecoflow\public-terrestrial-vertebrates"  --recursive
```
