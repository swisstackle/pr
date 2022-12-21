```
@startuml
title "Liquidization Process"

actor "MsgServer.go (Liquidate())" as MsgServer
actor "Keeper.go" as Keeper
actor "Borrows.go" as borrows
actor "Collateral.go" as collateral
actor Bankkeeper
actor "Store.go" as store


MsgServer -> Keeper : keeper.Liquidate()
Keeper ->  borrows: keeper.repayBorrow(liquidator)
alt directLiquidation
    Keeper -> collateral: keeper.liquidateCollateral()
else inDirectLiquidation
    Keeper -> collateral: keeper.decollaterlize()
end

alt directLiquidation
    collateral -> collateral: keeper.burnCollateral()
    collateral -> Bankkeeper: keeper.bankKeeper.SendCoinsFromModuleToAccount()
else inDirectLiquidation
    collateral -> store: keeper.setCollateral()
    collateral -> Bankkeeper: keeper.bankKeeper.SendCoinsFromModuleToAaccount()
end
@enduml
```
