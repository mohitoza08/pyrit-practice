# PyRIT Practice — LLM Red Teaming

## What is PyRIT?
**Microsoft's open-source LLM Red Teaming tool** — finds vulnerabilities in LLMs by running adversarial attacks.

## 5 Components
1. **Target** — Which LLM to attack
2. **Orchestrator** — Controls attack flow
3. **Strategy** — Type of attack (injection, jailbreak, etc.)
4. **Memory** — Stores conversation history
5. **Scorer** — Evaluates results

## Install
```bash
pip install pyrit
```

## Experiments

### 1. Prompt Injection (`prompt_injection.py`)
- Tests 5 injection prompts against GPT-4
- Attempts to override model instructions in a single line
- Results: `results/injection_results.txt`

### 2. Jailbreak (`jailbreak.py`)
- Uses multi-turn conversations to bypass model restrictions
- Strategies: DAN, Developer Mode, Evil Twin
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
