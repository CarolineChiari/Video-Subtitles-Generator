# Video Subtitles Generator
 
- [Video Subtitles Generator](#video-subtitles-generator)
  - [Introduction](#introduction)
  - [Requirements](#requirements)
    - [Creating an Azure Cognitive Service instance](#creating-an-azure-cognitive-service-instance)
    - [Getting the key](#getting-the-key)
  - [How to use the notebook](#how-to-use-the-notebook)

## Introduction

If you want to generate subtitles for your video, you can use this notebook. All you need, is your input video file.

## Requirements

In order to fun the notebook, you will need to have an Azure Cognitive Services instance, and a key.

### Creating an Azure Cognitive Service instance

- Log into the [Azure portal](https://portal.azure.com)
- Create a new resource group for your resources
- Click on the **+** at the top of the resource group to create a new resource.
- Look for **Cognitive Services** and click on it.
- Click **Create**.
- Make sure to select the proper resource group and region.
- Give your service a name and click **Review + Create**.

### Getting the key

- Click on your Azure Cognitive Services instance.
- In the left pane, click **Keys and Endpoints**.
- Copy one of the two keys.
- Make note of the region.

## How to use the notebook

1. Download ffmpeg from [here](https://www.ffmpeg.org/download.html) and put it in the ffmpeg folder.
2. Create a *.env* file in the same folder with the following content:
```
SPEECH_KEY=<your-speech-key>
SPEECH_REGION=<your-speech-region>
SPEECH_FILE=<your-source-video-file-path>
SPEECH_LANGUAGE=<your-speech-language>
```
3. Open the notebook in Jupyter Notebook/VS Code.
4. Run all cells. I would recommend you run the cells one at a time and read the outputs/comments your first time around.
