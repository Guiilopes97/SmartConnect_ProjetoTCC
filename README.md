# 🎓 Portal do Aluno UNISANTA - Aplicativo Multi-Plataforma

![.NET MAUI](https://img.shields.io/badge/.NET%20MAUI-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white)
![XAML](https://img.shields.io/badge/XAML-0C54C2?style=for-the-badge&logo=xaml&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![iOS](https://img.shields.io/badge/iOS-000000?style=for-the-badge&logo=ios&logoColor=white)
![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)

> 📱 Aplicativo multi-plataforma desenvolvido como Trabalho de Conclusão de Curso, integrando Portal do Aluno e Dashboard de COVID-19 usando .NET MAUI

## 📋 Sobre o Projeto

O **Portal do Aluno UNISANTA** é um aplicativo mobile desenvolvido com **.NET MAUI** (Multi-platform App UI) que permite aos alunos acessarem o portal acadêmico da universidade e visualizarem dados atualizados sobre COVID-19 no Brasil. O projeto demonstra a capacidade de criar aplicações nativas para múltiplas plataformas a partir de um único código-base em C#.

### 🎯 Objetivo do TCC

Desenvolver uma aplicação mobile multiplataforma que demonstre:
- Integração com sistemas web existentes (WebView)
- Consumo de APIs REST externas
- Arquitetura MVVM (Model-View-ViewModel)
- Navegação entre páginas
- Verificação de conectividade
- Interface responsiva e moderna

## ✨ Funcionalidades

### 🏠 Página Principal (MainPage)
- ✅ Contador interativo com MVVM
- ✅ Animações de imagem (rotação e movimento)
- ✅ Menu de eventos com ActionSheet
- ✅ Verificação de conectividade com internet
- ✅ Navegação para outras páginas
- ✅ Exibição de informações dos desenvolvedores

### 📚 Portal do Aluno
- ✅ Acesso direto ao Portal UNISANTA via WebView
- ✅ Navegação completa dentro do portal
- ✅ Suporte a conteúdo misto (HTTP/HTTPS)

### 🦠 Dashboard COVID-19
- ✅ Exibição de casos confirmados no Brasil
- ✅ Estatísticas de óbitos
- ✅ Consumo de API REST em tempo real
- ✅ Interface visual intuitiva com cards
- ✅ Ícones representativos dos dados

### 🌐 Recursos Gerais
- ✅ Verificação de conectividade antes de acessar recursos online
- ✅ Alertas informativos ao usuário
- ✅ Suporte a temas claro/escuro
- ✅ Animações e transições suaves

## 🛠️ Tecnologias Utilizadas

### Framework e Linguagens
- **.NET 6.0**
- **.NET MAUI** - Framework multi-plataforma
- **C#** - Linguagem de programação
- **XAML** - Markup para interfaces

### Bibliotecas e Pacotes
```xml
<PackageReference Include="CommunityToolkit.Mvvm" Version="8.0.0" />
<PackageReference Include="Newtonsoft.Json" Version="13.0.2" />
```

### APIs Externas
- **[COVID-19 Brazil API](https://covid19-brazil-api.now.sh/)** - Dados sobre COVID-19
- **Portal UNISANTA** - Sistema acadêmico

### Arquitetura
- **MVVM Pattern** - Separação de responsabilidades
- **Dependency Injection** - Injeção de dependências
- **Observable Pattern** - Binding de dados
- **Command Pattern** - Comandos reutilizáveis

## 📋 Pré-requisitos

### Software Necessário

- **[Visual Studio 2022](https://visualstudio.microsoft.com/)** (Windows ou Mac)
  - Workload: ".NET Multi-platform App UI development"
- **[.NET 6.0 SDK](https://dotnet.microsoft.com/download/dotnet/6.0)** ou superior

### Para Desenvolvimento Android
- Android SDK (API Level 21 ou superior)
- Emulador Android ou dispositivo físico

### Para Desenvolvimento iOS (somente macOS)
- Xcode 14 ou superior
- Simulador iOS ou dispositivo físico

### Para Desenvolvimento Windows
- Windows 10 versão 1809 (build 17763) ou superior
- Windows App SDK

## 🚀 Como Executar o Projeto

### 1️⃣ Clone o repositório

```bash
git clone https://github.com/Guiilopes97/ProjetoTCC.git
cd ProjetoTCC
```

### 2️⃣ Abra o projeto

- Abra o arquivo `ProjetoTCC.sln` no Visual Studio 2022

### 3️⃣ Restaure os pacotes NuGet

```bash
dotnet restore
```

### 4️⃣ Selecione a plataforma alvo

No Visual Studio, escolha a plataforma desejada na barra de ferramentas:
- 🤖 Android Emulator
- 🍎 iOS Simulator (apenas em Mac)
- 🖥️ Windows Machine

### 5️⃣ Execute o projeto

Pressione **F5** ou clique em "Start Debugging"

## 📁 Estrutura do Projeto

```
ProjetoTCC/
├── 📂 Classes/
│   ├── CovidData.cs          # Modelo de dados COVID
│   └── DashboardService.cs   # Serviço de API
│
├── 📂 View/
│   ├── MainPage.xaml         # Página principal
│   ├── DetailPage.xaml       # Portal do aluno
│   └── CovidPage.xaml        # Dashboard COVID
│
├── 📂 ViewModel/
│   ├── MainViewModel.cs      # ViewModel principal
│   ├── DetailViewModel.cs    # ViewModel do portal
│   └── CovidViewModel.cs     # ViewModel COVID
│
├── 📂 Resources/
│   ├── Images/               # Imagens do app
│   ├── Styles/               # Estilos XAML
│   └── Fonts/                # Fontes customizadas
│
├── 📂 Platforms/
│   ├── Android/              # Código específico Android
│   ├── iOS/                  # Código específico iOS
│   ├── Windows/              # Código específico Windows
│   └── MacCatalyst/          # Código específico macOS
│
├── App.xaml                  # Configuração global
├── AppShell.xaml             # Shell de navegação
└── MauiProgram.cs            # Ponto de entrada
```

## 🎨 Capturas de Tela

### Página Principal
- Interface com logo da UNISANTA
- Botões de navegação
- Contador interativo
- Animações de imagem

### Portal do Aluno
- WebView integrado
- Acesso completo ao portal
- Navegação fluida

### Dashboard COVID-19
- Cards informativos
- Dados em tempo real
- Interface visual moderna

## 📱 Plataformas Suportadas

| Plataforma | Versão Mínima | Status | Testado |
|-----------|---------------|--------|---------|
| Android | 5.0 (API 21) | ✅ Suportado | ✅ Sim |
| iOS | 14.2 | ✅ Suportado | ⚠️ Parcial |
| Windows | 10 (build 17763) | ✅ Suportado | ✅ Sim |
| macOS | 10.15 (Catalina) | ✅ Suportado | ⚠️ Parcial |

## 🔧 Configuração e Customização

### Alterar a API de COVID

No arquivo `CovidPage.xaml.cs`, modifique a URL:

```csharp
CovidData data = await service.GetCovidData("SUA_URL_AQUI");
```

### Alterar o Portal do Aluno

No arquivo `DetailPage.xaml`, modifique o Source do WebView:

```xml
<WebView Source="SUA_URL_AQUI" />
```

### Personalizar Cores

Edite o arquivo `Resources/Styles/Colors.xaml`:

```xml
<Color x:Key="Primary">#512BD4</Color>
<Color x:Key="Secondary">#DFD8F7</Color>
```

## 📊 Arquitetura MVVM

O projeto utiliza o padrão MVVM com auxílio do **CommunityToolkit.Mvvm**:

```csharp
// ViewModel
[ObservableProperty]
int count;

[RelayCommand]
void IncrementCount()
{
    Count += 10;
}

// XAML
<Label Text="{Binding Count}" />
<Button Command="{Binding IncrementCountCommand}" />
```

## 🔌 Consumo de API REST

Exemplo de consumo da API COVID-19:

```csharp
HttpClient _client = new HttpClient();
var response = await _client.GetAsync(query);
if (response.IsSuccessStatusCode)
{
    var content = await response.Content.ReadAsStringAsync();
    data = JsonConvert.DeserializeObject<CovidData>(content);
}
```

## ✅ Funcionalidades Implementadas

- [x] Navegação entre páginas usando Shell
- [x] MVVM com CommunityToolkit
- [x] Injeção de dependências
- [x] Consumo de API REST
- [x] WebView para conteúdo externo
- [x] Verificação de conectividade
- [x] Animações XAML
- [x] ActionSheet e Alerts
- [x] Data Binding
- [x] Themes (Light/Dark)

## 👥 Equipe de Desenvolvimento

### Desenvolvedores

| RA | Nome | Papel |
|----|------|-------|
| 188648 | **Guilherme Lopes de Oliveira** | Desenvolvedor Principal |
| 185378 | Thiago Ikenaga Suzuki | Desenvolvedor |
| 190718 | Pedro Henrique de Jesus Barbosa | Desenvolvedor |
| 150184 | Ramon Fisher de Paula Conceição | Desenvolvedor |

### Instituição

**Universidade Santa Cecília (UNISANTA)**
- Curso: Sistemas de Informação
- Ano: 2020/2023

## 📚 Referências e Recursos

### Documentação Oficial
- [📖 .NET MAUI Documentation](https://learn.microsoft.com/dotnet/maui/)
- [📘 CommunityToolkit.Mvvm](https://learn.microsoft.com/dotnet/communitytoolkit/mvvm/)
- [📗 XAML Documentation](https://learn.microsoft.com/dotnet/desktop/xaml/)

### APIs Utilizadas
- [🦠 COVID-19 Brazil API](https://covid19-brazil-api.now.sh/)
- [🎓 Portal UNISANTA](https://portalaluno.unisanta.br/)

### Tutoriais e Cursos
- [Microsoft Learn - MAUI](https://learn.microsoft.com/training/paths/build-apps-with-dotnet-maui/)
- [.NET MAUI Workshop](https://github.com/dotnet-presentations/dotnet-maui-workshop)

## 📄 Licença

Este projeto foi desenvolvido para fins acadêmicos como Trabalho de Conclusão de Curso.

## 📞 Contato

**Guilherme Lopes de Oliveira**

- GitHub: [@Guiilopes97](https://github.com/Guiilopes97)
- LinkedIn: [Seu LinkedIn](https://linkedin.com/in/seu-perfil)
- Email: guilherme.lopes@exemplo.com

## 🙏 Agradecimentos

- 🎓 **UNISANTA** - Universidade Santa Cecília
- 👥 **Equipe** - Pela colaboração e dedicação

---

<div align="center">

⭐ **Se este projeto foi útil para você, considere dar uma estrela!**

**Desenvolvido com 💜 por alunos da UNISANTA**

![UNISANTA](https://img.shields.io/badge/UNISANTA-TCC%202023-blue?style=for-the-badge)

</div>
