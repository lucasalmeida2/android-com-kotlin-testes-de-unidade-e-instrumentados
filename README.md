# Projeto android-com-kotlin

**O objetivo deste projeto é a criação do aplicativo "Orgs" com o foco na implementação de testes de unidade e intrumentados.**

## Testes de unidade e instrumentados

- **Os testes de unidade** no desenvolvimento de aplicativos Android referem-se à verificação do funcionamento individual de unidades de código, como classes, métodos ou funções, de forma isolada. Esses testes são escritos pelos desenvolvedores para garantir que cada unidade de código esteja operando corretamente e produzindo os resultados esperados.

- **Já os testes instrumentados**, também conhecidos como testes de integração, são realizados em um ambiente que simula o comportamento real do aplicativo em um dispositivo Android. Esses testes verificam a interação entre várias unidades de código, como classes, componentes ou módulos, e podem incluir testes de interface do usuário (UI). Os testes instrumentados são executados em um dispositivo ou emulador, permitindo que sejam avaliados aspectos como o fluxo de dados, a comunicação com serviços externos e o desempenho do aplicativo em um ambiente mais próximo do real.

## Arquitetura do Projeto
```
android-com-kotlin
├── manifests                       #Diretório que contém o arquivo de manifesto do Android
│   │   ├── AndroidManifest.xml     #Diretório que contém permissões, componentes e configurações do aplicativo
├── java                            #Diretório que contém o código-fonte Kotlin do projeto
│   │   ├── orgs
│   │   │       ├── database        #Diretório que contém classes relacionadas ao gerenciamento de banco de dados
│   │   │       ├── extensions
│   │   │       ├── model
│   │   │       ├── preferences
│   │   │       └── ui              #Diretório que contém classes responsáveis pela interface do usuário,como atividades, fragmentos,etc
│   │   ├── orgs(androidTest)       #Diretório que contém testes instrumentados (testes que são executados em um dispositivo)
│   │   │       └── ProdutosTelasTests
│   │   ├── orgs(test)              #Diretório que contém testes unitários
│   │   │       └── ProdutoRepositoryTests
│   │   │       └── ProdutosTelasTests
├── res                             #Diretório que contém recursos do aplicativo, como arquivos de layout, imagens, ícones, etc
│   │   │       ├── drawable        #Subdiretório que contém arquivos de imagem ou vetores usados para desenhar elementos visuais
│   │   │       ├── font            #Subdiretório que contém arquivos de fonte personalizados usados no aplicativo
│   │   │       ├── layout          #Subdiretório que contém arquivos XML que descrevem a estrutura e o design das interfaces do usuário
│   │   │       ├── menu            #Subdiretório que contém arquivos XML que descrevem menus usados no aplicativo
│   │   │       └── values          #Subdiretório que contém arquivos XML com valores constantes, como strings, cores, estilos, etc
├── Gradle Scripts                  #Diretório que contém scripts de configuração e construção do Gradle
│   │   │       ├── build.gradle(Project: Orgs)  #Diretório usado para configurar as dependências e as configurações gerais do projeto.
│   │   │       ├── build.gradle(Module :app)    #Diretório usado para configurar as dependências e as configurações do aplicativo
```
