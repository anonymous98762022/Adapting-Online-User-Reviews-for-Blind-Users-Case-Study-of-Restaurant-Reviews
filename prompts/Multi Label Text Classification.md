
# Prompts for Theme Classification

## Zero-Shot Prompt Example

### General Instruction
"Classify the given restaurant review into one or more relevant themes from the following list: [Food Quality, Ambiance, Hygiene, Service, Portion Size, Price, Presentation, Drink Quality]. Identify the most significant themes, and do not include slightly relevant topics. Provide a list of themes only."

### Example
**Input:**  
"The pasta was perfectly cooked, but the ambiance was too noisy."  

**Output:**  
Food Quality, Ambiance

### Task Input (Zero-Shot)
**Input:**  
"The chicken nuggets were crispy and flavorful, but the tables were dirty and poorly maintained."  

**Output:**  
Food Quality, Hygiene

---

## Few-Shot CoT (Chain of Thought) Prompt Example

### General Instruction
"Classify the given restaurant review into one or more relevant themes from the following list: [Food Quality, Ambiance, Hygiene, Service, Portion Size, Price, Presentation, Drink Quality]. Justify each theme selection with reasoning based on specific phrases or details in the input."

### Examples

#### Example 1
**Input:**  
"The pasta was perfectly cooked, but the ambiance was too noisy."  

**Reasoning:**  
1. The phrase "pasta" and "perfectly cooked" relate to Food Quality.  
2. The phrase "ambiance" and "too noisy" relate to Ambiance.  

**Output:**  
Food Quality, Ambiance

#### Example 2
**Input:**  
"The lemonade was tangy and refreshing, but the portion size was too small."  

**Reasoning:**  
1. "Lemonade," "tangy," and "refreshing" relate to Drink Quality.  
2. "Portion size" and "too small" relate to Portion Size.  

**Output:**  
Drink Quality, Portion Size

#### Task Input (Few-Shot CoT)
**Input:**  
"The chicken nuggets were crispy and flavorful, but the tables were dirty and poorly maintained."  

**Reasoning:**  
1. "Chicken nuggets," "crispy," and "flavorful" relate to Food Quality.  
2. "Tables," "dirty," and "poorly maintained" relate to Hygiene.  

**Output:**  
Food Quality, Hygiene

---

## CARP + Few-Shot Prompts

This is a theme classification task for restaurant reviews.  

1. Present **CLUES** (i.e., keywords, phrases, contextual information, semantic relations, semantic meaning, tones, or references) that indicate the themes relevant to the input.  
2. Deduce the **REASONING** process based on the clues and input to support the thematic classification (Limit the number of words to 130).  
3. Select as many significantly relevant themes as applicable but do not include slightly relevant topics.

### Predefined Themes:  
[Food Quality, Ambiance, Hygiene, Service, Portion Size, Price, Presentation, Drink Quality]

### Examples

#### Example 1
**INPUT:**  
"The pasta was perfectly cooked, but the ambiance was too noisy."  

**CLUES:**  
- "pasta," "cooked" (indicates quality of food).  
- "noisy," "ambiance" (indicates atmosphere).  

**REASONING:**  
The presence of "pasta" and "cooked" relates to the theme of Food Quality, while "noisy" and "ambiance" relate to the theme of Ambiance.  

**THEMES:**  
Food Quality, Ambiance  

#### Example 2
**INPUT:**  
"The lemonade was tangy and refreshing, but the portion size was too small."  

**CLUES:**  
- "lemonade," "tangy," "refreshing" (indicates drink quality).  
- "portion size," "too small" (indicates portion-related complaint).  

**REASONING:**  
The input highlights the drink quality with "lemonade," "tangy," and "refreshing," associating it with Drink Quality. The complaint about "portion size" being "too small" links it to Portion Size.  

**THEMES:**  
Drink Quality, Portion Size  

---

### Task Input (CARP + Few-Shot)
**INPUT:**  
"The chicken nuggets were crispy and flavorful, but the tables were dirty and poorly maintained."  

Find **CLUES**, **REASONING**, and **THEMES** for this input.
