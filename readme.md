::: mermaid
flowchart TB
    0>❔ data existed or not] --|✅|--> B[IMPORT in to pandas];
    style 0 fill: #151514, stroke: #0deb57,color: #cee921
    B[IMPORT in to pandas]--|pd.read|-->C[𝄜 ☷ '< / >'];
    C[𝄜 ☷ '< / >']-->a(((<span style="font-size:30px">📅</span>datetime)));;
    style a fill: #e6dadac3, stroke: #0deb80,color: #ee160f
    H[\df tabular data structure/]-->a(((<span style="font-size:30px">📅</span>datetime)));
    style C fill: #7ea77d, stroke: #0deb57,color: #1e1b4b
    B[IMPORT in to pandas]--|connector|-->E[(SQLDB)];
    style E fill: #148612, stroke: #0deb57,color: #1e1b4b
    style B fill: #74f816, stroke: #eb410d,color: #1e1b4b
     0>❔ data existed or not]  --|❌|--> D[create from scratch];
    style D fill: #f53d0b, stroke: #0deb57,color: #1e1b4b
    D[create from scratch]--|Series.to_df|-->F[list tuple dict np.arr];
    style F fill: #d6a597, stroke: #0deb57,color: #1e1b4b
    D[create from scratch]--|DataFrame|-->G[lists np.arrs matrix,dict ];
    style G fill: #d05728, stroke: #0deb57,color: #1e1b4b    
    C[𝄜 ☷ '< / >']-->H[pandas dataframe index columns tabular structure];
    E[(SQLDB)]-->H[\df tabular data structure/];
    F[list tuple dict np.arr]-->H[\df tabular data structure/];
    G[lists np.arrs matrix,dict ]-->H[\df tabular data structure/];
    H[\df tabular data structure/]--<span style="font-size:30px;background-color:SILVER">&nbsp;👀&nbsp;</span><BR>summary-->J[summary or snippet ];
    J[summary or snippet ]--summary-->N[df.inf. df.describe.sum.median.mode.count.value_counts<span style="background-color:cyan;color:magenta">df.transform.agg</span>];
    style H fill: #12ef12, stroke: #0deb57,color: #0a0af8 
    J[summary or snippet ]--snippet-->O[df.head df.tail];    
    H[\df tabular data structure/]--<span style="font-size:30px;background-color:grey">🖉📖</span><br>UPDATE-->K[existing or new];
    K[existing or new]--exist-->S[remove or replace na duplicate replace strip];
    style S fill: #4b504b, stroke: #0deb57,color: #eeeefa 
    style K fill: #9aa99a, stroke: #0deb57,color: #191958  
    style R fill: #9aa99a, stroke: #0deb57,color: #1e1b4b  
    style Q fill: #cad4c9, stroke: #0deb57,color: #efeef3  
    K[existing or new]--new-->T[column locrow ];    
    H[\df tabular data structure/]--<span style="font-size:30px;background-color:cyan">🔢↔🆎</span><br>|reshape|-->L[expand💠 or contract🔹];
    L[expand or contract]--<span style="font-size:30px;background-color:cyan">🔹</span>-->Q[df.groupby stack <br>pivot crosstab];
    L[expand or contract]--<span style="font-size:30px;background-color:red">💠</span>-->R[unstack melt explode <br>join merge concat];    
    style L fill: #33d028, stroke: #0deb57,color: #1e1b4b 
    style R fill: #9aa99a, stroke: #0deb57,color: #1e1b4b  
    style Q fill: #b9e0b6, stroke: #0deb57,color: #1e1b4b   
:::
