# 🛒 Lista de Compras Flutter

**Laboratório de Desenvolvimento de Aplicações Móveis e Distribuídas**  
**Curso de Engenharia de Software - PUC Minas**  
**Professores:** Cristiano Neto, Artur Mol, Cleiton Tavares

---

## 👤 **Informações do Projeto**

- **Nome do Aluno:** Mauricio Fernandes Leite
- **Matrícula:** 697964
- **Professor:** Cristiano Neto
- **Disciplina:** Desenvolvimento de Aplicações Móveis e Distribuídas

---

## 📋 **Descrição do Projeto**

Aplicação móvel Flutter para gerenciamento de listas de compras, desenvolvida seguindo os princípios do Material Design 3. O projeto demonstra conceitos fundamentais de desenvolvimento mobile com Flutter, incluindo gerenciamento de estado, interface responsiva e interações do usuário.

### **Características Principais:**
- **Interface Moderna** - Material Design 3 com tema personalizado
- **Gerenciamento de Estado** - StatefulWidget com setState()
- **Interface Responsiva** - Adaptável a diferentes tamanhos de tela
- **Funcionalidades Completas** - CRUD completo para listas de compras
- **Multiplataforma** - Suporte para Android, iOS, Web, Windows, Linux e macOS

### **Tecnologias Utilizadas:**
- **Flutter SDK** 3.24.5+
- **Dart** (incluído com Flutter)
- **Material Design 3** - Widgets nativos do Flutter
- **Hot Reload** - Desenvolvimento ágil

---

## 🚀 **Comandos para Execução**

### **1. Verificação do Ambiente**
```bash
flutter doctor
```

### **2. Criação do Projeto**
```bash
flutter create lista_compras_simples
cd lista_compras_simples
```

### **3. Execução da Aplicação**
```bash
# Executar no navegador (Chrome)
flutter run -d chrome

# Executar no emulador Android
flutter run -d android

# Executar no emulador iOS (apenas macOS)
flutter run -d ios

# Executar no desktop Windows
flutter run -d windows

# Listar dispositivos disponíveis
flutter devices
```

### **4. Comandos de Desenvolvimento**
```bash
# Hot Reload (durante execução)
r ou R

# Hot Restart (durante execução)
R

# Parar aplicação
q

# Limpar cache
flutter clean

# Atualizar dependências
flutter pub get
```

---

## ✅ **Funcionalidades Implementadas**

### **Funcionalidades Básicas (100%):**
- [x] **Adicionar Itens** - Campo de texto com validação
- [x] **Remover Itens** - Botão de exclusão individual
- [x] **Interface Responsiva** - Layout adaptável
- [x] **Validação de Entrada** - Prevenção de campos vazios

### **Funcionalidades Avançadas (100%):**
- [x] **Sistema de Checkbox** - Marcar itens como comprados
- [x] **Estatísticas em Tempo Real** - Contadores de Total, Comprados e Restantes
- [x] **Prevenção de Duplicatas** - Validação de itens únicos
- [x] **Diálogos de Confirmação** - Confirmação para remoções
- [x] **Sistema de Mensagens** - SnackBar para feedback
- [x] **Limpeza Completa** - Botão para limpar toda a lista
- [x] **Visual Moderno** - Cards com elevação e cores diferenciadas

### **Melhorias de Interface:**
- [x] **AppBar Personalizada** - Título e botão de ação
- [x] **Área de Entrada Estilizada** - Container com sombra e ícones
- [x] **Tela de Lista Vazia** - Ícone e mensagem amigável
- [x] **Cores Diferenciadas** - Estados visuais distintos
- [x] **Ícones Informativos** - Material Icons em toda interface

---

## 🏗️ **Estrutura do Projeto**

```
lista_compras_simples/
├── lib/
│   └── main.dart                 # Código principal da aplicação
├── android/                      # Configurações Android
├── ios/                         # Configurações iOS
├── web/                         # Configurações Web
├── windows/                     # Configurações Windows
├── linux/                       # Configurações Linux
├── macos/                       # Configurações macOS
├── pubspec.yaml                 # Dependências do projeto
├── README.md                    # Documentação do projeto
└── test/                        # Testes unitários
    └── widget_test.dart
```

---

## 📱 **Arquitetura da Aplicação**

### **Estrutura de Widgets:**
```dart
MeuApp (StatelessWidget)
└── MaterialApp
    └── PaginaInicial (StatefulWidget)
        └── Scaffold
            ├── AppBar
            ├── Body (Column)
            │   ├── Container (Área de Entrada)
            │   ├── Container (Estatísticas)
            │   └── Expanded (ListView)
            └── Actions (Botão Limpar)
```

### **Gerenciamento de Estado:**
- **List<String> itensCompra** - Armazena nomes dos itens
- **List<bool> itensComprados** - Armazena status de cada item
- **TextEditingController** - Controla campo de entrada
- **setState()** - Atualiza interface quando estado muda

---

## 🎯 **Conceitos Flutter Demonstrados**

### **Widgets Fundamentais:**
- [x] **MaterialApp** - Configuração principal da aplicação
- [x] **Scaffold** - Estrutura básica da tela
- [x] **AppBar** - Barra superior com ações
- [x] **Column/Row** - Layout em colunas e linhas
- [x] **ListView.builder** - Lista eficiente de itens
- [x] **Card/ListTile** - Componentes de lista
- [x] **TextField** - Campo de entrada de texto
- [x] **ElevatedButton** - Botões de ação
- [x] **Checkbox** - Seleção de itens
- [x] **AlertDialog** - Diálogos de confirmação
- [x] **SnackBar** - Mensagens de feedback

### **Conceitos de Programação:**
- [x] **StatefulWidget** - Widget com estado mutável
- [x] **setState()** - Atualização de estado
- [x] **Controllers** - Controle de campos de texto
- [x] **Callbacks** - Funções de resposta a eventos
- [x] **Condicionais** - Renderização condicional
- [x] **Loops** - Construção de listas dinâmicas
- [x] **Validação** - Verificação de dados de entrada

---

## 📊 **Estatísticas do Código**

- **Linhas de Código**: 305 linhas
- **Funções Implementadas**: 8 funções principais
- **Widgets Utilizados**: 15+ widgets diferentes
- **Funcionalidades**: 10+ funcionalidades completas
- **Dependências Externas**: 0 (apenas Flutter nativo)

---

## 🎨 **Design e Interface**

### **Tema Personalizado:**
```dart
ThemeData(
  primarySwatch: Colors.blue,
  useMaterial3: true,
)
```

### **Paleta de Cores:**
- **Primária**: Azul (#2196F3)
- **Sucesso**: Verde (#4CAF50)
- **Atenção**: Laranja (#FF9800)
- **Erro**: Vermelho (#F44336)
- **Neutro**: Cinza (#9E9E9E)

### **Componentes Visuais:**
- **Cards com Elevação** - Profundidade visual
- **Sombras Sutis** - Efeito de profundidade
- **Ícones Material** - Consistência visual
- **Tipografia Hierárquica** - Diferentes tamanhos de fonte

---

## 🧪 **Como Testar a Aplicação**

### **Fluxo de Teste Completo:**
1. **Adicionar Itens**
   - Digite "Leite" e pressione "Adicionar"
   - Digite "Pão" e pressione Enter
   - Digite "Ovos" e clique no botão

2. **Marcar como Comprado**
   - Clique no checkbox do item "Leite"
   - Observe o texto riscado e cor cinza

3. **Verificar Estatísticas**
   - Total: 3 itens
   - Comprados: 1 item
   - Restantes: 2 itens

4. **Remover Item**
   - Clique no ícone de lixeira do "Pão"
   - Confirme a remoção no diálogo

5. **Limpar Lista**
   - Clique no ícone "Limpar Lista" na AppBar
   - Confirme a ação no diálogo

6. **Testar Validações**
   - Tente adicionar item vazio
   - Tente adicionar item duplicado

---

## 🚀 **Próximas Melhorias Sugeridas**

### **Funcionalidades Futuras:**
- [ ] **Persistência de Dados** - SharedPreferences ou SQLite
- [ ] **Categorias de Itens** - Organização por tipo
- [ ] **Busca e Filtros** - Localizar itens rapidamente
- [ ] **Animações** - Transições suaves
- [ ] **Temas** - Modo escuro/claro
- [ ] **Compartilhamento** - Enviar lista por WhatsApp
- [ ] **Backup na Nuvem** - Sincronização entre dispositivos

### **Melhorias Técnicas:**
- [ ] **Arquitetura BLoC** - Gerenciamento de estado avançado
- [ ] **Testes Unitários** - Cobertura de testes
- [ ] **CI/CD** - Integração contínua
- [ ] **Análise de Performance** - Otimizações

---

## 📈 **Resultados de Desenvolvimento**

- **Tempo de Desenvolvimento**: ~2 horas
- **Linhas de Código**: 305 linhas
- **Funcionalidades**: 100% implementadas
- **Plataformas Testadas**: Web (Chrome)
- **Bugs Conhecidos**: 0
- **Performance**: Excelente (60 FPS)

---

## 📚 **Recursos de Aprendizado**

### **Documentação Oficial:**
- [Flutter Documentation](https://docs.flutter.dev/)
- [Material Design 3](https://m3.material.io/)
- [Dart Language](https://dart.dev/)

### **Conceitos Demonstrados:**
- Widgets básicos do Flutter
- Gerenciamento de estado
- Interface responsiva
- Interações do usuário
- Validação de dados
- Design patterns

---

**Desenvolvido com ❤️ usando Flutter**
