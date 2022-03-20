# GrammarToolMacOS

This is the **MacOS** release version of the [GrammarTool](https://github.com/MarekLampas/GrammarToolSln) project.

[Avalonia](https://docs.avaloniaui.net/#supported-platforms) is supported on the following platforms:
- MacOS High Sierra 10.13 and higher

This repository contains 2 folders. One of them contains framework-dependent version of the application and the second one containd self-contained version.
Installation guide below describes installation of the framework-dependent version of the application, that requires installed **dotnet** framework taht can be downloaded from [Microsoft page](https://dotnet.microsoft.com/en-us/download/dotnet/5.0).

Self-contained version do not need dotnet to run but the instalation takes much more time. Installation of the self-contained version of the application is similar but in order to run the application you need to manualy allow all the libraries in the application.
Because of that I do not recomend to install the self-contained version and I recomend to install dotnet framework instead.

## Installation

0. You must have dotnet 5 installed on your MacBook. You can install it from [Microsoft page](https://dotnet.microsoft.com/en-us/download/dotnet/5.0).

1. Download this repository folder using *Code->DownloadZIP* button. (Then unzip it if needed)

![alt text](https://github.com/MarekLampas/DiplomovaPracaLatex/blob/main/sablona-cze/obrazky/releaseDownload.png "Download app")

2. Open terminal and go to **osx.10.12-x64** folder in downloaded folder.

```bash
cd ~/Downloads/GrammarToolMacOS-main/osx.10.12-x64
```

3. In order to run the application, you must mark the application file as executable.

```bash
chmod +x GrammarTool
```

4. Copy *Scanners* folder to user root folder.

```bash
cp -R Scanners ~/Scanners
```

5. Open **osx.10.12-x64** folder in downloaded folder using **Finder** and double-click on app executable file **GrammarTool**.

![alt text](https://github.com/MarekLampas/DiplomovaPracaLatex/blob/main/sablona-cze/obrazky/Finder.png "Open in Finder")

6. Pop-up warning will show up. You must click **Open** button.

![alt text](https://github.com/MarekLampas/DiplomovaPracaLatex/blob/main/sablona-cze/obrazky/WarningGrammarTool.png "Open app")

7. You must allow application to use some libraries. Because of that another pop-up warning will show up. You must click **OK** button.

![alt text](https://github.com/MarekLampas/DiplomovaPracaLatex/blob/main/sablona-cze/obrazky/WarnngLibAvaloniaNativeOK.png "Denied library")

8. Then you must open **System Preferences** and go to **Security and Privacy** tab.

![alt text](https://github.com/MarekLampas/DiplomovaPracaLatex/blob/main/sablona-cze/obrazky/SystemPreferences.png "System Preferences")

9. In **General** tab in **Allow apps downloaded from** section you will see *libAvaloniaNative.dylib*. You must allow it by clicking **Allow Anyway** button.

![alt text](https://github.com/MarekLampas/DiplomovaPracaLatex/blob/main/sablona-cze/obrazky/SecurityAndPrivacy.png "Security and Privacy")

10. Run the application again by double-click in Finder. Previous **warning pop-ups will show up few more times**.
You must allow all the libraries, because app needs them to run.
Libraries needed to run the app are: *libAvaloniaNative.dylib*, *libSkyaSharp.dylib*, *libHarfBuzzSharp.dylib*.

11. After allowing all the libraries, app should start normaly.
