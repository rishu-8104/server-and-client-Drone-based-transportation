# System Functionality Description

The system consists of two main components: the **fleet service** and the **drone unit**. The fleet service is responsible for managing and coordinating drone flights, while the drone unit represents an individual drone with its own functionalities.

## Fleet Service

### Functionality:
- The fleet service communicates with individual drone units to manage assignments and flights.

### Endpoints:
- **/fleet/v1/flights** (GET): Tests the communication with the drone unit.

### Example Request and Response:

#### Command Line Request:
```
curl http://localhost:8585/fleet/v1/flights
```

#### Expected Response:
```
"The Drone unit responding"
```

## Drone Unit

### Functionality:
The drone unit handles assignments and provides a test endpoint for communication.

#### Endpoints:
/drone/v1/assignments (GET): Provides a test response indicating the drone unit is responding.

#### Example Request and Response:
Command Line Request:
```
curl http://localhost:8484/drone/v1/assignments
```

#### Expected Response:
```
"The Drone unit responding"
```


