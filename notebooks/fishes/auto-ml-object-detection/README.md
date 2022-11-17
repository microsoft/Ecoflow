Owner [Andrew Jansen](mailto:andrew.jansen@dcceew.gov.au)

#### Description
This dataset includes 44,112 images with 82,904 bounding box annotations for 23 tropical freshwater fish taxa from northern Australia.

Images were derived from Remote Underwater Video (RUV) deployments in deep channel and shallow lowland billabongs, Kakadu National Park, Northern Territory Australia. RUV deployments were conducted during the Supervising Scientists annual fish monitoring program in the 2016, 2017 and 2018 recessional flow period (dry season).

•	All images are in .jpg format and are 1920x1080 in dimension.

•	Bounding box annotations are in COCO format.

Fish taxa include:

```
Ambassis agrammus
Ambassis macleayi
Amniataba percoides
Craterocephalus stercusmuscarum
Denariusa bandata
Glossamia aprion
Glossogobius spp.
Hephaestus fuliginosus
Lates calcarifer
Leiopotherapon unicolor
Liza ordensis
Megalops cyprinoides
Melanotaenia nigrans
Melanotaenia splendida inornata
Mogurnda mogurnda
Nemetalosa erebi
Neoarius spp.
Neosilurus spp.
Oxyeleotris spp.
Scleropages jardinii
Strongylura kreffti
Syncomistes butleri
Toxotes chatareus
```

#### Labeling Guide
To speed up the labelling process and define what makes a "good" annotation for model training we developed the following criteria to standardise labelling across multiple users, projects and geographical regions.

1. Key features, fish were only labelled if key defining characteristics for species level identification were visible in the image, such as colouration or morphology.

2. Orientation, fish directly facing toward or away from the camera were not labelled, as key features are often obscured making species level identification difficult.

3. Depth, as fish move further away from the camera, ability to confidently identify reduces. Orientation combined with deteriorating light and turbidity makes species level identification difficult. Annotations were only made in clear conditions where the above criteria were also met.

4. Obstruction, if a fish was obscured by debris, aquatic vegetation or other fish, bounding boxes are not overlapped or separated into two boxes.


#### Azure Deployment

1. Deploy Azure Machine Learning

    [![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2Fquickstarts%2Fmicrosoft.machinelearningservices%2Fmachine-learning-workspace%2Fazuredeploy.json)

2. [Install Anaconda](https://www.anaconda.com/products/distribution)

3. Clone the Ecoflow repository

    Using Anaconda Prompt

```
git clone https://github.com/microsoft/Ecoflow.git
```

4. Create and activate environment

```
conda env create -f Ecoflow\notebooks\fishes\auto-ml-object-detection\ecoflow-fishes-auto-ml-object-detection_linux.yml
conda activate ecoflow-fishes-auto-ml-object-detection
```

7. Download Workspace Config

    [Download config.json from the Overview section of your workspace](https://docs.microsoft.com/en-us/azure/machine-learning/how-to-configure-environment#workspace)

8. Run Jupyter

```
> (ecoflow-auto-ml-object-detection)Ecoflow\notebooks\fishes\auto-ml-object-detection>jupyter notebook
```

9. Open ecoflow-fishes-auto-ml-object-detection.ipynb
