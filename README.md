# Curso de Java - Rockseat

## Primeira aula

### Como criar a aplicação

Formas de criar um projeto Java com o Framework JavaSpring: 

1. Utilizando o site [spring initializer](https://start.spring.io/);
2. Por meio do **Maven**;
3. Usando o próprio vscode.

> A forma mais fácil é por meio do site.

#### Como criar o projeto por meio do spring initializer

|              Campo               |               Valor/opção a informar               |
| :------------------------------: | :------------------------------------------------: |
|             Project              |                       Maven                        |
|             Language             |                        Java                        |
|           Spring Boot            |    Qualquer versão, evitando as SNAPSHOT(betas)    |
|     Project Metadata - Group     | Domínio da app invertido, exemplo: **br.com.luiz** |
| Project Metadata - Artifact/Name |                  Nome do projeto                   |
|  Project Metadata - Description  |                Descrição do projeto                |
| Project Metadata - Package name  |                  Manter o padrão                   |
|            Packaging             |                        JAR                         |
|          Versão do Java          |                        17+                         |
|           Dependencies           |                     Spring WEB                     |

### Estrutura do projeto

#### .mnv

Gerenciador de pacotes da aplicação.

#### src 

Coração da aplicação, contendo as pastas:

1. **main**
    - java: código fonte.
    - resources: templates e propriedades do projeto.

### Anotations

O framework javaspring é dependente das anotações para seu funcionamento, onde cada uma possui uma responsabilidade de indicar uma funcionalidade.

Exemplo de anotações: 

1. `@Controller`: utilziado em controllers que irão retornar alguma informação sem ser uma request;

2. `@RestController`: usado por controllers que são a camada de comunicação do cliente e a aplicação por meio das requests;

3. `@RequestMapping("/rota")`: tag obrigatória para informar a rota de acesso a um controller, exemplo: `localhost:8080/users`;

4. `@GetMapping("/rotaGet")`: define a rota para o tipo get;

5. `@PostMapping("/rotaPost")`: define a rota para o tipo post;

### Métodos de acesso HTTP

1. **GET**: buscar uma informação;
2. **POST**: adicionar uma informação;
3. **PUT**: alterar um dado/infomarção;
4. **DELETE**: remover um dado;
5. **PATCH**: alterar somente uma parte da informação/dado.

> Mais informações acessíveis em: [Métodos de requisição HTTP](https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Methods)



