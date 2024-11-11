# SCP - Containment Breach Ultimate Edition Reborn On Linux/SteamDeck

## Important Note: Please Report any Issues with the setup guide not listed in the common issues section directly to Me Not the UER Mod Devs. Only Report In-Game Bugs/Issues To The UER Devs.

![](Images/Setup/UER_Linux_Guide.png)

**Step 1**

Install Lutris and follow the instructions on their website for the device/distro you use, then download the installer for SCP CB UER Mod.

- **Lutris**: (*https://lutris.net/downloads*)

- **SCP Ultimate Edition Reborn Installer**: (*https://www.moddb.com/mods/scp-containment-breach-ultimate-edition/downloads/scp-containment-breach-ultimate-edition-reborn-setup*)


**Step 2**

**Open Lutris**:

![](Images/Setup/Lutris,_game_platform,_logo.png)

Go to the top left corner and **Click The Plus Symbol**, then a menu looking like this will pop up

![](Images/Setup/Step2.png)

Click the third option: "**Install a Windows game from an executable**"

Then a third menu will pop up asking you to name the game, **Name It Anything You Want**

After you named the game, **Click Install**

![](Images/Setup/Step2A.png)

After clicking install another menu will pop up showing you **The Installation Directory.**  **This is Important For Step 3, Make Sure You Remember Where the Directory/Folder Is.** 

Hit Continue:

![](Images/Setup/Step2B.png)

Then another menu will pop asking you to **Select The Setup File, Hit The 3 Dots And Navigate To The Directory Where The Installer Is And Select It, Hit Ok, And Hit Install**

![](Images/Setup/Step2C.png)

After Going through the setup **Launch The Game So It Will Generate An Options.ini file needed for Step 3**

![](Images/Setup/Step2D.png)

After Launching the game **you will get a Memory Access Violation, Dont Worry This Will Disapper after Step 3.**

![](Images/Setup/Step2E.png)

**Close The Game and Go Back to Lutris**

After going back to lutris, **Select the Game and Hit the Up Arrow next to Play and Select Configure.**

![](Images/Setup/Step2F.png)

After selecting configure a menu will pop with options to configure the game, Go to Game Options and **Click the Three Dots and Select the Game Executable then Hit Ok so *Common Issue 1* wont happen.**

**Step 3**

**Navigate to the directory where the Game/Wine prefix is**. It will look like this:

![](Images/Setup/Step3.png)

**Navigate and go through the following Directories/Folders:** *drive_c/users/"yourusername"/AppData/Roaming/scpcb-ue/Data*

After Getting to the directory/folder location, there will be a file called *Options.ini* 

![](Images/Setup/Step3A.png)

**Download The Pre-Configured Ini File from here in my repo and overwrite it with the on in the Data Folder** (*https://github.com/MrBonely/SCP-UER-Linux-SteamDeck-Setuo/blob/main/ini/options.ini*)

Also open up the ini file and make sure it looks like this:

![](Images/Setup/Step3B.png)

After Checking that, **Go Back to Lutris** and press play an it should start with no Memory Access Violation

![](Images/Setup/Step3C.png)


# Common Issues:

### 1. "Rmesh to load:"

![](Images/Setup/CommonIssue1.png)

**Fix:** Select the Game and Hit the Up Arrow next to Play and Select Configure, Go to Game Options and select the 3 dots then select the game executable and hit ok and close then the game should launch now.

**What Caused It?:** when you install a game on lutris it will automatically select the executable in the game directory. if there is multiple executables it will pick the first one A-Z so it picked Rmesh Viewer instead of the game executable