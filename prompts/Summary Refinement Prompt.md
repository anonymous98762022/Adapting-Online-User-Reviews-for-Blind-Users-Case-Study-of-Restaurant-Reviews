\subsection{Prompts for Summary Refinement}
\paragraph{\textbf{One-Shot Prompting Example}}  

\textbf{General Instruction:}  
\textit{"Refine the given summary to include only content that aligns with the specified main topic, subtopics, and desired sentiment. Ensure the refined summary excludes unrelated topics, redundant phrases, and undesired sentiments. Keep the output concise and clear."}

\textbf{Example:}  
\begin{quote}
\textbf{Input Summary:}  
"The burger was juicy and flavorful, but the fries were salty and the milkshake was delicious."

\textbf{Main Topic:} Burger  
\textbf{Subtopics:} Taste  
\textbf{Desired Sentiment:} Positive  

\textbf{Refined Summary:}  
"The burger was juicy and flavorful."
\end{quote}

---

\paragraph{\textbf{Few-Shot CoT (Chain-of-Thought) Prompting Example}}  

\textbf{General Instruction:}  
\textit{"Refine the given summary by reasoning through the alignment of each sentence with the specified main topic, subtopics, and desired sentiment. Identify relevant information step-by-step and remove irrelevant content."}

\textbf{Examples:}  

\textbf{Example 1:}  
\begin{quote}
\textbf{Input Summary:}  
"The pizza had fresh toppings, but the sauce was bland. The ambiance was cozy and the staff was polite."

\textbf{Main Topic:} Pizza  
\textbf{Subtopics:} Toppings  
\textbf{Desired Sentiment:} Positive  

\textbf{Reasoning:}  
1. The statement "The pizza had fresh toppings" is relevant to the main topic (Pizza) and subtopic (Toppings) and aligns with the positive sentiment.  
2. The statement "the sauce was bland" is negative and unrelated to the desired sentiment.  
3. The statement "The ambiance was cozy and the staff was polite" is unrelated to the main topic.  

\textbf{Refined Summary:}  
"The pizza had fresh toppings."
\end{quote}

\textbf{Example 2:}  
\begin{quote}
\textbf{Input Summary:}  
"The pasta was creamy and rich, but the portion size was small, and the service was great."

\textbf{Main Topic:} Pasta  
\textbf{Subtopics:} Taste  
\textbf{Desired Sentiment:} Positive  

\textbf{Reasoning:}  
1. "The pasta was creamy and rich" aligns with the main topic (Pasta), subtopic (Taste), and the positive sentiment.  
2. "The portion size was small" is negative and unrelated to the desired sentiment.  
3. "The service was great" is unrelated to the main topic.  

\textbf{Refined Summary:}  
"The pasta was creamy and rich."
\end{quote}

---

\paragraph{\textbf{DSP + Few-Shot Prompting Example}}  

\textbf{General Instruction:}  
\textit{"Refine the given summary to include only content that aligns with the specified main topic, subtopics, and desired sentiment. Use the directional stimuli (keywords) for guidance. Ensure the refined summary excludes unrelated topics, redundant phrases, and undesired sentiments. Keep the output concise and clear."}

\textbf{Examples:}  

\textbf{Example 1:}  
\begin{quote}
\textbf{Input Summary:}  
"The burger was juicy and flavorful, but the fries were salty and the milkshake was delicious."

\textbf{Directional Stimuli:}  
\begin{itemize}
    \item \textbf{Main Topic:} Burger
    \item \textbf{Subtopics:} Taste
    \item \textbf{Desired Sentiment:} Positive
\end{itemize}

\textbf{Refinement Instruction:}  
"Focus only on the burger and its taste, highlighting the positive sentiment. Remove mentions of fries and milkshake."

\textbf{Refined Summary:}  
"The burger was juicy and flavorful."
\end{quote}

\textbf{Example 2:}  
\begin{quote}
\textbf{Input Summary:}  
"The pizza had fresh toppings, but the sauce was bland. The ambiance was cozy and the staff was polite."

\textbf{Directional Stimuli:}  
\begin{itemize}
    \item \textbf{Main Topic:} Pizza
    \item \textbf{Subtopics:} Toppings
    \item \textbf{Desired Sentiment:} Positive
\end{itemize}

\textbf{Refinement Instruction:}  
"Focus only on the pizza and its toppings with positive sentiment. Remove mentions of sauce, ambiance, and staff."

\textbf{Refined Summary:}  
"The pizza had fresh toppings."
\end{quote}

\textbf{Example 3:}  
\begin{quote}
\textbf{Input Summary:}  
"The pasta was creamy and rich, but the portion size was small, and the service was great."

\textbf{Directional Stimuli:}  
\begin{itemize}
    \item \textbf{Main Topic:} Pasta
    \item \textbf{Subtopics:} Taste
    \item \textbf{Desired Sentiment:} Positive
\end{itemize}

\textbf{Refinement Instruction:}  
"Focus only on the pasta and its taste, highlighting the positive sentiment. Remove mentions of portion size and service."

\textbf{Refined Summary:}  
"The pasta was creamy and rich."
\end{quote}
