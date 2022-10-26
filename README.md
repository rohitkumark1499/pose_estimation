# pose_estimation
Here we tried to detected different poses made by person using movenet/singlepose/lightning model 

the link to download model https://tfhub.dev/google/lite-model/movenet/singlepose/lightning/3

Inputs
A frame of video or an image, represented as an float32 tensor of shape: 192x192x3. Channels order: RGB with values in [0, 255].

Outputs
A float32 tensor of shape [1, 1, 17, 3].

The first two channels of the last dimension represents the yx coordinates (normalized to image frame, i.e. range in [0.0, 1.0]) of the 17 keypoints 
(in the order of: [nose, left eye, right eye, left ear, right ear, left shoulder, right shoulder, left elbow, right elbow, left wrist, right wrist, l
eft hip, right hip, left knee, right knee, left ankle, right ankle]).

The third channel of the last dimension represents the prediction confidence scores of each keypoint, also in the range [0.0, 1.0].


