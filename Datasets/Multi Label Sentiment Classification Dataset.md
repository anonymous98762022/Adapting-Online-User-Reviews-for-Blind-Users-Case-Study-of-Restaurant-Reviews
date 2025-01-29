
### Sentiment Classification Dataset

This dataset includes restaurant reviews, ground truth sentiments, and predicted sentiments using various prompting strategies.

---

#### Input Reviews

| **Index** | **Review** |
|-----------|------------|
| 1 | The food was delicious, but the service was slow. |
| 2 | The dessert was amazing and beautifully presented. |
| 3 | The ambiance was dull and uninviting. |
| 4 | The drinks were refreshing, but the waiting time was long. |
| 5 | The main course was cooked perfectly and tasted great. |
| 6 | The appetizer was fresh and tasty. |
| 7 | The staff was friendly and attentive. |
| 8 | The restaurant was clean and well-organized. |
| 9 | The steak was juicy, but the side dish was undercooked. |
| 10 | The service was quick, and the food was served hot. |
| 11 | The soup was flavorful, but the bread was stale. |
| 12 | The dessert options were plentiful and very tasty. |
| 13 | The staff was rude and inattentive. |
| 14 | The ambiance was cozy and comfortable. |
| 15 | The cocktails were unique and perfectly mixed. |
| 16 | The waitstaff seemed uninterested in helping us. |
| 17 | The pasta was cooked perfectly, but the sauce was bland. |
| 18 | The atmosphere was lively and enjoyable. |
| 19 | The portion sizes were generous and filling. |
| 20 | The service was poor, and the staff was unprofessional. |
| 21 | The sushi was fresh, but the rice was overcooked. |
| 22 | The coffee was aromatic and served at the perfect temperature. |
| 23 | The menu had great variety and included vegan options. |
| 24 | The food was served promptly and tasted excellent. |
| 25 | The servers ignored us, and the food was cold. |
| 26 | The pizza was delicious, but the crust was too thick. |
| 27 | The decor was elegant and added to the dining experience. |
| 28 | The salad was fresh, but the dressing was overpowering. |
| 29 | The restroom was unclean, and the staff didn't seem to care. |
| 30 | The fish was flaky and perfectly seasoned. |
| 31 | The tacos were flavorful, but the salsa was too spicy. |
| 32 | The chairs were uncomfortable, making it hard to enjoy the meal. |
| 33 | The pastries were buttery and melted in the mouth. |
| 34 | The lasagna was cheesy, but it lacked seasoning. |
| 35 | The staff was cheerful and made us feel welcome. |
| 36 | The fries were crispy and golden. |
| 37 | The burger patty was undercooked. |
| 38 | The chef came out to greet us, which was a nice touch. |
| 39 | The desserts were decadent and worth every penny. |
| 40 | The wine selection was limited and overpriced. |
| 41 | The lamb chops were cooked perfectly, but the vegetables were bland. |
| 42 | The waiter provided excellent service and recommendations. |
| 43 | The ambiance was perfect for a romantic evening. |
| 44 | The curry was flavorful, but it was served lukewarm. |
| 45 | The sandwich was stale, and the coffee was burnt. |
| 46 | The ice cream was creamy and came with a variety of toppings. |
| 47 | The breadsticks were warm and freshly baked. |
| 48 | The pancakes were fluffy, but the syrup was too sweet. |
| 49 | The noodles were spicy and cooked to perfection. |

---

#### Sentiment Labels

| **Index** | **Ground Truth Sentiments** | **Zero-Shot Sentiments** | **Few-Shot CoT Sentiments** | **CARP Few-Shot Sentiments** |
|-----------|-----------------------------|---------------------------|-----------------------------|------------------------------|
| 1 | Positive, Negative | Positive | Positive, Negative | Positive, Negative |
| 2 | Positive | Positive | Positive | Positive |
| 3 | Negative | Negative | Negative | Negative |
| 4 | Positive, Negative | Positive | Positive, Negative | Positive, Negative |
| 5 | Positive | Positive | Positive | Positive |
| 6 | Positive | Positive | Negative | Positive |
| 7 | Positive | Positive, Negative | Positive | Positive |
| 8 | Positive | Positive | Positive | Positive |
| 9 | Positive, Negative | Positive | Positive, Negative | Positive, Negative |
| 10 | Positive | Positive | Positive | Positive |
| 11 | Positive, Negative | Positive | Negative | Positive, Negative |
| 12 | Positive | Positive | Positive | Positive |
| 13 | Negative | Negative | Negative | Negative |
| 14 | Positive | Positive | Positive | Positive |
| 15 | Positive | Positive, Negative | Positive | Positive |
| 16 | Negative | Negative | Negative | Negative |
| 17 | Positive, Negative | Positive | Positive, Negative | Positive, Negative |
| 18 | Positive | Positive | Positive | Positive |
| 19 | Positive | Positive | Positive | Positive |
| 20 | Negative | Negative | Negative | Negative |
| 21 | Positive, Negative | Positive, Negative | Positive, Negative | Positive, Negative |
| 22 | Positive | Positive | Positive | Positive |
| 23 | Positive | Positive | Positive | Positive |
| 24 | Positive | Positive | Positive | Positive |
| 25 | Negative | Negative | Negative | Negative |
| 26 | Positive, Negative | Positive | Positive, Negative | Positive, Negative |
| 27 | Positive | Positive | Positive | Positive |
| 28 | Positive | Positive | Positive | Positive |
| 29 | Negative | Negative | Negative | Negative |
| 30 | Positive | Positive, Negative | Positive | Positive |
| 31 | Positive, Negative | Positive | Positive, Negative | Positive, Negative |
| 32 | Negative | Negative | Negative | Negative |
| 33 | Positive | Positive | Positive | Positive |
| 34 | Positive | Positive | Positive | Positive |
| 35 | Positive, Negative | Positive | Positive, Negative | Positive, Negative |
| 36 | Positive | Positive | Positive | Positive |
| 37 | Positive | Positive | Positive | Positive |
| 38 | Negative | Negative | Negative | Negative |
| 39 | Positive | Positive | Positive | Positive |
| 40 | Positive | Positive | Negative | Negative |
| 41 | Positive | Positive | Positive | Positive |
| 42 | Negative | Negative | Negative | Negative |
| 43 | Positive, Negative | Positive, Negative | Positive, Negative | Positive, Negative |
| 44 | Positive | Positive | Positive | Positive |
| 45 | Positive | Positive | Positive | Positive |
| 46 | Negative | Negative | Positive | Positive |
| 47 | Positive, Negative | Positive | Negative | Negative |
| 48 | Positive | Positive | Positive, Negative | Positive, Negative |
| 49 | Positive | Positive | Positive | Positive |
| 50 | Positive | Positive | Positive | Positive |

---

### Caption

**Table: Sentiment Classification Dataset**

This table includes input reviews, their ground truth sentiment labels, and the predictions from various sentiment classification prompting strategies.
