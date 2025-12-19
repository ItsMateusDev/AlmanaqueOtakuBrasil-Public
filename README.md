# 🚀 Anime Data Engine | React 19 & TypeScript

Este projeto representa uma implementação robusta de frontend moderno, focado em alta performance e resiliência. A aplicação consome dados da **Anime News Network**, transformando um fluxo de dados legado (XML) em uma experiência de usuário fluida e tipada.

## 🛠️ Stack Tecnológica

* **Core:** React 19 & TypeScript
* **Arquitetura:** Modular e Escalável
* **Processamento de Dados:** DOMParser (XML para Objeto)
* **UX/UI:** Skeleton Screens & Gerenciamento de Estado Complexo

---

## 🏗️ Desafios Técnicos & Soluções

Trabalhar com APIs tradicionais exige um cuidado que vai além do convencional. Abaixo, destaco como as principais barreiras foram superadas:

### 📄 Parsing de XML e Integridade

Diferente do padrão JSON, a API utilizada entrega dados em **XML**. Para garantir a segurança e a consistência no frontend:

* Implementação de uma camada de **parsing via DOMParser**.
* Tratamento rigoroso de **interfaces TypeScript** para garantir que a tipagem flua corretamente por toda a aplicação.

### 🚦 Controle de Concorrência e Rate Limit

A API possui uma restrição estrita de **1 requisição por segundo**. Para evitar bloqueios e garantir a estabilidade:

* **Throttle:** Lógica de controle de concorrência assíncrona com intervalos de segurança.
* **Dynamic Proxy:** Integração de um proxy dinâmico para contornar restrições de **CORS**.

---

## ⚡ Performance e Experiência do Usuário (UX)

A aplicação não apenas entrega os dados, mas se preocupa com *como* eles chegam ao usuário:

* **Skeleton Screens:** Utilizados para mitigar a percepção de carregamento em dados massivos, mantendo o layout estável.
* **Estado Complexo:** Sistema de filtros e paginação que operam de forma simultânea e reativa.
* **Resiliência:** Tratamento de erros avançado que mantém a aplicação funcional mesmo sob instabilidades de rede ou latência da API.

> "A estabilidade de um sistema é provada nos momentos de estresse da rede."
