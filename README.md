# Challenge Next Education ONE | Conversor de Moedas CLI 💱

Um conversor de moedas simples e eficiente baseado em linha de comando (CLI), desenvolvido em Java. O projeto utiliza a [ExchangeRate-API](https://www.exchangerate-api.com/) para obter taxas de conversão em tempo real.

<p align="center">
  <img width="100" height="100" alt="Java Logo" src="https://github.com/user-attachments/assets/4d41d56a-e35b-4424-b883-6f65b83f0947" />
</p>

## 🚀 Funcionalidades (Features)

O programa permite realizar conversões entre as seguintes moedas:
- **BRL** (Real Brasileiro) 🇧🇷
- **USD** (Dólar Americano) 🇺🇸
- **EUR** (Euro) 🇪🇺

Opções de menu:
1. Real para Euro
2. Euro para Real
3. Dólar para Euro
4. Real para Dólar
5. Euro para Dólar
6. Dólar para Real

## 🖼️ Imagens do Projeto (Project Images)

### Menu Principal
<img width="300" height="300" alt="Menu do Conversor" src="https://github.com/user-attachments/assets/1f673538-6122-4401-b1de-01754c854d0a" />

### Demonstração de Conversão
<img width="360" height="300" alt="Exemplo de Conversão" src="https://github.com/user-attachments/assets/eba7f904-cf7b-4f8d-a1e3-7cc07a1948a0" />

## 🛠️ Tecnologias Utilizadas (Technologies)

- **Java**: Linguagem base.
- **Maven**: Gerenciamento de dependências.
- **Gson**: Biblioteca para conversão de JSON para objetos Java.
- **Java Dotenv**: Para gerenciar variáveis de ambiente de forma segura.

## 📋 Pré-requisitos (Prerequisites)

Antes de começar, você vai precisar ter instalado em sua máquina:
- [JDK](https://www.oracle.com/java/technologies/downloads/) (Recomendado 17 ou superior).
- [Maven](https://maven.apache.org/download.cgi).
- Uma chave de API da **ExchangeRate-API**.

## ⚙️ Configuração (Configuration)

Para proteger sua chave de API, o projeto utiliza um arquivo `.env`.

1. Na raiz da pasta do código (`conversor_moedas_`), crie um arquivo chamado `.env`.
2. Adicione sua chave de API no seguinte formato:
   ```env
   API_KEY=sua_chave_aqui
   ```

## 🏃 Como rodar (How to run)

1. Navegue até a pasta do projeto:
   ```bash
   cd conversor_moedas_
   ```
2. Compile o projeto com Maven:
   ```bash
   mvn clean install
   ```
3. Execute o programa:
   ```bash
   mvn exec:java -Dexec.mainClass="com.app.Main"
   ```

## 📂 Estrutura do Projeto (Project Structure)

- `Main.java`: Ponto de entrada (entry point) do programa.
- `Menu.java`: Gerencia a interface do usuário e validações.
- `Request_Https.java`: Faz as requisições (requests) para a API.
- `Conversion_json.java`: Converte a resposta JSON em objetos.
- `Conversor.java`: Modelo de dados (record) para a conversão.
- `Processador_Conversor.java`: Orquestra a lógica de conversão.

---
**Feito por:** Vinícius Feitosa de Souza Filho
