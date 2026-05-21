# LangChain Chains

Learning and implementing the **Chains** concept in LangChain using LCEL.

## Files

| File | What it does |
|---|---|
| `simple_chain.py` | Basic `prompt | model | parser` pipeline |
| `sequential_chain.py` | Output of one chain fed into the next |
| `parallel_chain.py` | Two chains run in parallel, outputs merged |
| `conditional_chain.py` | Routes to different chains based on sentiment |

## Setup

```bash
pip install langchain langchain-openai langchain-anthropic python-dotenv pydantic
```

Create a `.env` file:
```
OPENAI_API_KEY=your_key
ANTHROPIC_API_KEY=your_key
```

## Concepts Used

- LCEL (`|` operator) for chaining components
- `RunnableParallel` — run chains concurrently
- `RunnableBranch` — conditional routing
- `PydanticOutputParser` — structured outputs

## Author
[Prabhav54](https://github.com/Prabhav54) — NIT Rourkela
