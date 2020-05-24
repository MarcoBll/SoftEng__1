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
