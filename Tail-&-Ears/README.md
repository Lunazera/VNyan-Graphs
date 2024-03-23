# Tail & Ears

Responsive Tail and Ear controls!

Works through using pendulum chains to control bone rotations.
*currently vnyan has a bug that pendulum chains wont save the bone, rotation, or offset values. There are notes in the graph that have the info of what to put here.


## TailSway

Add dynamic tail movement to your model!
Requires two accompanying pendulum chains, TailSway and TailSwayY.

<b>SETUP:</b>
1. Load this graph, and the two pendulum chains.
2. In the chains, set the Avatar GameObject's to be your control bone for your tail. This bone must not have any other animators on it (like springbones)
3. Make sure the Transforms are Rotation Y and Z for the first chain's outputs, and Rotation X for the second chain output.
4. Change the Offset value for TailSway's first bone output if you want your tail to lean to either the left or right.

<b>Controls:</b>
• TailSpeed = base speed of your tail 
• TailMovement = amount/distance of tail movement
• TailWagAdd = how much smiling increases your tail wagging
• TailMovementReduce = how much heartrate reduces your tail movement (needs Pulsoid)

<b>Info</b>
• This is responsive to your model's head movement. It will try to move your tail to the opposite side that your model looks & follow your head tilt.
• This is also responsive to your smiling and heartrate! When ARKit smiling increases, your tail will start wagging faster and with more movement. As your heart rate increases, tail movement will reduce (so smaller movements).

You can toggle the smile-wagging and heartrate response off and on with the websockets below.

<b>Requirements:</b>Your tail bones must have at least one bone that does NOT have any springbone or dynamic bone applied to it.

## EarSway Wiggle 

This is a little extra thing that works with the EarSway Pendulums. It will periodically wiggle a random ear :3

To set up the EarSway Pendulum chains, just set the gameobject to be your control bones for your ears (they can't have springbones on that bone). 

The pendulums will tilt your ears along with your head, raise ears with eyebrow raising, and lower them with your brows down. Also will wiggle if you blink.
