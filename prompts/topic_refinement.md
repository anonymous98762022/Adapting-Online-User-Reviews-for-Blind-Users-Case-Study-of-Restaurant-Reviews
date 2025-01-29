
# Sequential Topic Modeling Prompts

## Prompt for Parallel Topic Modeling (ParTM)

### General Instruction
Write the results of simulating topic modeling for the following reviews, each starting with `#`. Assume you will identify 5 topics and use 5 top words for each topic. Outputs must always be in the format `Topic k: word word word word word` and nothing else.

### Input
```
# pasta perfectly cooked flavorful sauce portion
# desserts tiramisu waffles creamy rich presentation
# chicken sandwiches crispy juicy sauce filling
# fries portion size crispy hot seasoning
# service friendly staff quick hygiene ambiance
# lemonade tangy refreshing glass sweet sour
# mac cheese creamy cheesy rich comfort
# ambiance clean welcoming noisy lighting
```

### Output Format
```
Topic k: word word word word word
```

---

## Prompt for Sequential Topic Modeling (SeqTM)

### General Instruction
We aim to identify topics for the entire set of restaurant reviews by sequentially updating tentative topics identified from each subset, considering topics identified just before from another subset. Write the results of simulating topic modeling for the following reviews, each starting with `#`. Make the most use of the following topics previously identified from another set of reviews, each starting with `Topic k:`. Assume you will finally identify 5 topics and use 5 top words for each topic. Outputs must always be in the format `Topic k: word word word word word` and nothing else. Outputs should be the same as the previous topics as much as possible. You can change them minimally only when the given reviews don’t include them much, and a new topic needs to be added to describe the reviews.

### Previously Identified Topics
```
Topic 1: pasta ambiance cleanliness service
Topic 2: dessert tiramisu waffles portion
Topic 3: chicken nuggets crispy flavor sauce
Topic 4: drinks lemonade tangy refreshing glass
Topic 5: mac cheese creamy rich comfort
```

### Input
```
# pasta perfectly cooked flavorful
# desserts tiramisu rich presentation
# fries crispy portion hot hygiene
# chicken sandwiches fresh slow service
# mac and cheese rich creamy delicious
```

### Output Format
```
Topic k: word word word word word
```

---

## Usage

1. Use **Parallel Topic Modeling (ParTM)** for the first subset of reviews to generate initial topics.
2. Use **Sequential Topic Modeling (SeqTM)** for subsequent subsets, refining topics based on the previously identified topics.
3. Ensure minimal changes to topics unless required by the new review content.

---

This `.md` file is ready to be added to your GitHub repository. Copy and paste this into a file named `sequential_topic_modeling.md`. Let me know if you need further adjustments!
