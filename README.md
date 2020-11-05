# Fundamentos do Node.js

Esta aplicação reforça os conhecimentos dos principais fundamentos em Node.js para construção de uma API (Application Programming Interface) que segue bons padrões de projeto.

## Conhecimentos Obtidos

Entre os conhecimentos obtidos, pode-se destacar a importância da correta utilização dos principais fundamentos do Node.js, conforme a tabela abaixo:

### Principais Fundamentos

| Fundamento    | Descrição                          |
| --------- | ---------------------------------- |
| Routes       | Responsável em receber a requisição, chamar outro arquivo (services) e devolver uma resposta. As operações de transformações de dados (parse) pode deixar na própria rota.     |
| Services      | Têm como objetivo abstrair regras de negócio das rotas, além de tornar o código mais reutilizável. O Service deve ter um nome descritivo (ex.: updateDeliveryManProfileService) e sempre possuir apenas um método (ex.: execute()). Além disso, caso outra rota ou arquivo precise executar essa  mesma ação, basta chamar e executar esse Service, obedecedo assim a outro importante princípio: DRY (Don't Repeat Yourself).   |
| Models | Define o formato dos dados e sua forma de armazenamento. |
| Repositories    | Consiste em uma ponte entre nossa aplicação e a fonte de dados, seja ela um banco de dados, um arquivo físico ou qualquer outro meio de persistência de dados da aplicação. Geralmente o Repository possui os métodos comuns de comunicação com uma fonte de dados como listagem, busca, criação, edição, remoção, mas conforme a aplicação cresce o desenvolvedor tende a encontrar outras operações repetitíveis e, com isso, popula o repositório com mais funcionalidades. |

## Tecnologias

Este projeto foi desenvolvido com as seguintes tecnologias:

- [Express](https://expressjs.com/)
- [VS Code][vc]

## Executando

Para clonar e executar este aplicativo, você precisará de [Git](https://git-scm.com), [Node.js v12.13][nodejs] ou superior + [Yarn v1.19][yarn] ou superior instalado no seu computador.

Na sua linha de comando execute:

```bash
# Clonando este repositório
$ git clone https://github.com/augustocesarfmo/fundamentos-nodejs

# Acessando o repositório
$ cd fundamentos-nodejs

# Instalando as dependências
$ yarn install

# Executando o app
$ yarn dev:server
```

## 📝 Licença

Este projeto está sob a licença MIT. Consulte a [LICENÇA](https://github.com/fradeneto/devradar-mobile/blob/master/LICENSE) para obter mais informações.

---

by Augusto César

[nodejs]: https://nodejs.org/
[yarn]: https://yarnpkg.com/
[vc]: https://code.visualstudio.com/
