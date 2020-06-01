# CRIB

```mermaid
graph TD
	A[fa:fa-user User] -->|Generate & store passphrase: ''secret''| Storage1(Home Edge Orchestrator #1)
    
subgraph Home Edge Node #1
    HEO1[Home Edge Orchestrator #1]-->CAPP1(Client app)
    HEO1[Home Edge Orchestrator #1]-->Storage1[...passprase.txt]
end	

```plantuml
@startuml

top to bottom direction

actor User

node "Home Edge Node #1" {
  User --> [f1] : Generate & store ''secret''
  [HOM1] --> [f1] 
  [CA1] --> [f1] 
  [HOM1] <--> [HOM2]
  rectangle "/var/edge-orchestration/data/jwt/passprasejwt.txt" as f1 {
  }
  rectangle "App" as CA1 {
  }
  rectangle "Home Edge Orchestrator" as HOM1 {
  }
}
node "Home Edge Node #2" {
  User --> [f2] : Generate & store ''secret''
  [HOM2] --> [f2] 
  [CA2] --> [f2] 
  folder "/var/edge-orchestration/data/jwt/passprasejwt.txt" as f2 {
  }
  rectangle "App" as CA2{
  }
  rectangle "Home Edge Orchestrator" as HOM2 {
  }
}

@enduml
```
[Shell]: (shell/README.md)
