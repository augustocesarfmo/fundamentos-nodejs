# <span id="head1">Fundamentos do Node.js</span>

Esta aplicação reforça os conhecimentos dos principais fundamentos em Node.js para construção de uma API (Application Programming Interface) que segue bons padrões de projeto.

- [Fundamentos do Node.js](#head1)
  - [📚 Principais fundamentos](#head2)
  - [🚀 Tecnologias](#head3)
  - [ℹ️ Executando](#head4)
  - [📝 Licença](#head5)

## <span id="head2">📚 Principais fundamentos</span>

| Fundamento    | Descrição                          |
| --------- | ---------------------------------- |
| Routes       | Responsável em receber a requisição, chamar outro arquivo (services) e devolver uma resposta. As operações de transformações de dados (parse) pode deixar na própria rota.     |
| Services      | Têm como objetivo abstrair regras de negócio das rotas, além de tornar o código mais reutilizável. O Service deve ter um nome descritivo (ex.: updateDeliveryManProfileService) e sempre possuir apenas um método (ex.: execute()). Além disso, caso outra rota ou arquivo precise executar essa  mesma ação, basta chamar e executar esse Service, obedecedo assim a outro importante princípio: DRY (Don't Repeat Yourself).   |
| Models | Define o formato dos dados e sua forma de armazenamento. |
| Repositories    | Consiste em uma ponte entre nossa aplicação e a fonte de dados, seja ela um banco de dados, um arquivo físico ou qualquer outro meio de persistência de dados da aplicação. Geralmente o Repository possui os métodos comuns de comunicação com uma fonte de dados como listagem, busca, criação, edição, remoção, mas conforme a aplicação cresce o desenvolvedor tende a encontrar outras operações repetitíveis e, com isso, popula o repositório com mais funcionalidades. |

## <span id="head3">🚀 Tecnologias</span>

Este projeto foi desenvolvido com as seguintes tecnologias:

- [express](https://expressjs.com/)
- [vs code][vc]

## <span id="head4">ℹ️ Executando</span>

Para clonar e executar este aplicativo, você precisará do [Git](https://git-scm.com), [Node.js v12.13][nodejs] ou superior + [Yarn v1.19][yarn] ou superior instalado no seu computador.

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

## <span id="head5">📝 Licença</span>

Este projeto está sob a licença MIT. Consulte a [LICENÇA](https://github.com/augustocesarfmo/fundamentos-nodejs/blob/master/LICENSE.md) para obter mais informações.

---

by Augusto César Oliveira 👐🏼

[nodejs]: https://nodejs.org/
[yarn]: https://yarnpkg.com/
[vc]: https://code.visualstudio.com/
