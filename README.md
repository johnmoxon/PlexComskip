# PlexComskip

  added a ffmpeg command after the video parts are reassembled to convert to h264 and compress the video a bit
  using the following settings: "ffmpeg -i inputfile.mkv -crf 18 -map 0 -acodec copy -scodec copy -c:v libx264 -threads 0 -preset veryslow outputfile.mkv"

* moved ffmpeg command line switches to config file for customizing transcode options on the fly
