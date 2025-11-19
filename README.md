# IA AstroView**

<div align="center">

![Collaboration Banner](https://img.shields.io/badge/Collaboration-Teamwork-orange?style=for-the-badge&logo=github)

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square&logo=git)](http://makeapullrequest.com)
[![Open Source](https://img.shields.io/badge/Open%20Source-%E2%9D%A4%EF%B8%8F-red?style=flat-square&logo=opensource)](https://opensource.org/)
[![Code of Conduct](https://img.shields.io/badge/Code%20of%20Conduct-Contributor%20Covenant-blueviolet?style=flat-square&logo=handshake)](https://www.contributor-covenant.org/)

**Bem-vindo ao time!**
*Este guia define os padrões para contribuir com o motor de Data Science e a plataforma AstroView.*

</div>

---

## 🚀 **Como Começar**

Estamos felizes em ter você contribuindo para o **NASA Space Apps Challenge 2025**! Antes de começar a codificar, por favor, leia as diretrizes abaixo para garantir que nosso fluxo de trabalho permaneça ágil e organizado.

### 📋 **Workflow de Desenvolvimento (Git Flow)**

Utilizamos um fluxo simplificado para garantir a integridade do código principal.

1.  **🍴 Fork & Clone**: Faça um fork do projeto e clone localmente.
2.  **🌿 Branching**: Crie uma branch descritiva para sua feature ou correção.
    * `feature/nova-analise-impacto`
    * `fix/correcao-calculo-energia`
    * `docs/atualizacao-readme`
3.  **💾 Commits**: Faça commits pequenos e com mensagens claras (Conventional Commits).
    * ✅ `feat: adiciona cálculo de densidade atmosférica`
    * ❌ `update code`
4.  **🚀 Push & PR**: Envie para seu fork e abra um Pull Request para a branch `main`.

---

## 🧠 **Diretrizes para Data Science (.ipynb)**

Trabalhar com Jupyter Notebooks no Git pode gerar conflitos complexos. Siga estas regras estritas para o arquivo `Desafio_Nasa.ipynb`:

### **1. Limpeza de Saídas (Outputs)**
Antes de commitar qualquer alteração no notebook, **limpe todas as saídas das células**. Isso mantém o diff do Git limpo e legível.
* *No Jupyter:* `Kernel` > `Restart & Clear Output`

### **2. Estrutura de Células**
* Mantenha imports no topo.
* Use células de Markdown para explicar a lógica física/matemática antes do código.
* Não use caminhos absolutos (ex: `C:/Users/Juliana/...`), use caminhos relativos ou variáveis de ambiente.

### **3. Instalação de Dependências**
Se você adicionar uma nova biblioteca (ex: `scikit-learn`), adicione-a à célula de instalação no topo do notebook E atualize o arquivo `requirements.txt` se ele existir.

---

## 💻 **Padrões de Código (Python/Engine)**

Para garantir que o motor de simulação seja integrável com o Frontend (Next.js):

* **Tipagem**: Use Type Hints sempre que possível.
    ```python
    def calcular_energia(massa: float, velocidade: float) -> float:
        return 0.5 * massa * (velocidade ** 2)
    ```
* **Docstrings**: Documente todas as funções de física.
    ```python
    """
    Calcula a energia cinética do asteroide em Joules.
    Args:
        massa (float): Massa em kg
        velocidade (float): Velocidade em m/s
    """
    ```
* **JSON Output**: Garanta que a célula final do notebook sempre gere o JSON no formato esperado pelo Frontend (ver README).

---

## 🐛 **Reportando Bugs**

Encontrou um erro na simulação ou na interface?

1. Vá para a aba [Issues](https://github.com/julianaivo/2025-NASA-Space-Apps-Challenge_trifidia-squad/issues).
2. Use o template de **Bug Report**.
3. Inclua:
    * Parâmetros usados (Diâmetro, Velocidade, etc).
    * Comportamento esperado vs. Comportamento real.
    * Screenshots ou logs do console.

---

## 🛡️ **Código de Conduta**

Nosso time e comunidade se comprometem a oferecer uma experiência livre de assédio para todos.
* Seja respeitoso e inclusivo.
* Aceite críticas construtivas.
* Foque no que é melhor para o projeto e para a ciência.

---

<div align="center">

**Obrigado por contribuir para a defesa planetária! 🌍☄️**

*Team Trifidia Squad*

</div>
