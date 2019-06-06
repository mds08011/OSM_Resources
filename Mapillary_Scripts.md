#### Linux Upload


#### Windows Upload Photos


#### Windows Upload Videos

C:

Video Sampling and Upload
- Sample the video(s) located in path/to/videos into the directory path/to/images, at a sample interval of 0.5 seconds and tag the sampled images with capture time. Note that the video frames will always be sampled into sub directory .mapillary/sampled_video_frames/"video_import_path", whether import path is specified or not. In case import_path is specified the final path for the sampled video frames will be "import path"/.mapillary/sampled_video_frames/"video_import_path" and in case import_path is not specified, the final path for the sampled video frames will be path/to/.mapillary/sampled_video_frames/"video_import_path".

`mapillary_tools sample_video --import_path "Z:\Malcolm\OSM\StreetLevelImagery\Waylens\2019-06-06\Mapillary\Images" --video_import_path "Z:\Malcolm\OSM\StreetLevelImagery\Waylens\2019-06-06\Mapillary\Videos" --video_sample_interval 1.0 --advanced `

