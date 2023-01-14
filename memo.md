- use firefox
- display grid

# column

- grid-template-columns

```
grid-template-columns: 200px 150px 20%
```

# important topics

- container layout

  - `grid-template-columns`
  - `grid-template-rows`
    - `auto`
      - takes space of content
    - `minmax`
      ```
      grid-template-rows: 300px minmax(10px, 50px);
      ```
      ```
      minmax(10px, auto)
      ```
    - `repeat`
      ```
      grid-template-rows: repeat(4, 25%);
      ```

- child element layout
  - `grid-column-start`
  - `grid-column-end`
    ```
    grid-column-end: 5;
    ```
    - `span`
      - takes a number of columns
      ```
      grid-column-end: span 2;
      ```
  - `grid-row-start`
  - `grid-row-end`
