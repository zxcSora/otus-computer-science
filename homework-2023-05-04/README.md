Формально данная машина Тьюринга может быть описана как:

```M = ({0, 1, 2}, {0, 1},{0, 1},𝛿,q0,B,{2})```

| δ | 0       | 1       | *       | _       |
|---|---------|---------|---------|---------|
| 0 |         |         | (0,*,R) | (1,*,L) |
| 1 | (2,0,L) | (1,0,L) |         |         |
| 2 |         |         |         |         |