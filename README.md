# FFMpeg-compress-videos
Compress videos using FFMpeg algorithm

## How to use the app
- Select source video files (.avi) to compress, or select folders where video files are stored. Video files will be searched in the folders and all subfolders. You can select multiple files and folders.
- All the video files found will be listed in the left listbox. From there, select the videos you want to compress and move them to the right listbox.
- Select:
  * Compression factor (between 1 and 51, default 25 corresponding to a compression of ~18 times)
  * Whether to delete source files or not. If you select Yes, you will be asked for confirmation (deafult is Don't delete)
  * Destination folder (default: destination folder is the same of the source video). Note: if you specify a folder, the same destination folder will be used for all videos regardless of their respective source folder.
  * A prefix or suffix can be added to the file name. If you specify any, the same prefix/suffix will be added to the file name of all videos.
- Start FFMpeg compression!
  * Compression will take 1-5 min per video. The output videos will be have .mp4 extension.

## Installation
- Download and install FFMpeg (http://ffmpeg.org/)
  * Follow [wikiHow](https://www.wikihow.com/Install-FFmpeg-on-Windows) or this [guide](https://github.com/adaptlearning/adapt_authoring/wiki/Installing-FFmpeg) for help installing FFmpeg.
- Download this repository.
- Run ffmpegsetup.m and follow its instructions to specify the path of the ffmpeg executable file.
