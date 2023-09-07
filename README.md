# Curso Full Cycle 3.0 - Módulo Arquitetura Hexagonal (Ports and Adapters)

<div>
    <img alt="Criado por Alcir Junior [Caju]" src="https://img.shields.io/badge/criado%20por-Alcir Junior [Caju]-%23f08700">
    <img alt="License" src="https://img.shields.io/badge/license-MIT-%23f08700">
</div>

---

## Descrição

O Curso Full Cycle é uma formação completa para fazer com que pessoas desenvolvedoras sejam capazes de trabalhar em projetos expressivos sendo capazes de desenvolver aplicações de grande porte utilizando de boas práticas de desenvolvimento.

---

## Repositório Pai
https://github.com/alcir-junior-caju/study-full-cycle-3-0

---

## Visualizar o projeto na IDE:

Para quem quiser visualizar o projeto na IDE clique no teclado a tecla `ponto`, esse recurso do GitHub é bem bacana

---
### Pontos importantes sobre arquitetura
- Crescimento sustentável;
- Software precisa se pagar ao passar o tempo;
- Software deve ser desenhado por você e não pelo seu framework;
- Peças precisam se encaixar e eventualmente ser substituídas;
- Arquitetura diz respeito com o futuro do seu software;
- CRUD qualquer um faz;

#### Ciclo de vida de muitos projetos
- Fase 1:
    - Banco de dados;
    - Cadastros;
    - Validações;
    - Servidor Web;
    - Controllers;
    - Views;
    - Autenticação;
    - Upload de arquivo;
- Fase 2:
    - Regras de negócio;
    - Criação de APIs;
    - Consumo de APIs;
    - Autorização (ACL);
    - Relatórios;
    - Logs;
- Fase 3:
    - Mais acessos;
    - Upgrades hardware;
    - Cache;
    - API parceiros;
    - Regras parceiros;
    - Relatórios;
- Fase 4:
    - Mais acessos;
    - Upgrade hardware;
    - BD relatórios;
    - Comandos;
    - V2 da API;
- Fase 5:
    - Escala horizontal;
    - Sessões compartilhadas;
    - Uploads na nuvem;
    - Refatoração;
    - Autoscaling;
    - CI/CD;
- Fase 6:
    - GraphQL;
    - Bugs constantes;
    - Logs? Ops;
    - Integração CRM;
    - Migração para React;
- Fase 7:
    - Inconsistência CRM;
    - Containers;
    - CI/CD;
    - Memória;
    - Logs;
    - Se livrar do legado;
Fase 8:
    - Microserviços;
    - DB Compartilhado;
    - Problemas com tracing;
    - Lentidão;
    - Custo elevado;
- Fase 9:
    - Kubernetes;
    - CI/CD;
    - Mensageria;
    - Perda de mensagens;
    - Consultorias;
- Fase 10:
    - Use a imaginação;

#### Principais problemas
- Visão de futuro;
- Limites bem definidos;
- Troca e adição de componentes;
- Escala;
- Otimizações frequentes;
- Preparado para mudanças radicais;

#### Reflexões
- Está sendo doloroso para o dev?
- Poderia ter sido evitado?
- Software está se pagando?
- Será que a relação com o cliente está boa?
- Cliente terá prejuízo com a brusca mudança arquitetural?
- Em qual momento tudo se perdeu?
- Se você fosse novo na equipe, você julgaria os devs que fizeram tudo isso?

#### Arquitetura vs Design de software
- Atividades relacionadas a arquitetura de software são sempre de design. Entretanto, nem toda atividade de design são sobre arquitetura. O objetivo primário da arquitetura de software é garantir que os atributos de qualidade, restrições de alto nível e os objetivos de negócio, sejam atendidos pelo sistema. Qualquer decisão de design para um componente que não sejam `visíveis` fora dele, geralmente, também não são.(Elemar Jr.);

#### Arquitetura Hexagonal (Ports and Adapters)
- Permitir que um aplicativo seja igualmente conduzido por usuários, programas, testes automatizados ou scripts em lote, e que seja desenvolvido e testado isoladamente de seus eventuais dispositivos de tempo de execução e bancos de dados.(Cockburn);
- O termo `Arquitetura` Hexagonal está muito mais ligado com decisões de `Design` de software do que necessariamente de arquitetura;
- Definição de limites e proteção nas regras da aplicação;
- Componentização e desaclopamento;
    - Logs;
    - Cache;
    - Banco de Dados;
    - Comandos;
    - Filas;
    - HTTP / APIs / GraphQL;
- Facilidade na quebra para microserviços;

#### Dependency Inversion Principle
- Módulos de alto nível não devem depender de módulos de baixo nível. Ambos devem depender de abstrações;
- Abstrações não devem depender de detalhes. Detalhes devem depender de abstrações;

#### Observações
- Não há padrão estabelecidos de como códio deve ser organizado;

#### Hexagonal x Clean x Onion
- Elas seguem os mesmos pricícios da Hexagonal, mas cada um definem com mais específidades cada camada.
