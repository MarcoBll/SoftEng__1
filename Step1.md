# Dependency graph 

@staruml

interface GasStationService{ 
}

class GasStationServiceimpl{ 
}

interface GasStationRepository{ 
}

class GasStationConverter{
}

class GasStationDto{
}

class GasStation{
}

class GasStationRepositoryimpl{
}

interface UserService{ 
}

class UserServiceimpl{ 
}

interface UserRepository{ 
}

class UserRepositoryimpl{
}

class UserConverter{
}

class User{
}

class UserDto{
}


GasStationService <|.. GasStationServiceimpl 
GasStationServiceimpl --> GasStationRepository 
GasStationServiceimpl --> UserConverter 
GasStationServiceimpl --> GasStationConverter
UserService <.. GasStationServiceimpl
GasStationConverter --> GasStationDto
GasStationConverter --> GasStation
GasStationRepository <|.. GasStationRepositoryimpl


UserService <|.. UserServiceimpl 
UserServiceimpl --> UserRepository
UserServiceimpl --> UserConverter
UserConverter --> User
UserConverter --> UserDto
UserRepository <|.. UserRepositoryimpl

@enduml


#  Tests

   <define below a table for each integration step. For each integration step report the group of classes under test, and the names of
     JUnit test cases applied to them>

## Step 1
| Classes  | JUnit test cases |
|--|--|
|||


## Step 2
| Classes  | JUnit test cases |
|--|--|
|||


## Step n API Tests

   <The last integration step  should correspond to API testing, or tests applied to all classes implementing the APIs defined in the Service package>

| Classes  | JUnit test cases |
|--|--|
|||

