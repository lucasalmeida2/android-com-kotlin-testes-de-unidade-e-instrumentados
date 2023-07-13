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
│   │   │       ├── extensions      #Diretório que contém extensões de função Kotlin adicionais para facilitar tarefas comuns
│   │   │       ├── model           #Diretório que contém classes que representam modelos de dados, como objetos ou entidades
│   │   │       ├── preferences     #Diretório que contém classes relacionadas ao gerenciamento de preferências do aplicativo
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
│   │   │       ├── build.gradle(Project: Orgs)  #Diretório usado para configurar as dependências e as configurações gerais do projeto
│   │   │       ├── build.gradle(Module :app)    #Diretório usado para configurar as dependências e as configurações do aplicativo
```

## Ferramentas utilizadas para o desenvolvimento do aplicativo
- **Kotlin**, como linguagem de programação;
- **Android Studio**, é o ambiente de desenvolvimento integrado (IDE) oficial para o desenvolvimento de aplicativos Android
- **JDK**, foi utilizado para fornecer as ferramentas necessárias para compilar, depurar e executar o código Kotlin;
- **Xml**, foi utilizado para a criação de arquivos de marcação estruturada, como layouts de interface e configurações de recursos;
- **Room**, foi utilizado para fornecer uma camada de abstração sobre o banco de dados, facilitando a manipulação e persistência de dados no aplicativo;
- **Coil**, foi utilizado para facilitar o carregamento e exibição de imagens no aplicativo, oferecendo recursos avançados de cache e manipulação de imagens;


## Ferramentas utilizadas para a criação dos testes de unidade e instrumentados
- **Junit**, é um framework open-source, utilizado para escrever e executar testes de unidade automatizados;
- **Triple A**, o padrão AAA é uma maneira comum de escrever testes de unidade e deve possuir três etapas: Arrange (Preparar o teste), Act (Rodar o teste) e Assert (Verificar as asserções);
- **Mockk**, é uma biblioteca Kotlin que permite a criação de objetos simulados (mocks) para testes,facilitando a criação de testes mais robustos e isolados;
- **Kluent**, é uma biblioteca Kotlin que fornece uma sintaxe mais fluente e legível para asserções em testes;
- **Espresso**, é um framework de teste instrumentado para Android, projetado para testar a interface do usuário de um aplicativo;

## Como executar os testes? 

1- Abra o Android Studio e navegue até o diretório do projeto.

2- No painel esquerdo do Android Studio, clique na pasta "Java".

3- Abra a pasta Orgs(androidTest) para executar os testes instrumentados ou a pasta Orgs(test) para executar os testes de unidade.

4- Clique com o botão direito do mouse no arquivo de teste de unidade que deseja executar e selecione a opção "Run 'nome_do_teste'".

5- O Android Studio começará a executar o teste selecionado e exibirá os resultados no painel "Run" na parte inferior da janela.

<img width="994" alt="Como executar os testes " src="https://github.com/lucasalmeida2/android-com-kotlin-testes-de-unidade-e-instrumentados/assets/101592386/cda6009f-d7b3-49bc-ac43-3195c3214de3">
