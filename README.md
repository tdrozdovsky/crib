# CRIB

```plantuml

@startuml

top to bottom direction

actor User

node "Home Edge Node #1" {
  User --> [f1] : 1. Generate & store ''secret''
  [HOM1] --> [f1] : 4. Get ''secret''
  [HOM1] --> [HOM1] : 5. Check JWT, if success handle request
  [CA1] --> [f1] : 2. Get ''secret'' & generate JWT 
  [CA1] -->[HOM1] : 3. Send Request & JWT
  rectangle "/var/edge-orchestration/data/jwt/passprasejwt.txt" as f1 {
  }
  rectangle "App" as CA1 {
  }
  rectangle "Home Edge Orchestrator" as HOM1 {
  }
}

@enduml
```
[Shell]: (shell/README.md)
