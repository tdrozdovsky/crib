# CRIB

## Contents
1. [Introduction](#1-introduction)
2. [License](#2-license)
3. [Shell script](#3-shell-script-template)
4. [C template](#4-c-template)
5. [Makefile template](#5-makefile-template)
6. [Doxygen](#6-doxygen)

---
## 1. Introduction
The `crib git` contains simple examples and file templates for quick start of
implementation programs, etc.

---
## 2. License
The software is distributed mostly under the free license.

## 3. Shell script template
This part contains references to the documentation, the shell script template
and shell script code style.

## 4. C template
This part contains the `*.c` and `*.h` template, several examples and etc.

## 5. Makefile template
This part contains references to the documentation, the Makefile template.

## 6. Doxygen
This part contains references to the documentation and example how to use
doxygen tool.

```mermaid
graph TD
    Start --> Stop
```

```mermaid
sequenceDiagram
  Home Edge Node->>+Home Edge Node1: Hello
```

```mermaid
sequenceDiagram
    participant Alice
    participant Bob
    Alice->>John: Hello John, how are you?
    loop Healthcheck
        John->>John: Fight against hypochondria
    end
    Note right of John: Rational thoughts <br/>prevail!
    John-->>Alice: Great!
    John->>Bob: How about you?
    Bob-->>John: Jolly good!
```
# Mermaid Test

```mermaid
graph TD
    id1[A] --> id2[B]
    id2[B] --> id3[C]
    id3[C] --> id4[D]
    id4[D] --> id5[E]
    id5[E] --> id6[F]
    id6[F] --> id7[G]
    id7[G] --> id8[H]
```  
    
```mermaid
graph TD;
A-->B;
A-->C;
B-->D;
C-->D;
```

```mermaid
graph TD
	A[Christmas] -->|Get money| B(Go shopping)
	B --> C{Let me think}
	C -->|One| D[Laptop]
	C -->|Two| E[iPhone]
	C -->|Three| F[fa:fa-car Car]
	C -->|Four| F[fa:fa-user Car]
```					

[Shell]: (shell/README.md)
