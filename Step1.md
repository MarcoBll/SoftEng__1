Prova di Scrittura con .md e plantuml per esame

```plantuml
class GasStationService{ 
}

class UserService{ 
}

class GasStationServiceimpl{ 
}

class UserServiceimpl{ 
}

class GasStationRepository{ 
}

class UserRepository{ 
}

class UserConverter{
}

class GasStationConverter{
}

GasStationService --> GasStationServiceimpl : use
GasStationServiceimpl --> GasStationRepository 
GasStationServiceimpl --> UserConverter 
GasStationServiceimpl --> GasStationConverter
UserService <.. GasStationServiceimpl

UserService --> UserServiceimpl : use
UserServiceimpl --> UserRepository
UserServiceimpl --> UserConverter
```
