Contact [Andrew Jansen](mailto:andrew.jansen@awe.gov.au)

#### Description

...

#### Labeling Guide
...

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
conda env create -f Ecoflow\notebooks\fishes\auto-ml-object-detection\ecoflow-auto-ml-object-detection_linux
conda activate ecoflow-auto-ml-object-detection
```

7. Download Workspace Config

[Download config.json from the Overview section of your workspace](https://docs.microsoft.com/en-us/azure/machine-learning/how-to-configure-environment#workspace)

8. Run Jupyter

```
> (ecoflow-auto-ml-object-detection)Ecoflow\notebooks\fishes\auto-ml-object-detection>jupyter notebook
```

9. Open ecoflow-auto-ml-object-detection.ipynb
