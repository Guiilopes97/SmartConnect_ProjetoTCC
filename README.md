# 🚀 SmartConnect - Aplicativo Multi-Plataforma com .NET MAUI

![.NET MAUI](https://img.shields.io/badge/.NET%20MAUI-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-blue.svg?style=for-the-badge)

> Uma solução moderna e elegante para desenvolvimento cross-platform, construída com o poder do .NET MAUI

## 📋 Sobre o Projeto

O **SmartConnect** é uma aplicação multiplataforma desenvolvida como Trabalho de Conclusão de Curso (TCC), demonstrando as capacidades do framework .NET MAUI para criar aplicações nativas que rodam em diferentes sistemas operacionais a partir de um único código-fonte.

### ✨ Características Principais

- 📱 **Multi-Plataforma**: Um código, múltiplas plataformas (Android, iOS, Windows, macOS)
- ⚡ **Performance Nativa**: Aproveita os recursos nativos de cada plataforma
- 🎨 **Interface Moderna**: Design responsivo e intuitivo
- 🔧 **Arquitetura Limpa**: Código organizado e de fácil manutenção
- 🔒 **Seguro**: Implementação de boas práticas de segurança

## 🛠️ Tecnologias Utilizadas

- **.NET MAUI** - Framework principal para desenvolvimento multi-plataforma
- **C#** - Linguagem de programação
- **XAML** - Markup para construção de interfaces
- **MVVM Pattern** - Padrão de arquitetura Model-View-ViewModel

## 📋 Pré-requisitos

Antes de começar, certifique-se de ter instalado:

- [.NET 8.0 SDK](https://dotnet.microsoft.com/download) ou superior
- [Visual Studio 2022](https://visualstudio.microsoft.com/) (Windows/Mac) com workload ".NET Multi-platform App UI development"
  - OU [Visual Studio Code](https://code.visualstudio.com/) com extensões C# e .NET MAUI
- Para desenvolvimento Android: Android SDK (API Level 21 ou superior)
- Para desenvolvimento iOS/macOS: Xcode (apenas em macOS)

## 🚀 Como Executar

### 1. Clone o repositório

```bash
git clone https://github.com/Guiilopes97/SmartConnect_ProjetoTCC.git
cd ProjetoTCC
```

### 2. Restaure as dependências

```bash
dotnet restore
```

### 3. Execute o projeto

**Para Windows:**
```bash
dotnet build -t:Run -f net8.0-windows10.0.19041.0
```

**Para Android:**
```bash
dotnet build -t:Run -f net8.0-android
```

**Para iOS (requer macOS):**
```bash
dotnet build -t:Run -f net8.0-ios
```

**Para macOS:**
```bash
dotnet build -t:Run -f net8.0-maccatalyst
```

## 📁 Estrutura do Projeto

```
ProjetoTCC/
├── Models/              # Modelos de dados
├── Views/               # Páginas e interfaces XAML
├── ViewModels/          # Lógica de apresentação
├── Services/            # Serviços e APIs
├── Resources/           # Imagens, fontes, estilos
├── Platforms/           # Código específico de plataforma
│   ├── Android/
│   ├── iOS/
│   ├── Windows/
│   └── MacCatalyst/
└── App.xaml            # Configuração global do app
```

## 🧪 Executando Testes

```bash
dotnet test
```

## 📱 Plataformas Suportadas

| Plataforma | Versão Mínima | Status |
|-----------|---------------|--------|
| Android | 5.0 (API 21) | ✅ Suportado |
| iOS | 11.0 | ✅ Suportado |
| Windows | 10.0.17763.0 | ✅ Suportado |
| macOS | 10.15 | ✅ Suportado |

## 🤝 Como Contribuir

Contribuições são sempre bem-vindas! Para contribuir:

1. Faça um Fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/MinhaFeature`)
3. Commit suas mudanças (`git commit -m 'Adiciona nova feature'`)
4. Push para a branch (`git push origin feature/MinhaFeature`)
5. Abra um Pull Request

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
