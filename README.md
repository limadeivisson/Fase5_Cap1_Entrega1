# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href="https://www.fiap.com.br/"><img src="assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Administração Paulista" width="40%"></a>
</p>

<br>

# FarmTech Solutions: Previsão de Rendimento Agrícola com Machine Learning

## Fase 5 – Capítulo 1  
Período: 09/09/2025 a 29/09/2025

## 👨‍🎓 Integrantes do Grupo 64:
- Deivisson Gonçalves Lima – RM565095 – [deivisson.engtele@gmail.com](mailto:deivisson.engtele@gmail.com)
- Omar Calil Abrão Mustafá Assem – RM561375 – [ocama12@gmail.com](mailto:ocama12@gmail.com)
- Paulo Henrique de Sousa – RM564262 – [pauloo.sousa16@outlook.com](mailto:pauloo.sousa16@outlook.com)
- Renan Danilo dos Santos Pereira – RM566175 – [renansantos4978@gmail.com](mailto:renansantos4978@gmail.com)

## 👩‍🏫 Professores:
### Tutor(a):
- Lucas Gomes Moreira  
### Coordenador(a):
- André Godoi Chiovato  

---

## 📜 Introdução

Nesta entrega, a FarmTech Solutions atua em uma fazenda de médio porte (200 hectares) para aplicar **Machine Learning** na análise de dados climáticos e agrícolas.  
O objetivo é prever o **rendimento da safra (Yield)** e identificar **tendências de produtividade** por meio de **clusterização**, de modo a apoiar a gestão agrícola com base em dados reais.

A base utilizada foi o arquivo `crop_yield.csv`, com as seguintes variáveis:  
- Cultura (Crop)  
- Precipitação (mm/dia)  
- Umidade específica a 2 metros (g/kg)  
- Umidade relativa a 2 metros (%)  
- Temperatura a 2 metros (°C)  
- Rendimento (t/ha)

---

## 🔧 Desenvolvimento

### 💡 Desafio
- Explorar e entender os dados fornecidos (EDA).  
- Aplicar **técnicas de clusterização** para identificar cenários de produtividade e possíveis outliers.  
- Construir **cinco modelos de regressão supervisionada** diferentes para prever o rendimento da safra.  
- Avaliar o desempenho por métricas como **RMSE, MAE e R²**.  
- Interpretar resultados, limitações e propor próximos passos.  

### 🧠 Soluções Aplicadas
- Bibliotecas: `pandas`, `numpy`, `seaborn`, `matplotlib`, `scikit-learn`.  
- **Clusterização**: K-Means (Elbow e Silhouette) e DBSCAN.  
- **Modelos preditivos**:
  - Regressão Linear
  - Árvore de Decisão
  - Random Forest
  - Gradient Boosting
  - SVR  
- **Validação**: Hold-out + Repeated K-Fold Cross-Validation.  
- **Interpretação**: Importância de variáveis e análise de resíduos.  

---

## 📊 Bases de Dados

As bases de dados utilizadas estão disponíveis na pasta `/data/` do repositório:

- `crop_yield.csv` – base principal fornecida pela FIAP  
- `base_auxiliar_1.csv` – (descrição breve)  
- `base_auxiliar_2.csv` – (descrição breve)  

Essas bases são utilizadas diretamente no notebook para permitir a reprodutibilidade completa do trabalho.

---

## 📈 Prints do Projeto

### 📊 Análise Exploratória
<p align="center">
  <img src="imagens/correlacao.png" alt="Heatmap de Correlação" width="600">
</p>
<p align="center">
  <img src="imagens/distribuicao_yield.png" alt="Distribuição do Yield" width="600">
</p>

### 📉 Clusterização
<p align="center">
  <img src="imagens/elbow.png" alt="Método Elbow" width="500">
  <img src="imagens/silhouette.png" alt="Silhouette Score" width="500">
</p>

### 🤖 Modelagem Preditiva
<p align="center">
  <img src="imagens/comparacao_modelos.png" alt="Comparação de Modelos" width="600">
  <img src="imagens/feature_importance.png" alt="Importância de Variáveis" width="600">
</p>

---

## 📂 Estrutura de Pastas

```
📁Fase5_Cap1/
├─ 📜DeivissonGoncalvesLima_RM565095_fase5_cap1.ipynb
├─ 📜README.md
├─ 📂data/
│   ├─ crop_yield.csv
│   ├─ base_auxiliar_1.csv
│   └─ base_auxiliar_2.csv
├─ 📂imagens/
│   ├─ correlacao.png
│   ├─ distribuicao_yield.png
│   ├─ elbow.png
│   ├─ silhouette.png
│   ├─ comparacao_modelos.png
│   └─ feature_importance.png
```

---

## 🎥 Demonstração em Vídeo
O vídeo demonstrando a solução (≤ 5 min) está disponível no YouTube em modo **não listado**:  
👉 [Acessar vídeo da entrega](https://youtube.com/...)  

*(Link será atualizado após upload.)*

---

## 📜 Licença
Este projeto foi desenvolvido exclusivamente para fins acadêmicos no contexto da disciplina de Inteligência Artificial da FIAP.  
Todos os direitos reservados aos autores mencionados.
