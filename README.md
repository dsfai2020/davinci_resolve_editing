DAVINCI RESOLVE EDITING

Git Large File Storage (LFS) is an extension of Git that helps manage large binary files more efficiently within a Git repository. It's especially useful for version controlling multimedia assets, such as video files, images and Audio.

First:
	In the effects tab, right click and create a fusion composition.

Next:
	Drag the fusion composition into the edit tab.  Right click it and open it up in the fusion page.

Next:
	Inside of the Fusion page, make sure that the correct fusion is displaying.  Once you like it, select File, Export, Fusion Composition and save it in a folder that you will house future compositions in.

Finally:
	If you would like to use this fusion comp again in other projects all you have to do is go to File, Import, Fusion Composition and locate the file that .comp file that you need.

This Repository uses Git LFS to manage Fusion Compositions.  
If you'd like to get started from scratch using your own repository you can Either fork this repostiory or run the following commands.

First:
	Use git init to create a repository.  Make sure to do this in a folder that will house all of your Fusion Compositions.

Next:
	git lfs install
	
Next:
	git lfs track "*.comp"
	This will track all of the .comp files.  Which are the files that we want to target since that is type that Fusion Compositions are saved as.

Next:
	git add .gitattributes
	git commit -m "Enable Git LFS for .comp files"

Next:
	git add name_of_your_composition_file.comp

Next:
	git commit -am "Updated the Fusion Comp"


Assuming that you've already configured a Remote follow these steps:

Next:
	git push -u origin main
	(origin is your remote id that you created when you configured at remote.  main is the name of the current branch)

IF you're not sure that you have git lfs installed run the following commands in the terminal.
	git lfs version
	git lfs status

 ![image](https://github.com/dsfai2020/davinci_resolve_editing/assets/60169737/3f5366bf-fe2d-455e-ba7c-b41ba899c7e0)
