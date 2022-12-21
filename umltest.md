```
                                               
                                               Liquidization Process                                           
                                                                                                               
                  ┌─┐                          ┌─┐                             ┌─┐                    ┌─┐      
                  ║"│                          ║"│                             ║"│                    ║"│      
                  └┬┘                          └┬┘                             └┬┘                    └┬┘      
                  ┌┼┐                          ┌┼┐                             ┌┼┐                    ┌┼┐      
                   │                            │                               │                      │       
                  ┌┴┐                          ┌┴┐                             ┌┴┐                    ┌┴┐      
      MsgServer.go (Liquidate())            Keeper.go                      Borrows.go            Collateral.go 
                  │     keeper.Liquidate()      │                              │                       │       
                  │ ───────────────────────────>│                              │                       │       
                  │                             │                              │                       │       
                  │                             │keeper.repayBorrow(liquidator)│                       │       
                  │                             │──────────────────────────────>                       │       
      MsgServer.go (Liquidate())            Keeper.go                      Borrows.go            Collateral.go 
                  ┌─┐                          ┌─┐                             ┌─┐                    ┌─┐      
                  ║"│                          ║"│                             ║"│                    ║"│      
                  └┬┘                          └┬┘                             └┬┘                    └┬┘      
                  ┌┼┐                          ┌┼┐                             ┌┼┐                    ┌┼┐      
                   │                            │                               │                      │       
                  ┌┴┐                          ┌┴┐                             ┌┴┐                    ┌┴┐      

```

test
