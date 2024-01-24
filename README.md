### O Projeto:

Projeto do livro: [Desenvolvimento de Backend com Node.js, TypeScript, MongoDB e Docker: Práticas Avançadas com TDD, DDD, Clean Architecture e SOLID
](https://www.amazon.com.br/gp/product/B0CGCCMY2Q/ref=kinw_myk_ro_title)

---

### :raising_hand: Sobre Min:

 [![linkedin](https://img.shields.io/badge/Acesse%20o%20meu-linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jos%C3%A9-r-99896a39/) [![twitter](https://img.shields.io/badge/Acesse%20o%20meu-twitter-1D9BF0?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/aromademirtilo) [![Instagram](https://img.shields.io/badge/Acesse%20o%20meu-Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/learningenuity/) ![Badge Status](https://img.shields.io/badge/STATUS-EM_DESENVOLVIMENTO-green?style=for-the-badge)

---

#### :keyboard: Snippet para criar testes em jest no VsCode:
No menu do `VsCode` acesse `Arquivo > Preferências > Configurar Snippets de Usuário` criar um snippt chamado `javascript.json` e inserir o seguinte código:
```javascript
{
  "JestTest": {
    "prefix": ["test"],
    "body": [
      "describe('Describe HERE', () => {",
      "	test('Test HERE', () => {",
      "		",
      "	})",
      "})",
    ],
    "description": "Bloco Jest"
  }
}
```

---

#### :bar_chart: Diagrama do projeto usando Clean Architecture:
<img src="./docs/images/project_clean_architecture_diagram.png">

_Imagem retirada do livro_


---

#### :wolf: Configurando Husky:
```bash
$ mkdir .husky
$ npx husky add .husky/commit-msg ".git/hooks/commit-msg \$1"
$ ln -s ../.husky/commit-msg .git/hooks/commit-msg
```
`.huskyrc.json`:
```json
{
    "hooks": {
        "pre-commit": "lint-staged",
        "pre-push": "1"
    }
}
```