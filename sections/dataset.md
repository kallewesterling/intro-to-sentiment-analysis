## Set Up a Dataset

### Option 1: 

Next, we'll make sure that we have a dataset. In this case, we have a text file that will provide us with a number of reviews from RateMyProfessor about Judith Butler.

```python
with open("./butler_ratings.txt", "r") as file:
    dataset = file.read().split("\n")
print(f"Dataset is imported and contains {len(dataset)} reviews.")
```

You should end up with a result that reads `Dataset is imported and contains 15 reviews.`


### Option 2:

You can use any file with one caption per row. Just replace the `./butler_ratings.txt` path above with the path to any text file correctly formatted.
