# Fundamental Prompt Patterns

## In-Context Training

- Zero-Shot Prompting - no example
- One-Shot Prompting - 1 example
- Few-Shot Prompting - 2+ examples

### Zero Shot Prompting

- The model can do something without any further training (zero)
- Iow, without in-context training
- Might not always get the best results

### One-Shot Prompting

Zero-Shot Example:

> Multiply 6 by 10 
=> the result of multiplying 6 by 10 is 60

One-Shot Example:

> Multiply 6 by 10 
> use the following format as an example
> Multiply 4 by 10: 40

=> Multiply 6 by 10: 60

### Few-Shot Prompting

- makes the response more accurate and more useful
- increase accuracy and effectiveness
- [Study](https://arxiv.org/pdf/2005.14165)
- we should be using between 4 and 8 examples
- Performance gains plateau after 8

### Chain-of-Thought Prompting

- The shot contains the chain of thought

Ex.:

Q: Roger has 5 tennis balls. He buys 2 more cans of tennis balls. Each can has 3 tennis balls. How many tennis balls does he have now?

A: Roger started with 5 balls. 2 cans of 3 tennis balls each is 6 tennis balls. 5 + 6 = 11. The answer is 11.

Q: The cafeteria had 23 apples. If they used 20 to make lunch and bought 6 more, how many do they have?


- Chain-of-Thought prompting improves accuracy
- it allows the model to break complex, multi-step problems into simpler, intermediate steps.
- Write the reasoning in your shot prompting

#### Zero Shot Chain of Thought

- add "Let's think steps-by-steps" to the prompt

