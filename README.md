# Neverwinter Build Compare Tool
This is a tool to compare Neverwinter builds, created in [Rainer's Character Builder](https://www.patreon.com/RainerNW).
It's a macro-enabled Microsoft Excel spreadheet, that loads two .cbf files and higlights the differences.
It is typically used to compare your current build vs your target build and to track your progress.

## Warning!
This spreadsheet contains VBA code. The code is mostly harmless and it is used to automatically parse and load the .cbf files into appropriate tab. When you run the spreadheet, you will be prompted to "Enable Editing" and "Enable Content", which is recommended, so you can just load the .cbf files using the buttons. If you don't feel comfortable enabling content (which is fair enough, I am just a random dude from the internet after all), you can still use the tool, but you will need to load the .cbf files manually (which is more involved). 

Here is how:

1. In the spreadsheet, select the "Base" tab.
2. Hit Ctrl+A and Delete - to delete the content of the sheet.
3. Find your baseline/current .cbf file and open it in Notepad (or any other text editor).
4. Hit Ctrl+A and Ctrl+C - to copy the content of the file into Clipboard.
5. Go back to the spreadsheet, click on the arrow down under the "Paste" icon and select the "Text Import Wizard" ![Text Import Wizard](/images/PasteTextImportWizard.PNG)
6. Click "Next", and on Step 2 screen, click on "Other:" and enter equal sign ("=") into the little box. ![TIW - Step 2](/images/TextImportWizardStep2.PNG)
7. Click "Finish" - this should load the content of the .cbf file into the "Base" tab.
8. Repeat the steps 1-7 for the "Target" tab and your target build .cbf file.

Congratulations, the "Compare" tab is now showing the differences between the two builds.
