```
@startuml

title "Liquidization Process"

actor "MsgServer.go (Liquidate())" as MsgServer
actor "Keeper.go" as Keeper
actor "Borrows.go" as borrows
actor "Collateral.go" as collateral


MsgServer -> Keeper : keeper.Liquidate()
Keeper ->  borrows: keeper.repayBorrow(liquidator)

@enduml
```
