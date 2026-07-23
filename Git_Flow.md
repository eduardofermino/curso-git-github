# Git Flow

**GitFlow** é um workflow que visa **organizar o desenvolvimento e lançamento de software** através de branches estruturadas, separando etapas de criação de funcionalidades, preparação para releases e correções de bugs com emergência.

---

## Conceito

* **Proteger a branch `main`:** A branch `main` representa o código de **produção** e **não deve receber commits diretos**.
* **A branch `develop` como Guardrail:** É criada uma branch chamada `develop` a partir da `main`. Ela funciona como um **ambiente de integração provisório** onde todas as novas alterações são testadas e consolidadas antes de subirem para a `main`.

---

## Estrutura de Branches e Nomenclatura

* **`main`** — Código estável em produção.
* **`develop`** — Linha principal para integração das novas funcionalidades.
* **`feature/*`** — Branches para desenvolvimento de novas funcionalidades (criadas a partir da `develop`).
* **`release/*`** — Branches de preparação para novos lançamentos e testes finais (criadas a partir da `develop`).
* **`hotfix/*`** — Branches para correções urgentes diretamente em produção (criadas a partir da `main`).
