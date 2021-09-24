# Cpp_ConcurrentTrafficSimulation_L3
This is a training for writing a concurrent program in C++

## The Project's Description:

### Project Tasks
**Task L1.1 :** In class WaitingVehicles, safeguard all accesses to the private members _vehicles and _promises with an appropriate locking mechanism, that will not cause a deadlock situation where access to the resources is accidentally blocked. \

**Task L1.2 :** Add a static mutex to the base class TrafficObject (called _mtxCout) and properly instantiate it in the source file. This mutex will be used in the next task to protect standard-out.\

**Task L1.3 :** In method Intersection::addVehicleToQueue and in Vehicle::drive() ensure that the text output locks the console as a shared resource. Use the mutex _mtxCout you have added to the base class TrafficObject in the previous task. Make sure that in between the two calls to std::cout at the beginning and at the end of addVehicleToQueue the lock is not held. \

You can find these tasks in the project_tasks.txt within the workspace as well.

### Build Instructions
To compile and run the code, create a build directory and use cmake and make as follows:
../L1_Project# mkdir build \
../L1_Project# cd build \
../L1_Project/build# cmake .. \
../L1_Project/build# make \
../L1_Project/build# ./traffic_simulation
