# 🌿 Calculadora de Emissão de CO₂

Uma aplicação web interativa para calcular a emissão de carbono das suas viagens com base no meio de transporte utilizado e na distância percorrida.

## 🎯 Funcionalidades

- ✅ **Cálculo de Emissões**: Calcule a emissão de CO₂ para diferentes meios de transporte
- ✅ **Autocomplete de Cidades**: Digite a cidade de origem e destino com sugestões automáticas
- ✅ **Distância Automática**: A distância é preenchida automaticamente baseada nas cidades selecionadas
- ✅ **Múltiplos Meios de Transporte**: Bicicleta 🚲, Carro 🚗, Ônibus 🚌 e Caminhão 🚚
- ✅ **Comparação de Emissões**: Veja a comparação entre todos os meios de transporte
- ✅ **Créditos de Carbono**: Saiba quantos créditos de carbono equivalem à sua emissão
- ✅ **Entrada Manual**: Opção para inserir a distância manualmente

## 📋 Tecnologias

- **Frontend**: HTML5, CSS3, JavaScript Vanilla
- **Banco de Dados**: Rotas brasileiras com distâncias em km
- **Deploy**: GitHub Pages com GitHub Actions

## 📁 Estrutura do Projeto

```
carbon_calculator/
├── index.html              # Página principal da aplicação
├── css/
│   └── style.css          # Estilos da aplicação
├── js/
│   ├── app.js             # Lógica principal da aplicação
│   ├── calculator.js      # Funções de cálculo de emissões
│   ├── config.js          # Configurações e dados da aplicação
│   ├── routes-data.js     # Base de dados de rotas brasileiras
│   └── ui.js              # Funções de manipulação da UI
├── .github/
│   └── workflows/
│       └── deploy.yml     # Configuração de deploy automático
└── README.md              # Este arquivo
```

## 🚀 Como Usar

### Opção 1: Abrir no Navegador
1. Clique duas vezes em `index.html` ou arraste-o para seu navegador

### Opção 2: Usar um Servidor Local (Recomendado)

**Com Python:**
```bash
python -m http.server 8000
# Acesse: http://localhost:8000
```

**Com Node.js:**
```bash
npx http-server
# ou
npx serve
```

## 📊 Como Funciona

1. **Selecione as Cidades**: Digite a cidade de origem e destino
2. **Escolha o Transporte**: Selecione entre bicicleta, carro, ônibus ou caminhão
3. **Calcule**: Clique no botão "Calcular Emissão"
4. **Visualize os Resultados**: Veja a emissão de CO₂ em kg
5. **Compare**: Analise a comparação com outros meios de transporte
6. **Saiba sobre Créditos**: Descubra o equivalente em créditos de carbono

## 📈 Fatores de Emissão por km

| Transporte | Emissão (kg CO₂/km) |
|-----------|-------------------|
| Bicicleta | 0 kg |
| Ônibus | 0.089 kg |
| Carro | 0.12 kg |
| Caminhão | 0.96 kg |

## 🌐 Deploy no GitHub Pages

O projeto possui configuração automática de deploy via GitHub Actions:

1. Faça push para a branch `main`
2. O GitHub Actions automaticamente fará o deploy
3. Acesse: `https://seu-usuario.github.io/carbon_calculator/`

## 🔧 Instalação Local para Desenvolvimento

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/carbon_calculator.git

# Acesse a pasta
cd carbon_calculator

# Inicie um servidor local (Python)
python -m http.server 8000

# Abra no navegador
# http://localhost:8000
```
---

**Dicas úteis:**
- 🌍 As rotas incluem cidades brasileiras de todas as regiões
- 💡 Use a opção de inserção manual para calcular distâncias personalizadas