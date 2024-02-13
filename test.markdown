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

```mermaid
flowchart LR
    subgraph one[" "]
    data1[&lt;li&gt;42&lt;/li&gt;]
    next1(nextElementSibling)
    end

    subgraph two[" "]
    direction LR
    data2[&lt;li id=&quot;current&quot;&gt;7&lt;/li&gt;]
    next2(nextElementSibling)
    end

    subgraph three[" "]
    direction LR
    data3[&lt;li&gt;120&lt;/li&gt;]
    next3(nextElementSibling)
    end

    next1-->two
    next2-->three
    next3-->null
```
