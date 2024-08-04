# 1. Stealing an Idea


# 2. 
AcQuIrE bAt(s) https://github.com/Enrop/RVC-test/releases/tag/v1.0

# 3. 
install -> https://www.python.org/ftp/python/3.10.11/python-3.10.11-amd64.exe

install -> https://github.com/git-for-windows/git/releases/download/v2.43.0.windows.1/Git-2.43.0-64-bit.exe

install -> https://aka.ms/vs/17/release/vs_BuildTools.exe with the optional boxes named "MSVC VS 2022" and "Windows 11 SDK"

# 4.
python tools/download_models.py if doesnt work go to https://huggingface.co/lj1995/VoiceConversionWebUI/tree/main/ and manually download the files

```
./assets/hubert/hubert_base.pt

./assets/pretrained 

./assets/uvr5_weights

Additional downloads are required if you want to test the v2 version of the model.

./assets/pretrained_v2

If you want to test the v2 version model (the v2 version model has changed the input from the 256 dimensional feature of 9-layer Hubert+final_proj to the 768 dimensional feature of 12-layer Hubert, and has added 3 period discriminators), you will need to download additional features

./assets/pretrained_v2

If you want to use the latest SOTA RMVPE vocal pitch extraction algorithm, you need to download the RMVPE weights and place them in the RVC root directory

https://huggingface.co/lj1995/VoiceConversionWebUI/blob/main/rmvpe.pt

    For AMD/Intel graphics cards users you need download:

    https://huggingface.co/lj1995/VoiceConversionWebUI/blob/main/rmvpe.onnx

```

https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI/blob/main/docs/en/README.en.md#preparation-of-other-pre-models

# 5.
You will always launch from bat's acquired in step 2 (1), unless you modify url to be from the standard repo, then you have a choice of continuing to grab custom ui from next step, and it changes how you'd launch.

# 6. 
If you want to use official repo change bat url from this repo to https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI and if you want the modifications i did after, manually go to https://github.com/Enrop/RVC-Edits/tree/NotPrebuilt press code, download as zip, and unzip in the final install, launch from EnropStart.bat

# 7.
if you care for realtime and dont want to install everything else, just use okada either from following https://rentry.co/VoiceChangerGuide this guide, and or felts github repo that installs it manually listed here https://github.com/MrFelt/voice-changer

# 8. 
Bonus tip, if you are on win11, and have the "Terminal" app, you can create a shortcut to your bat file of choice and change the target to the following line

%LOCALAPPDATA%\Microsoft\WindowsApps\wt.exe -w _quake "C:\Path\To\File.bat"

what this allows is the terminal app to be run in a quake window, aka a window that appears from the top of your screen, you can edit the keybind to toggle hide it from the terminal, thus having no visible window shown while training, or if voice changing only the PySimpleGUI or Chrome based browser tab if on Okada.
