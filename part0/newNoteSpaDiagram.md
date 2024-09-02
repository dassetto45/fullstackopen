```mermaid
flowchart TD
    subgraph SERVER
    direction TB
        A[retrieve formData]
        B[redraw notes list]
        C[POST /new_note_spa]
        A-->B
        A-->|XMLHttpRequest|C
    end
    browser-->|form submit|SERVER
```