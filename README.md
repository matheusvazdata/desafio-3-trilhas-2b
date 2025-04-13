# 📊 Dashboard - Participantes do Programa Trilhas 2B

Este projeto tem como objetivo apresentar um painel interativo que analisa os dados dos participantes do programa **Trilhas Inova 2B**, com foco em:

- Perfil demográfico (idade, gênero, cor/raça)
- Escolaridade e situação profissional
- Acesso à tecnologia
- Motivações para participação
- Distribuição geográfica

## 🛠️ Tecnologias Utilizadas

- Python (ETL)
- Google Colab
- Pandas + Unidecode
- Google Looker Studio
- Big Query
- Google Sheets (como fonte de dados)

## 📁 Organização do Projeto

| Pasta / Arquivo | Descrição |
|-----------------|-----------|
| `notebooks/` | Notebook com o código de ETL (limpeza e transformação) |
| `looker/` | Imagens e link para o dashboard final |
| `data/` | Informações sobre a planilha usada como fonte |

## 🔄 Pipeline de Dados (ETL)

1. **Extract:** Planilha do Google Sheets com os dados brutos (copiada do desafio).
2. **Transform:**
   - Limpeza de colunas e normalização (`snake_case`, sem acentos)
   - Criação de campos úteis: `faixa_etaria`, `trilha_simplificada`, `tem_acesso`
   - Tratamento de exceções como "Programação de Jogos"
3. **Load:** Resultado enviado para a Big Query e depois consumido pelo Looker Studio.

## 🔗 Links úteis

- 📄 **[Planilha no Google Drive](https://docs.google.com/spreadsheets/d/13_p8nO5A3boUxYGNhPNmqH5thv6kuZIvaI6oLwPRCKk)**
- 📓 **[Notebook no Google Colab](https://colab.research.google.com/drive/1BKlTwg5i1KL7bYBKUFwGtUe8-WVpBijy?usp=sharing)**
- 📊 **[Dashboard no Looker Studio](https://lookerstudio.google.com/reporting/4f29a346-4608-41ba-bf1b-694195b9fce9)**

## ✅ Resultado

O dashboard apresenta uma análise completa e interativa, com filtros por município, gênero, trilha e faixa etária — permitindo uma leitura clara do perfil e das necessidades dos participantes.

## 📌 Autor

**Matheus Vaz**  
Estudante de Dados • Engenharia de Analytics em construção  
[Datacamp](https://www.datacamp.com/portfolio/matheusvazdata) • [LinkedIn](https://www.linkedin.com/in/matheusvazdata/)