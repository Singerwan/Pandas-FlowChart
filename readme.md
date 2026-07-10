```mermaid
    0> data existed or not] --|yes|--> B[IMPORT in to pandas];
    style 0 fill: #151514, stroke: #0deb57,color: #cee921
    B[IMPORT in to pandas]--|pd.read|-->C[];
    C[]-->a(((datetime)));;
    H[\df tabular data structure/]-->a(((datetime)));
    style C fill: #7ea77d, stroke: #0deb57,color: #1e1b4b
    B[IMPORT in to pandas]--|connector|-->E[(SQLDB)];
    style E fill: #148612, stroke: #0deb57,color: #1e1b4b
    style B fill: #74f816, stroke: #eb410d,color: #1e1b4b
     0> data existed or not]  --no|--> D[create from scratch];
    style D fill: #f53d0b, stroke: #0deb57,color: #1e1b4b
    D[create from scratch]--|Series.to_df|-->F[list tuple dict np.arr];
    style F fill: #d6a597, stroke: #0deb57,color: #1e1b4b
    D[create from scratch]--|DataFrame|-->G[lists np.arrs matrix,dict ];
    style G fill: #d05728, stroke: #0deb57,color: #1e1b4b    
    C[𝄜 ☷ '< / >']-->H[pandas dataframe index columns tabular structure];
    E[(SQLDB)]-->H[\df tabular data structure/];
    F[list tuple dict np.arr]-->H[\df tabular data structure/];
    G[lists np.arrs matrix,dict ]-->H[\df tabular data structure/];
    H[\df tabular data structure/]---->J[summary or snippet ];
    J[summary or snippet ]--summary-->N[df.inf. df.describe.sum.median.mode.count.value_counts;
    style H fill: #12ef12, stroke: #0deb57,color: #0a0af8 
    J[summary or snippet ]--snippet-->O[df.head df.tail];    
    H[\df tabular data structure/]---->K[existing or new];
    K[existing or new]--exist-->S[remove or replace na duplicate replace strip];
    K[existing or new]--new-->T[column locrow ];    
    H[\df tabular data structure/]---->L[expand or contract];
    L[expand or contract]---->Q[df.groupby stack <br>pivot crosstab];
    L[expand or contract]---->R[unstack melt explode <br>join merge concat];    
    style L fill: #33d028, stroke: #0deb57,color: #1e1b4b 
    style R fill: #9aa99a, stroke: #0deb57,color: #1e1b4b  
    style Q fill: #b9e0b6, stroke: #0deb57,color: #1e1b4b   
```
