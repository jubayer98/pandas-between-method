# Pandas Between Method

This repository demonstrates how to use the `between` method in pandas to match mutations with regions from two CSV files.

## Files

**annotated.csv**: Contains columns `chr`, `start`, and `alt`.

<img width="197" alt="Screenshot 2023-05-05 at 15 21 11" src="https://user-images.githubusercontent.com/13205577/236469906-12ae49ec-fa4b-4ba5-86d8-befd419b9178.png">

**haplo.csv**: Contains columns `chr`, `start`, `end`, and `score`.

<img width="264" alt="Screenshot 2023-05-05 at 15 27 16" src="https://user-images.githubusercontent.com/13205577/236470350-292fd15f-4861-4aca-8ed4-0ed2be821ddb.png">

## Objective

For each mutation in `annotated.csv`, find if it falls within any region in `haplo.csv` and append the corresponding `score` to `annotated.csv`.

## Example

- **annotated.csv**:
  ```
  chr    start    alt
  chr1   234      G
  ```

- **haplo.csv**:
  ```
  chr    start    end    score
  chr1   200      210    3
  chr1   230      240    10
  ```

- **Result**:
  ```
  chr    start    alt    score
  chr1   234      G      10
  ```
