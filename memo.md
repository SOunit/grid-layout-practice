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
    - naming row
      ```
      grid-template-rows: [row-1-start]1fr [row-1-end row-2-start]1fr [row-2-end row-3-start]1fr;
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
    - `-1`

      - can always be the last column

      ```
      grid-column-end: -1;
      ```

    - can overlap if explicitly defined the overlapping position

  - `grid-row-start`
  - `grid-row-end`

# naming row

- template / container

  ```
  grid-template-row: [row-1-start]200px [row-1-end row-2-start]200px [row-2-end]200px;
  ```

- child element
