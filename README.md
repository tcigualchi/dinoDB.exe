# DinoDB 🦖

**DinoDB** é um aplicativo desktop para Windows desenvolvido em Java para explorar um catálogo de aproximadamente **1.800 dinossauros**. O projeto reúne pesquisa, filtros, detalhes das espécies, estatísticas e um minigame em uma interface gráfica.

## Funcionalidades

- Pesquisa por nome, tradução, identificador, período, localidade e descrição.
- Filtros por dieta e período geológico.
- Visualização de informações detalhadas sobre cada dinossauro.
- Estatísticas do catálogo.
- Recarga dos dados sem precisar reiniciar o aplicativo.
- API HTTP local para consultar os dados.
- Minigame desenvolvido em JavaScript com Canvas.

## Tecnologias

| Tecnologia | Uso no projeto |
| --- | --- |
| Java e JavaFX | Aplicativo desktop e interface gráfica |
| FXML e CSS | Estrutura e apresentação da interface |
| Jackson e JSON | Leitura e processamento do catálogo |
| `HttpServer` | API HTTP local |
| JavaScript e Canvas | Desenvolvimento do minigame |
| `jpackage` | Distribuição da aplicação para Windows |

Os registros são carregados de arquivos JSON e consultados em memória. **DinoDB não utiliza um banco de dados SQL ou NoSQL**, apesar do nome.

## 🎮 Minigame e artes

O **minigame presente no DinoDB**, assim como suas **artes e elementos visuais**, foram desenvolvidos pelo meu amigo **Takeshi**.

GitHub: [@paulooka2007](https://github.com/paulooka2007)

Ele foi responsável pela programação do jogo utilizando **JavaScript e Canvas**, além da criação das artes utilizadas nessa parte do projeto.

## Como executar

1. Baixe a versão distribuída do projeto.
2. O arquivo completo pode ser baixado pelo Google Drive, pois seu tamanho ultrapassa o limite permitido pelo GitHub:

   https://drive.google.com/file/d/1vAx7REx3Tm_I9tmos-skO6cotjCTg_tl/view

3. Extraia o pacote completo, preservando a estrutura de pastas.
4. No Windows, execute `DinoDB.exe`.

A distribuição portátil inclui o runtime Java e as dependências necessárias; **não é preciso instalar o Java separadamente**.

Mantenha os arquivos do pacote junto ao executável para que o catálogo, o minigame e os demais recursos funcionem corretamente.

## API local

Com o aplicativo em execução, a API fica disponível em:

`http://127.0.0.1:3000`

Ela é destinada a consultas na própria máquina. Os caminhos específicos dos endpoints podem ser documentados conforme a versão publicada do aplicativo.

## Sobre esta versão do repositório

Esta distribuição contém a aplicação compilada.

O código Java está empacotado em `dinodb-app.jar`; os arquivos-fonte `.java`, os testes e a configuração de compilação (Maven ou Gradle) não estão incluídos nesta versão.

Portanto, o executável é a forma indicada para experimentar o projeto.

## Autores e colaboradores

### 🦖 João Victor Gualchi

Desenvolvimento da aplicação **DinoDB**, incluindo:

- aplicação desktop em Java e JavaFX;
- sistema de pesquisa e filtros;
- processamento do catálogo;
- estatísticas;
- API HTTP local;
- integração dos recursos da aplicação;
- empacotamento e distribuição para Windows.

### 🎨 Takeshi — [@paulooka2007](https://github.com/paulooka2007)

Responsável por:

- programação do minigame;
- desenvolvimento em JavaScript e Canvas;
- criação das artes;
- elementos visuais utilizados no jogo.

---

Desenvolvido como **projeto acadêmico**, unindo Java, interfaces gráficas, processamento de dados e desenvolvimento de jogos.
