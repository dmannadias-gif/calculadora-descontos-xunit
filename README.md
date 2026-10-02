# Calculadora de Descontos — xUnit

Projeto da disciplina Gestão e Qualidade de Software (UNA), com o Prof. Daniel Henrique Matos de Paiva.

## [Fact] vs [Theory]

- **[Fact]**: teste sem parâmetros. Executa uma única vez e verifica um cenário fixo.
- **[Theory]**: teste parametrizado. Executa uma vez para cada `[InlineData]`, e cada conjunto de dados aparece como um teste individual. Isso evita duplicar métodos que só mudam os valores de entrada.

## Estrutura

- `CalculadoraDescontos.App`: código de produção (`DescontoService`)
- `CalculadoraDescontos.Tests`: testes unitários com xUnit (`DescontoServiceTests`)

## Como executar

Pré-requisito: .NET 10 SDK

```
dotnet test
```

Para ver cada caso de teste separadamente:

```
dotnet test --logger "console;verbosity=detailed"
```

## Licença

MIT