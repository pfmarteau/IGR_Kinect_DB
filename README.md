# IGR_Kinect_DB

## Descrition:
The IGR_Kinect_DB is a Kinect captured gesture database dedicated to Isolated Gesture Recognition. Its purpose is to evaluate 
the recognition the hand-shape and the upper body movement using 3D positions of skeletal joints captured using a Microsoft 
Kinect 2 sensor. 

20 subjects have been selected (15 males and 5 females) to perform in front of the sensor (at a three meters distance) 
the six selected NATOPS gestures. Each subject repeated each gesture three times. 
Hence the isolated gesture dataset is composed of 360 gesture utterances that have been manually segmented to a fixed length 
of 51 frames.

## Citation Request
If you use this dataset, please cite the following paper:

    Nehla Ghouaiel, Pierre-François Marteau, Marc Dupont, 
    Continuous pattern detection and recognition in stream - a benchmark for online gesture recognition
    International Journal of Applied Pattern Recognition, 2017, 4 (2), 〈10.1504/IJAPR.2017.085315〉

## File format:
<subject_id> <gesture_id> <frame_1> <frame_2> .... <frame_N>
...

<subject_id> <gesture_id> <frame_1> <frame_2> .... <frame_N>
eof


i=1..N, <frame_i>=<x_1 x_2 ... x_24>


i=1..24, x_i in list of features (24), in the following order:
			X,  Y,  Z
Hand tip left :		1,   2,  3
Hand tip right : 	4,   5,  6
Thumb left : 		19, 20, 21
Thumb right : 		22, 23, 24
wrist left :		13, 14, 15
wrist right :		16, 17, 18
Elbow left : 		7,   8,  9
Elbow right : 		10, 11, 12
