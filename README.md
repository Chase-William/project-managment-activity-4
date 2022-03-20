## PERT Diagram

```mermaid
flowchart TD
  A[A: 3.2] ----> B[B: 3.8];
  A ----> C[C: 2.0];
  B ----> D[D: 4.0];
  C ----> E[E: 3.7];
  C ----> F[F: 4.5];
  E ----> G[G: 3.0];
  D ----> H[H: 1.0];
  G ----> H;
  I[I: 3.7] ----> H;
  F ----> I;
  H ----> J[J: 2.2];
```


1. Critical-Path: `A-C-F-I-H-J`
2. Slack-Path: `A-B-D-H-J`
3. If activity `E` crashes the critical path will not change.
4. If activity `F` crashes the new critical path becomes `A-C-E-G-H-J`.
