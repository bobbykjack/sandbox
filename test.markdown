# testing

hello *world*

```mermaid
  graph TD;
      A-->B;
      A-->C;
      B-->D;
      C-->D;
```

```mermaid
  sequenceDiagram
    participant Alice
    participant Bob
    Alice->>Bob: Hi Bob
    Bob->>Alice: Hi Alice
```

```mermaid
sequenceDiagram
    Bart->>Homer: Don't have a cow, man.
```

```mermaid
stateDiagram-v2
    [*] --> New
    New --> Ready: admitted
    Ready --> Running: scheduler dispatch
    Running --> Ready: interrupt
    Running --> Waiting: I/O or event wait
    Waiting --> Ready: I/O or event completion
    Running --> Terminated: exit
    Terminated --> [*]
```
