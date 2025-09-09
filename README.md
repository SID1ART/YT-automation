# YT-automation
Creating YouTube videos using n8n automation

In this workflow, you must upload your script for the video to be generated; it will be broken into chunks for further image generation. For audio, you can manually upload the audio file for the voiceover for the video or add the audio generation node according to your preference.

The audio duration is transcribed from the file, which is further used to trim the video for each scene equally

Ai agent is used for generating the image generation prompt, which the Flux Schnell model further uses to generate images.

Once all the images are created, the video is created(zoom in effect in each image for that particular scene), all videos are aggregated and combined for a single video

At last, the audio has been added to the video 

Your YouTube video is ready

NOTE - You can customize the workflow according to your needs, from generating voiceover to images(size, models, theme) to image prompts
     - This is executed using Docker-installed NCA-toolkit(ffmpeg included in it)
