<div align="center">
  <img src="logo/dark.png" alt="Alpa Gateway API" width="200" />
  
  # Alpa Gateway API - Documentação Pública
  
  [![Documentation](https://img.shields.io/badge/Documentation-Live-brightgreen)](https://docs.usealpa.com)
  [![API Version](https://img.shields.io/badge/API-v1.0-blue)](https://alpa-sistema-api.onrender.com)
  [![License](https://img.shields.io/badge/License-MIT-purple)](LICENSE)
  [![Node.js SDK](https://img.shields.io/badge/SDK-Node.js-339933?logo=node.js&logoColor=white)](pages/sdk-nodejs.mdx)
  [![Python SDK](https://img.shields.io/badge/SDK-Python-3776AB?logo=python&logoColor=white)](pages/sdk-python.mdx)
  [![PHP SDK](https://img.shields.io/badge/SDK-PHP-777BB4?logo=php&logoColor=white)](pages/sdk-php.mdx)
  [![Java SDK](https://img.shields.io/badge/SDK-Java-ED8B00?logo=java&logoColor=white)](pages/sdk-java.mdx)
  
  **Documentação oficial e completa da API Alpa Gateway**
  
  Plataforma completa de pagamentos com PIX, cartão de crédito/débito, boleto bancário e muito mais.
</div>

---

## 📋 Sobre

A **Alpa Gateway API** é uma solução completa de processamento de pagamentos desenvolvida para oferecer integração simples, segura e eficiente. Esta documentação fornece todas as informações necessárias para desenvolvedores integrarem pagamentos em suas aplicações.

### Características Principais

- ✅ **API RESTful moderna** - Endpoints intuitivos e bem documentados
- ✅ **Múltiplos métodos de pagamento** - PIX, Cartão de Crédito/Débito e Boleto Bancário
- ✅ **Links de pagamento personalizados** - Crie e compartilhe links únicos com configurações flexíveis
- ✅ **Gestão completa de produtos** - Catálogo integrado com controle de estoque
- ✅ **Sistema de cupons** - Descontos percentuais ou valores fixos com regras configuráveis
- ✅ **Gestão de clientes** - Cadastro e consulta de clientes
- ✅ **Saques e antecipações** - Solicite saques e antecipações de recebíveis
- ✅ **Programa de afiliados** - Crie e gerencie programas de afiliados com comissões
- ✅ **Assinaturas recorrentes** - Planos e cobranças automáticas por assinatura
- ✅ **Advanced Sales Tracking (Utmify)** - Suporte completo para UTMs, fbclid, gclid e src
- ✅ **Webhooks em tempo real** - Notificações instantâneas sobre eventos importantes
- ✅ **Dashboard administrativo** - Interface completa para gerenciamento e relatórios
- ✅ **SDKs oficiais** - Bibliotecas para Node.js, Python, PHP e Java
- ✅ **Documentação interativa** - Exemplos práticos e referência completa da API

## 🚀 Início Rápido

### Para Desenvolvedores

1. **Obtenha suas credenciais de API**
   - Acesse o [Dashboard Alpa](https://app.usealpa.com)
   - Complete o processo de verificação (KYC)
   - Gere sua API Key em **Configurações → Credenciais de API**

2. **Faça sua primeira requisição**
   ```bash
   curl -X GET "https://alpa-sistema-api.onrender.com/api/v1/payment-links" \
     -H "Authorization: Bearer SUA_API_KEY" \
     -H "Content-Type: application/json"
   ```

3. **Explore a documentação**
   - [Guia de Início Rápido](pages/quickstart.mdx)
   - [Autenticação](pages/authentication.mdx)
   - [Referência Completa da API](api-reference/openapi.json)
   - [SDKs disponíveis](pages/sdks.mdx)

## 📚 Estrutura do Projeto

```
documentação_alpa/
├── api-reference/              # Especificação OpenAPI e referência de endpoints
│   └── openapi.json            # Especificação OpenAPI 3.0.3 completa
├── pages/                      # Conteúdo principal da documentação
│   ├── guides/                 # Guias e tutoriais detalhados
│   │   └── features/           # Guias específicos por funcionalidade
│   ├── payment-links/          # Documentação de Links de Pagamento
│   ├── products/               # Documentação de Produtos
│   ├── customers/              # Documentação de Clientes
│   ├── coupon/                 # Documentação de Cupons
│   ├── transactions/           # Documentação de Transações
│   ├── balance/                # Documentação de Saldo
│   ├── withdrawals/            # Documentação de Saques
│   ├── affiliates/             # Documentação de Afiliados
│   ├── subscriptions/          # Documentação de Assinaturas
│   ├── advances/               # Documentação de Antecipações
│   ├── webhooks/               # Documentação de Webhooks
│   ├── quickstart.mdx          # Guia de início rápido
│   ├── authentication.mdx      # Autenticação e segurança
│   ├── webhooks.mdx            # Visão geral de webhooks
│   ├── glossary.mdx            # Glossário de termos
│   ├── sdks.mdx                # Visão geral dos SDKs
│   ├── sdk-nodejs.mdx          # SDK Node.js
│   ├── sdk-python.mdx          # SDK Python
│   ├── sdk-php.mdx             # SDK PHP
│   ├── sdk-java.mdx            # SDK Java
│   └── changelog.mdx           # Histórico de alterações
├── images/                     # Imagens e assets visuais
├── logo/                       # Logos para temas claro e escuro
├── custom.css                  # Estilos customizados (scrollbar, etc.)
├── docs.json                   # Configuração principal do Mintlify
├── favicon.ico                 # Ícone do site
└── README.md                   # Este arquivo
```

### Adicionando Novo Conteúdo

1. **Nova página de guia**: Adicione arquivo `.mdx` em `pages/guides/`
2. **Novo endpoint**: Atualize `api-reference/openapi.json` e crie página em `pages/[recurso]/`
3. **Atualizar navegação**: Edite `docs.json` na seção `navigation`

### Convenções

- Use Markdown/MDX para formatação
- Siga a estrutura de pastas existente
- Mantenha consistência com o tom e estilo da documentação
- Inclua exemplos de código quando relevante

**URL da Documentação**: [https://docs.usealpa.com](https://docs.usealpa.com)

## 📖 Recursos da API

### Endpoints Principais

| Recurso | Descrição | Documentação |
|---------|-----------|--------------|
| **Links de Pagamento** | Crie e gerencie links personalizados | [Ver Documentação](pages/payment-links/reference.mdx) |
| **Produtos** | Gerencie seu catálogo de produtos | [Ver Documentação](pages/products/reference.mdx) |
| **Clientes** | Cadastre e consulte clientes | [Ver Documentação](pages/customers/reference.mdx) |
| **Cupons** | Sistema completo de cupons de desconto | [Ver Documentação](pages/coupon/reference.mdx) |
| **Transações** | Consulte e gerencie transações | [Ver Documentação](pages/transactions/reference.mdx) |
| **Saldo** | Consulte saldo e movimentações | [Ver Documentação](pages/balance/reference.mdx) |
| **Saques** | Solicite e gerencie saques | [Ver Documentação](pages/withdrawals/reference.mdx) |
| **Afiliados** | Programas de afiliados e comissões | [Ver Documentação](pages/affiliates/reference.mdx) |
| **Assinaturas** | Planos recorrentes e cobranças automáticas | [Ver Documentação](pages/subscriptions/reference.mdx) |
| **Antecipações** | Solicite antecipação de recebíveis | [Ver Documentação](pages/advances/reference.mdx) |
| **Webhooks** | Configure notificações em tempo real | [Ver Documentação](pages/webhooks/reference.mdx) |

### Autenticação

A API utiliza autenticação via **API Key** (Bearer Token). Todas as requisições autenticadas devem incluir o header:

```
Authorization: Bearer SUA_API_KEY
```

Para mais detalhes, consulte a [documentação de autenticação](pages/authentication.mdx).

## 🛠️ SDKs Oficiais

| Linguagem | Instalação | Documentação |
|-----------|-----------|--------------|
| **Node.js** | `npm install alpa-sdk` | [Ver Documentação](pages/sdk-nodejs.mdx) |
| **Python** | `pip install alpa-sdk` | [Ver Documentação](pages/sdk-python.mdx) |
| **PHP** | `composer require alpa/sdk` | [Ver Documentação](pages/sdk-php.mdx) |
| **Java** | Maven / Gradle | [Ver Documentação](pages/sdk-java.mdx) |

## 🔗 Links Importantes

### Documentação e Recursos

- **Documentação Online**: [https://docs.usealpa.com](https://docs.usealpa.com)
- **API Base URL**: `https://alpa-sistema-api.onrender.com`
- **Dashboard**: [https://app.usealpa.com](https://app.usealpa.com)
- **Status da API**: [https://status.usealpa.com](https://status.usealpa.com)
- **Changelog**: [Ver histórico de alterações](pages/changelog.mdx)

### Repositórios

- **Documentação**: [GitHub Repository](https://github.com/anthonymengottii/documentation_alpa)
- **Sistema Principal**: [GitHub Repository](https://github.com/anthonymengottii/alpa_sistema)

### Suporte

- **Email**: [suporte@usealpa.com](mailto:suporte@usealpa.com)
- **Issues**: [GitHub Issues](https://github.com/anthonymengottii/documentation_alpa/issues)
- **Glossário**: [Ver Glossário](pages/glossary.mdx)

## 🤝 Contribuindo

Contribuições são bem-vindas! Se você encontrar erros, tiver sugestões ou quiser adicionar conteúdo:

1. Abra uma [Issue](https://github.com/anthonymengottii/documentation_alpa/issues) descrevendo sua proposta
2. Faça um Fork do repositório
3. Crie uma branch para sua alteração (`git checkout -b feature/minha-contribuicao`)
4. Faça commit das alterações (`git commit -m 'Adiciona nova funcionalidade'`)
5. Faça push para a branch (`git push origin feature/minha-contribuicao`)
6. Abra um Pull Request

## 📝 Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

---

<div align="center">
  <p>
    <strong>Alpa Gateway API</strong> - Simplificando pagamentos online
  </p>
</div>
