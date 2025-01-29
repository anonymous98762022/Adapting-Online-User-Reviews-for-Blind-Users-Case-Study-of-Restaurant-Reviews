
# Prompts for Topic Refinement

## Zero-Shot Prompt

### General Instruction
"Given the input topics, refine them by removing non-dish-related topics and retaining only food-related items. Ensure that the final output strictly contains dish-related topics and excludes irrelevant items."

### Task Input (Zero-Shot)
**Input Topics:**  
Tiramisu, Decorations, Desserts, Tables, Noise, Candles  

**Refined Topics:**  
Tiramisu, Desserts

---

## One-Shot Prompt

### General Instruction
"Here is an example of topic refinement. Use this example to refine the input topics by removing all non-dish-related items."

### Example
**Input Topics:**  
Tiramisu, Decorations, Desserts, Tables, Noise, Candles  

**Refined Topics:**  
Tiramisu, Desserts

### Task Input (One-Shot)
**Input Topics:**  
Fries, Music, Pasta, Chairs, Walls, Promotions  

**Refined Topics:**  
Fries, Pasta

---

## Few-Shot CoT (Chain of Thought) Prompt

### General Instruction
"Here are examples of topic refinement with explanations. Use similar reasoning to refine the input topics by removing irrelevant items and keeping only food-related topics."

### Examples

#### Example 1
**Input Topics:**  
Tiramisu, Decorations, Desserts, Tables, Noise, Candles  

**Refined Topics:**  
Tiramisu, Desserts  

**Reasoning:**  
Tiramisu and Desserts are dish-related, while Decorations, Tables, Noise, and Candles are not and are removed.

#### Example 2
**Input Topics:**  
Fries, Music, Pasta, Chairs, Walls, Promotions  

**Refined Topics:**  
Fries, Pasta  

**Reasoning:**  
Fries and Pasta are food-related, while Music, Chairs, Walls, and Promotions are irrelevant and are removed.

#### Example 3
**Input Topics:**  
Chicken Nuggets, Drinks, Flowers, Service, Paintings, Restroom  

**Refined Topics:**  
Chicken Nuggets, Drinks  

**Reasoning:**  
Chicken Nuggets and Drinks are food items, while Flowers, Service, Paintings, and Restroom are non-dish-related and are excluded.

### Task Input (Few-Shot CoT)
**Input Topics:**  
Salads, Lighting, Burgers, Staff Behavior, Waffle Fries, Cleanliness  

**Refined Topics:**  
Salads, Burgers, Waffle Fries  

**Reasoning:**  
Salads, Burgers, and Waffle Fries are food-related topics, while Lighting, Staff Behavior, and Cleanliness are not and are removed.

---

## Tree of Thought Prompt

### General Instruction
"To refine topics, use a step-by-step tree of thought approach. Identify and retain key food-related items, remove non-dish-related topics, and ensure that the final output strictly contains only dish-related topics."

### Task Input (Tree of Thought)
**Steps:**  
1. Identify and retain key food-related items in the input topics.  
2. Remove all non-dish-related topics, such as Decorations, Tables, Noise, Flowers, and Restroom.  
3. Ensure that the final output contains only dish-related topics.  

**Input Topics:**  
Salads, Lighting, Burgers, Staff Behavior, Waffle Fries, Cleanliness  

**Refined Topics:**  
Salads, Burgers, Waffle Fries
