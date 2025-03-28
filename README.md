# 📞 Web Scraper de Telefones de Anúncios

Este projeto é um **web scraper** desenvolvido em **Python** para coletar telefones de anúncios da seção de automóveis do site [Django Anúncios](https://django-anuncios.solyd.com.br/automoveis/). O script utiliza **requests**, **BeautifulSoup** e **expressões regulares** para extrair os números de telefone e armazená-los em um arquivo `.csv`.

## 🚀 Tecnologias Utilizadas

```md
- **Python**
- **Requests** (Para fazer requisições HTTP)
- **BeautifulSoup** (Para fazer o parsing do HTML)
- **Regex (re)** (Para extrair números de telefone)
- **Threading** (Para melhorar a performance)
```

## 📂 Estrutura do Projeto

```bash
├── scraper.py  # Arquivo principal do scraper
├── telefones.csv  # Arquivo onde os telefones serão armazenados
├── README.md  # Documentação do projeto
```

## 🔧 Como Executar

### 1️⃣ Clonar o Repositório

```bash
git clone https://github.com/seu-usuario/nome-do-repositorio.git
cd nome-do-repositorio
```

### 2️⃣ Criar um Ambiente Virtual (Opcional, mas Recomendado)

```bash
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate  # Windows
```

### 3️⃣ Instalar as Dependências

```bash
pip install -r requirements.txt
```

### 4️⃣ Executar o Script

```bash
python scraper.py
```

## 📜 Funcionamento

1. O script faz uma requisição HTTP para a página principal de automóveis.
2. Ele extrai os links dos anúncios e os armazena em uma lista.
3. Para cada link, o script acessa a página do anúncio e procura por telefones na descrição.
4. Os telefones encontrados são armazenados no arquivo `telefones.csv`.
5. O processo é feito com **múltiplas threads** para melhorar o desempenho.

## 📝 Exemplo de Saída

O arquivo `telefones.csv` será preenchido com números no formato:

```csv
11987654321
21987654321
31987654321
```

## ⚠️ Aviso Legal

Este projeto é apenas para **fins educacionais**. Certifique-se de estar em conformidade com as **políticas do site** antes de realizar qualquer raspagem de dados.

## 📌 Autor

Desenvolvido por **Seu Nome**.

📧 Contato: [seu-email@email.com](mailto\:seu-email@email.com)

🔗 GitHub: [github.com/seu-usuario](https://github.com/seu-usuario)

## 🏷️ Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

