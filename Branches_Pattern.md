# Padronização de Branches

Padrão de nomenclatura para criação de branches no Git, garantindo organização, clareza no fluxo de trabalho e facilidade na identificação do objetivo de cada branch.

---

## Tipos de Branches e Exemplos

| Prefixo | Finalidade / Quando Usar | Exemplo Prático |
| :--- | :--- | :--- |
| `feature/` ou `feat/` | **Nova funcionalidade:** Desenvolvimento de uma nova tela, recurso, API ou lógica de negócio. | `feature/login-com-google`<br>`feat/TASK-102-filtro-de-produtos` |
| `fix/` ou `bugfix/` | **Correção de bug:** Correção de falhas encontradas durante o desenvolvimento ou testes em ambiente interno. | `fix/erro-calculo-frete`<br>`bugfix/ISSUE-45-quebra-layout-mobile` |
| `hotfix/` | **Correção urgente em Produção:** Correção crítica de erro que está acontecendo no sistema ao vivo (produção). | `hotfix/falha-processamento-pagamento`<br>`hotfix/PROD-88-vazamento-memoria` |
| `refactor/` | **Refatoração:** Melhoria ou reestruturação de código existente sem alterar o comportamento final. | `refactor/simplifica-service-autenticacao` |
| `release/` | **Preparação de lançamento:** Preparação e homologação de uma nova versão do software para subir para produção. | `release/v1.2.0`<br>`release/v2026.04` |
| `chore/` | **Manutenção / Configuração:** Ajustes de ambiente, atualização de dependências, CI/CD ou ferramentas externas. | `chore/atualiza-dockerfile` |
| `docs/` | **Documentação:** Criação ou alteração exclusiva de arquivos de documentação (ex: `README.md`, Swagger). | `docs/atualiza-guia-instalacao` |

---

## Regras e Boas Práticas

1. **Use apenas letras minúsculas:**
   * ✅ `feature/cadastro-usuario`
   * ❌ `feature/CadastroUsuario` ou `feature/CADASTRO_USUARIO`

2. **Separe palavras com hífen (`-`):**
   * ✅ `fix/validacao-email`
   * ❌ `fix/validacao_email` ou `fix/validacaoemail`

3. **Seja conciso e descritivo:**
   * ✅ `feature/recuperacao-senha`
   * ❌ `feature/tela` ou `feature/ajusta-o-fluxo-onde-o-usuario-esqueceu-a-senha`

4. **Evite nomes genéricos:**
   * Evite nomes como `testes`, `ajustes`, `desenvolvimento` ou seu próprio nome na branch.

5. **Limpeza após o Merge:**
   * Após o Pull Request (PR) ser aprovado e integrado à branch principal, exclua a branch (`git branch -D <nome>`) para manter o repositório limpo.
