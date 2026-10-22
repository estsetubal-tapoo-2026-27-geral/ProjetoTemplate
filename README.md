# Projeto TAPOO – Template

Template Maven (JavaFX + [SmartGraph](https://github.com/brunomnsilva/JavaFXSmartGraph) + JUnit) para o projeto de TAPOO.

## Requisitos

- JDK **17 ou superior** (o projeto compila com `release 17`)
- Maven 3.9+ (ou o Maven integrado no IDE)
- JavaFX 21 (descarregado automaticamente pelo Maven)

## Como começar

### 1. Criar o repositório a partir do template

1. Nesta página do template, clicar em **Use this template** → **Create a new repository**.
2. Escolher como *Owner* a conta pessoal do elemento do grupo que está a criar o repositório.
3. Dar ao repositório um nome que identifique o grupo (ex.: `Projeto-GrupoXX`).
4. Em *Visibility*, escolher **Private**.
5. Clicar em **Create repository**.

> Se o repositório ficou público, ir a **Settings → General → Danger Zone → Change visibility** e alterá-lo para **Private**.

### 2. Adicionar o docente e os colegas de grupo

Só quem tem permissões de administração do repositório (quem o criou) consegue fazer isto:

1. No repositório, abrir **Settings**.
2. No menu lateral, escolher **Collaborators** (em *Access*).
3. Clicar em **Add people**.
4. Pesquisar pelo *username* GitHub (ou e-mail) de cada colega de grupo e do docente e confirmar.
5. Cada pessoa convidada tem de **aceitar o convite** (recebido por e-mail ou em <https://github.com/notifications>).

**Adicionar o docente da vossa turma** como colaborador:

| Docente | Utilizador GitHub | Turmas |
|---------|-------------------|--------|
| Bruno Silva | [`brunomnsilva-estsetubal`](https://github.com/brunomnsilva-estsetubal) | PL4, PL5 |
| Patrícia Macedo | [`patriciamacedo`](https://github.com/patriciamacedo) | PL1, PL3, PL7 |
| Pedro Albuquerque Santos | [`petersaints`](https://github.com/petersaints) | PL2, PL6 |

### 3. Clonar e executar

```bash
git clone <url-do-repositorio>
cd <nome-do-repositorio>
mvn            # compila e executa a aplicação (compile javafx:run)
mvn test       # executa os testes
```

## Estrutura Base

- `src/main/java/pt/unips/tapoo` – código da aplicação (`Main`, `GraphApp`)
- `src/test/java/pt/unips/tapoo` – testes JUnit
- `smartgraph.properties` / `smartgraph.css` – configuração e estilo da visualização do grafo
