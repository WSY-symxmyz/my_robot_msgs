# msg
## LabwareOBB.msg
```
std_msgs/Header header
geometry_msgs/Pose pose
float32 x_length
float32 y_width
float32 z_height
```

## MovePose.msg
```
# For pose in move_line function
# [x,y,z,r,p,y] in unit [mm,mm,mm,rad,rad,rad]

float64[6] pose
```

#srv
## BeakerMani.srv
```
# input 
bool shake
---
# output
bool success
string message
```

## pHMeasure.srv
```
# input

float32 timeout_s
---
# output
bool success
float32 ph
string message
```

## PipetteDo.srv
```
# input 
string liquid # "HCl" or "water"
float32 volume_ul # Volume to aspirate
int32 tip_id
---
# output
bool success
string message
```

## TweezersDraw.srv
```
# input 
bool draw
---
# output
bool success
string message
```
