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

# shorthand

- grid-column
  ```
  grid-column: 1 / -1;
  ```
- grid-row

  ```
  grid-row: row-2-start / span 1
  ```

- grid-area
  ```
  grid-area: row-1-start / column-1-start / row-1-end / column-1-end
  ```
  ```
  grid-area: row-1-start / 2 / row-2-end / span 3;
  ```

# gap

- grid-column-gap
- grid-row-gap
- grid-gap

# area

- define template layout
  ```
  grid-template-columns: repeat(4, 25%);
  grid-template-rows: [row-1-start]1rem [row-1-end row-2-start]1rem [row-2-end]1rem;
  ```
- define area name
  ```
  grid-template-areas: "header header header header"
                       ". . main main"
                       "footer footer footer footer";
  ```

# fit-content

```
grid-template-rows: 3.5rem auto fit-content(8rem);
```

# positioning grid element

## for align elements in grid layout

- justify-items

  - center
  - start
  - end
  - stretch(default)

- align-items
  - center

## for align grid layout itself

- justify-content(x-axis)

  - start
  - end
  - stretch

- align-content(y-axis)

# position single element

- justify-self(x)
  - center
  - start
  - end
- align-self(y)

# responsive grid layout

- use media-query

# applying auto flow

- grid-auto-rows
  - default
  ```
  grid-auto-rows: auto
  ```
