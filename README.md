# FFMpeg-compress-videos
Compress videos using FFMpeg algorithm

![image](https://user-images.githubusercontent.com/29898879/110732527-54d13e80-81f2-11eb-92d8-a156a368ca5d.png)

## How to use the app
1. Select source video files (.avi) to compress, or select folders where video files are stored. Video files will be searched in the folders and all subfolders. You can select multiple files and folders.
2. All the video files found will be listed in the left listbox. From there, select the videos you want to compress and move them to the right listbox.
3. Select Destination folder (default: destination folder is the same of the source video). Note: if you specify a folder, the same destination folder will be used for all videos regardless of their respective source folder.
4. A prefix or suffix can be added to the file name. If you specify any, the same prefix/suffix will be added to the file name of all videos.
5. Select whether to delete source files or not. If you select Yes, you will be asked for confirmation (deafult is Don't delete).
   * For some reason, I do not get the "delete source files" to work, delete will fail for permission denial, even with Matlab running as administrator or executing fclose('all') before delete.
6. Select the compression factor (between 1 and 51, default 25 corresponding to a compression of ~18 times)
   * A compress factor of 20 (about 10 times) should be fine in most cases. 
7. Start FFMpeg compression!
   * Compression will take 1-5 min per video. The output videos will have .mp4 extension.

## Installation
- Download and install [FFMpeg](http://ffmpeg.org/)
  * Follow [wikiHow](https://www.wikihow.com/Install-FFmpeg-on-Windows) or this [guide](https://github.com/adaptlearning/adapt_authoring/wiki/Installing-FFmpeg) for help installing FFmpeg.
- Download this repository.
- Run ffmpegsetup.m and follow its instructions to specify the path of the ffmpeg executable file.

## Dependencies
- [FFMpeg Toolbox](https://www.mathworks.com/matlabcentral/fileexchange/42296-ffmpeg-toolbox) (already included in this repository)
- [uipickfiles: uigetfile on steroids](https://www.mathworks.com/matlabcentral/fileexchange/10867-uipickfiles-uigetfile-on-steroids) (already included in this repository)
