# PyRIT Practice — LLM Red Teaming

## Kya Hai PyRIT?
**Microsoft ka open-source LLM Red Teaming tool** — LLM ko adversarial attacks karke vulnerabilities dhundhta hai.

## 5 Components
1. **Target** — Kaunsa LLM attack hoga
2. **Orchestrator** — Attack flow control
3. **Strategy** — Kis type ka attack
4. **Memory** — Conversation history
5. **Scorer** — Result evaluate

## Install
```bash
pip install pyrit
```

## Experiments

### 1. Prompt Injection (`prompt_injection.py`)
- 5 injection prompts GPT-4 pe try kiye
- Ek line mein instructions override karne ki koshish
- Results: `results/injection_results.txt`

### 2. Jailbreak (`jailbreak.py`)
- Multi-turn conversation se model ko bypass karne ki koshish
- DAN, Developer Mode, Evil Twin strategies
- Results: `results/jailbreak_results.txt`

## Garak vs PyRIT
| Garak | PyRIT |
|-------|-------|
| Quick scan | Deep testing |
| Single-turn | Multi-turn |
| Report-focused | Attack-focused |

## References
- [PyRIT GitHub](https://github.com/Azure/PyRIT)
- [Garak GitHub](https://github.com/leondz/garak)
