# HTTP Adaptive Live streaming workshop

HTTP Adaptive Live Streaming workshop - build up MPD for MPEG-DAH and M3U8 fro HLS


##  Example mp4 video files
- 1080p mp4, 25 sec, 7MB
  -   http://workshop.jznight.net/101_1080p_25sec.mp4
- 720p mp4, 200 sec, 50MB
  - http://workshop.jznight.net/GOG_720p_200sec.mp4


## How to start?
- Install FFMPEG
  - http://www.ffmpegmac.net/
- Install Bento4
  - https://www.bento4.com/
  
- `source utility.func`
  - `transcode` ${input} ${output} ${bitrate} ${resolution}
  - `fragment` ${duration} ${input} ${output}
  - `hls_multiple_bitrate`    ${manifest_file_name} ${target_folder} ${input_file} [${input_file}]
  - `dash_multiple_bitrate` ${manifest_file_name} ${target_folder} ${input_file} [${input_file}]