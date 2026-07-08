Robot Dog Design

The design of the CAD model was performed in Onshape. The CAD file and images of the model are provided in the repository.
Dimension of the Robot:
    Main body:
        Base: 120mm x 60mm x 15mm
        Hip base: Diameter of 12mm and thickness of 5mm
        Hip length: 60mm x 5mm
        Leg length: 70mm x 3mm
    Arm:
        Base: Diameter of 20mm and thickness of 7mm
        Shoulder base: 10mm x 10mm x 11mm
        Shoulder length: 38mm x 4mm
        Elbow length: 30mm x 4mm
        Gripper length: 5.75mm x 1mm

For the main body each leg has a hip joint and a knee joint, therefore 2 DOF. The four legs has 8 DOF in total.
The Arm on the other hand has a base, shoulder, elbow and a gripper joint, which gives us 4 DOF.

Servo motors will be used for all the joints as they provide precise movements and are cost friendly.
The type of the Servo motors must be able to provide the sufficient torque needed.

Torque calculation for the hip joint:
    The mass of the joint is assumed to be uniformly distributed and the gravitational force as a concentrated force at the middle, furthermore
    the joint is assumed to have a mass of 0.1 kg. The angle between the gravitational force and the perpendicular line to the joint is 60°.
        joint length = 60mm
        joint mass = 0.1 kg
        τ = F * r = mg * r * cos(60)
        τ = 0.1 * 9.81 * 30*10^-3 * cos(60)
        τ = 0.0147 Nm

Without the robotic arm added the center of gravity would be slighty shifted towards the rear end of the chassis as the rear legs
are shifted towards the back, however with the arm added the center of gravity will be shifted a bit towards the middle.
The components that will be added should keep the center of gravity between the center and rear end of the chassis to prevent
the robot from tilting, especially during the movment of the arm.

The recommended walking method is one leg at a time, when a front leg moves it should be followed by the opposing leg on the rear side.
This method is the simplest and most stable.

Mechanical challenges:
    Servo motors may not provide enough torque if the robot becomes too heavy.
    The robotic arm shifts the center of gravity forward when extended.
    Batteries can move inside the chassis if not securely mounted.
    Feet may slip on smooth surfaces without rubber pads.
    
        
        
