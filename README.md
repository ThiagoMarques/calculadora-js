# Calculadora JS - Testes Unitários

Repositório para estudo de testes unitários utilizando TravisCI, Jasmine e Karma.

[![Build Status](https://app.travis-ci.com/ThiagoMarques/calculadora-js.svg?branch=main)](https://app.travis-ci.com/ThiagoMarques/calculadora-js)

## Sobre

Este projeto implementa uma calculadora simples em JavaScript e serve como exemplo prático para aprendizado de testes unitários, utilizando as ferramentas Jasmine e Karma, com integração contínua através do Travis CI.

## Objetivo

Demonstrar e estudar:
- Testes unitários em JavaScript
- Framework Jasmine para testes
- Karma como test runner
- Integração contínua com Travis CI
- Boas práticas de testing

## Como Usar

### Pré-requisitos
- Node.js (versão 14+ recomendada)
- npm ou yarn

### Instalação

```bash
# Clonar o repositório
git clone https://github.com/ThiagoMarques/calculadora-js.git

# Instalar dependências
npm install
```

### Executar Testes

```bash
# Executar testes com Karma
npm test

# Executar testes em modo watch
npm run test:watch

# Executar testes uma vez
npm run test:single
```

### Abrir no Navegador

```bash
# Abrir a calculadora
open index.html
# ou simplesmente abrir index.html no navegador
```

## Estrutura do Projeto

```
calculadora-js/
├── src/
│   ├── js/
│   │   ├── calculadora.js    # Lógica da calculadora
│   │   └── util.js            # Funções utilitárias
│   └── css/
│       └── calculadora.css    # Estilos
├── spec/
│   └── calculadora/
│       ├── adicionarSpec.js   # Testes de adição
│       ├── subtrairSpec.js    # Testes de subtração
│       ├── multiplicarSpec.js # Testes de multiplicação
│       └── dividirSpec.js     # Testes de divisão
├── karma.conf.js              # Configuração do Karma
├── package.json
└── README.md
```

## Tecnologias Utilizadas

- **JavaScript**: Linguagem principal
- **Jasmine**: Framework de testes BDD
- **Karma**: Test runner para JavaScript
- **Travis CI**: Integração contínua
- **HTML/CSS**: Interface da calculadora

## Funcionalidades da Calculadora

A calculadora implementa as operações básicas:
- Adição
- Subtração
- Multiplicação
- Divisão

## Exemplo de Teste

```javascript
describe("Calculadora - Adição", function() {
  it("deve somar dois números positivos", function() {
    expect(adicionar(2, 3)).toBe(5);
  });

  it("deve somar números negativos", function() {
    expect(adicionar(-2, -3)).toBe(-5);
  });

  it("deve somar zero", function() {
    expect(adicionar(5, 0)).toBe(5);
  });
});
```

## CI/CD

O projeto está configurado com Travis CI para execução automática de testes em cada push.

### Status do Build
[![Build Status](https://app.travis-ci.com/ThiagoMarques/calculadora-js.svg?branch=main)](https://app.travis-ci.com/ThiagoMarques/calculadora-js)

## Configuração do Karma

O arquivo `karma.conf.js` configura:
- Frameworks de teste (Jasmine)
- Navegadores para teste (Chrome, Firefox, etc.)
- Arquivos a serem testados
- Plugins e relatórios

## Conceitos Aprendidos

### Testes Unitários
Testam unidades individuais de código (funções) de forma isolada.

### TDD (Test-Driven Development)
Desenvolvimento guiado por testes - escrever testes antes do código.

### BDD (Behavior-Driven Development)
Foco no comportamento esperado, usando linguagem natural.

### Integração Contínua
Execução automática de testes a cada mudança no código.

## Contribuindo

Contribuições são bem-vindas! Áreas de interesse:
- Novas funcionalidades da calculadora
- Mais casos de teste
- Melhorias na interface
- Documentação

## Licença

Este projeto é de código aberto e está disponível para fins educacionais.

## Links Úteis

- [Jasmine Documentation](https://jasmine.github.io/)
- [Karma Documentation](https://karma-runner.github.io/)
- [Travis CI](https://travis-ci.com/)
- [JavaScript Testing Best Practices](https://github.com/goldbergyoni/javascript-testing-best-practices)

---

**Autor**: Thiago Marques  
**Frameworks**: Jasmine, Karma  
**CI/CD**: Travis CI
