
### Dataset for Summary Refinement

This dataset provides examples of how different refinement strategies process input summaries into more concise and targeted outputs.

#### Input Summaries with Refining Information and Ground Truth

| **Input Summary** | **Refining Information** | **Refined Summary Ground Truth** |
|--------------------|--------------------------|-----------------------------------|
| Customers praised the crispy fries and large portions. Staff were friendly but slow to respond. | Topic: Fries, Subtopic: Taste, Portions, Sentiment: Positive | Customers praised the crispy fries and large portions. |
| Tiramisu was described as rich and flavorful. Tables were unclean according to some customers. | Topic: Tiramisu, Subtopic: Taste, Sentiment: Positive | Tiramisu was described as rich and flavorful. |
| Drinks were refreshing, though some found them too sweet. Service was inconsistent. | Topic: Drinks, Subtopic: Flavor, Sentiment: Negative | Drinks were refreshing, though some found them too sweet. |
| The pasta dishes were well-received for their taste and portion size. Ambiance was cozy and warm. | Topic: Pasta, Subtopic: Taste, Portions, Sentiment: Positive | The pasta dishes were well-received for their taste and portion size. |
| Nuggets were praised for their crispy exterior and juicy chicken, but the tables were not clean. | Topic: Chicken Nuggets, Subtopic: Texture, Taste, Sentiment: Positive | Nuggets were praised for their crispy exterior and juicy chicken. |
| Lemonade was described as tangy and refreshing. Some found the service too slow. | Topic: Lemonade, Subtopic: Flavor, Sentiment: Positive | Lemonade was described as tangy and refreshing. |
| Burgers were praised for their flavor, but the wait times were long. | Topic: Burgers, Subtopic: Taste, Sentiment: Positive | Burgers were praised for their flavor. |
| Pizza received positive feedback for the crust and toppings, but some found it too oily. | Topic: Pizza, Subtopic: Crust, Toppings, Sentiment: Positive | Pizza received positive feedback for the crust and toppings. |
| Waffle fries were described as crispy and generously portioned. Cleanliness was a concern. | Topic: Waffle Fries, Subtopic: Texture, Portions, Sentiment: Positive | Waffle fries were described as crispy and generously portioned. |
| Ice cream was loved for its creamy texture, but portions were small. | Topic: Ice Cream, Subtopic: Texture, Sentiment: Positive | Ice cream was loved for its creamy texture. |
| Cocktails were enjoyed for their unique flavors, though some found them overpriced. | Topic: Cocktails, Subtopic: Flavor, Sentiment: Positive | Cocktails were enjoyed for their unique flavors. |
| Grilled chicken was juicy and flavorful, but some portions were unevenly cooked. | Topic: Grilled Chicken, Subtopic: Texture, Taste, Sentiment: Positive | Grilled chicken was juicy and flavorful. |
| Bread rolls were fresh and soft, but the butter was served cold. | Topic: Bread Rolls, Subtopic: Texture, Sentiment: Positive | Bread rolls were fresh and soft. |
| Soups were described as hearty and well-seasoned, but service was slow. | Topic: Soups, Subtopic: Flavor, Sentiment: Negative | Soups were described as hearty and well-seasoned. |
| Dim sum was praised for its authenticity, but the wait was long. | Topic: Dim Sum, Subtopic: Authenticity, Sentiment: Positive | Dim sum was praised for its authenticity. |
| Shrimp tempura was crispy and perfectly cooked, but the dipping sauce lacked flavor. | Topic: Shrimp Tempura, Subtopic: Texture, Sentiment: Positive | Shrimp tempura was crispy and perfectly cooked. |
| Paneer butter masala was rich and creamy, but naan was undercooked. | Topic: Paneer Butter Masala, Subtopic: Flavor, Sentiment: Positive | Paneer butter masala was rich and creamy. |
| Salads were fresh and vibrant, but the dressings were overpowering. | Topic: Salads, Subtopic: Freshness, Sentiment: Positive | Salads were fresh and vibrant. |
| Nachos were loved for their generous toppings, but the chips were slightly stale. | Topic: Nachos, Subtopic: Toppings, Sentiment: Negative | Nachos were loved for their generous toppings. |
| Cheesecake was smooth and rich, but some found it too sweet. | Topic: Cheesecake, Subtopic: Texture, Flavor, Sentiment: Positive | Cheesecake was smooth and rich. |
| Spring rolls were crispy and packed with vegetables, but the sauce was too spicy. | Topic: Spring Rolls, Subtopic: Texture, Filling, Sentiment: Positive | Spring rolls were crispy and packed with vegetables. |
| Mojitos were refreshing and perfectly balanced, but the ice melted quickly. | Topic: Mojitos, Subtopic: Flavor, Sentiment: Positive | Mojitos were refreshing and perfectly balanced. |
| Mac and cheese was creamy and flavorful, but the portion size was small. | Topic: Mac and Cheese, Subtopic: Texture, Flavor, Sentiment: Positive | Mac and cheese was creamy and flavorful. |
| Chicken wings were crispy and juicy, but the spice level was inconsistent. | Topic: Chicken Wings, Subtopic: Texture, Taste, Sentiment: Positive | Chicken wings were crispy and juicy. |

---

#### Refined Summaries from Different Prompting Strategies

| **Input Summary** | **Zero-Shot Output** | **Few-Shot CoT Output** | **DSP + Few-Shot Output** |
|--------------------|----------------------|--------------------------|---------------------------|
| Customers praised the crispy fries and large portions. Staff were friendly but slow to respond. | Crispy fries and large portions praised. | Customers praised the crispy fries and large portions. | Customers praised the crispy fries and their generous portions. |
| Tiramisu was described as rich and flavorful. Tables were unclean according to some customers. | Rich tiramisu with flavorful taste. | Tiramisu was described as rich and flavorful. | Tiramisu was described as rich and flavorful, a favorite among desserts. |
| Drinks were refreshing, though some found them too sweet. Service was inconsistent. | Refreshing drinks, a bit too sweet. | Drinks were refreshing though a bit sweet. | Drinks were refreshing, though a few found them slightly sweet. |
| The pasta dishes were well-received for their taste and portion size. Ambiance was cozy and warm. | Pasta dishes were well-received for taste. | The pasta dishes were well-received for taste and portions. | The pasta dishes were praised for their excellent taste and portion size. |
| Nuggets were praised for their crispy exterior and juicy chicken, but the tables were not clean. | Nuggets were crispy and juicy. | Nuggets were crispy and juicy. | Nuggets were crispy and juicy, highly appreciated by diners. |
| Lemonade was described as tangy and refreshing. Some found the service too slow. | Tangy and refreshing lemonade. | Lemonade was tangy and refreshing. | Lemonade was tangy and refreshing, perfectly balanced. |
| Burgers were praised for their flavor, but the wait times were long. | Flavorful burgers praised by customers. | Burgers were flavorful and satisfying. | Burgers were loved for their flavor and fresh toppings. |
| Pizza received positive feedback for the crust and toppings, but some found it too oily. | Pizza crust and toppings were good. | Pizza was praised for its crust and fresh toppings. | Pizza received positive feedback for its crust and toppings. |
| Waffle fries were described as crispy and generously portioned. Cleanliness was a concern. | Crispy and generously portioned waffle fries. | Waffle fries were crispy and generously portioned. | Waffle fries were described as crispy and generously portioned. |
| Ice cream was loved for its creamy texture, but portions were small. | Ice cream had a creamy texture. | Ice cream was creamy and well-loved. | Ice cream was creamy and smooth, enjoyed for its rich texture. |
| Cocktails were enjoyed for their unique flavors, though some found them overpriced. | Unique cocktails with balanced flavors. | Cocktails had unique and balanced flavors. | Cocktails were unique and enjoyed for their vibrant flavors. |
| Grilled chicken was juicy and flavorful, but some portions were unevenly cooked. | Juicy and perfectly grilled chicken. | Grilled chicken was juicy and flavorful. | Grilled chicken was juicy and flavorful, cooked to perfection. |
| Bread rolls were fresh and soft, but the butter was served cold. | Soft and fresh bread rolls. | Bread rolls were fresh and served warm. | Bread rolls were soft and fresh, served warm. |
| Soups were described as hearty and well-seasoned, but service was slow. | Hearty soups with good seasoning. | Soups were hearty and well-seasoned. | Soups were hearty and well-seasoned, a comforting choice. |
| Dim sum was praised for its authenticity, but the wait was long. | Authentic dim sum praised for taste. | Dim sum was praised for its authentic flavors. | Dim sum was praised for its authentic flavors. |
| Shrimp tempura was crispy and perfectly cooked, but the dipping sauce lacked flavor. | Shrimp tempura crispy and well-made. | Shrimp tempura was crispy and perfectly cooked. | Shrimp tempura was crispy and perfectly cooked. |
| Paneer butter masala was rich and creamy, but naan was undercooked. | Rich paneer butter masala enjoyed. | Paneer butter masala was creamy and rich. | Paneer butter masala was rich and creamy. |
| Salads were fresh and vibrant, but the dressings were overpowering. | Vibrant and fresh salads. | Salads were fresh and vibrant. | Salads were fresh and vibrant. |
| Nachos were loved for their generous toppings, but the chips were slightly stale. | Nachos with generous toppings were liked. | Nachos had generous toppings and good flavor. | Nachos were loved for their generous toppings. |
| Cheesecake was smooth and rich, but some found it too sweet. | Smooth and rich cheesecake. | Cheesecake was smooth, rich, and delicious. | Cheesecake was smooth and rich, a popular dessert. |

---

#### Caption

**Table: Refined Summaries from Different Prompting Strategies**

This table provides examples of how input summaries are refined through Zero-Shot, Few-Shot CoT (Chain of Thought), and DSP (Directional Stimuli with Few-Shot) prompting strategies.
