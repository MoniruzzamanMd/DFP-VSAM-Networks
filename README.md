# Human Action Recognition by Discriminative Feature Pooling and Video Segment Attention Model
# Abstract
We Introduce a simple yet effective network that embeds a novel Discriminative Feature Pooling (DFP) mechanism and a novel Video Segment Attention Model (VSAM), for video-based human action recognition from both trimmed and untrimmed videos. Our DFP module introduces an attentional pooling mechanism for 3D Convolutional Neural Networks that attentionally pools 3D convolutional feature maps to emphasize the most critical spatial, temporal, and channel-wise features related to the actions within a video segment, while our VSAM ensembles these most critical features from all video segments and learns (1) class-specific attention weights to classify the video segments into the corresponding action categories, and (2) class-agnostic attention weights to rank the video segments based on their relevance to the action class. Our action recognition network can be trained from both trimmed videos in a fully-supervised way and untrimmed videos in a weakly-supervised way. For untrimmed videos with weak labels, our network learns attention weights without the requirement of precise temporal annotations of action occurrences in videos. Evaluated on the untrimmed video datasets of THUMOS14 and ActivityNet1.2, and trimmed video datasets of HMDB51, UCF101, and HOLLYWOOD2, our network achieves promising performance, compared to the latest state-of-the-art method.
# Overview of our approach
![Overview](https://user-images.githubusercontent.com/59179258/214441791-1b79abbc-dea2-45e0-992a-24031cf31370.png)

# Video clips, video segments and feature representation generation.
![Clips_Segments_Feature](https://user-images.githubusercontent.com/59179258/214441821-1837b0ce-d8f5-47f0-8f01-6216a7f9e9e4.png)

# Discriminative feature pooling mechanism in a video segment.
![DFP](https://user-images.githubusercontent.com/59179258/214441852-eb063b58-0acf-4440-8730-a2681f6e3c4c.png)

# Video segment attention model (VSAM).
![VSAM](https://user-images.githubusercontent.com/59179258/214441868-0e6b129a-c0c3-4fc9-9518-8b55daa4a504.png)
