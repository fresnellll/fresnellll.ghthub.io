# C Program Flowchart

```mermaid
flowchart TD
    A[Input integer m] --> B[Initialize character array a[33] to '0']
    B --> C[Define mask = 0x00000001]
    C --> D[Loop i from 31 to 0]
    D --> E[Extract the lowest bit of m and store in a[i], a[i] = (m & mask) + '0']
    E --> F[Right shift m, m >>= 1]
    F --> G[Continue loop until i = 0]
    G --> H[End loop]
    H --> I[Loop j from 0 to 31]
    I --> J[Output a[j]]
    J --> K[End]
