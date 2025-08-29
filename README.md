# 📊 Global Equity Momentum (GEM) vs Buy & Hold – Analiza porównawcza

https://colab.research.google.com/drive/1UtOiyTeH1acO44K7jVBjXX8QA9zv6_pe#scrollTo=CQAIrU5z6FKv

To repozytorium zawiera kod i wyniki analizy strategii **Global Equity Momentum (GEM)**.  
Celem projektu jest porównanie wyników GEM z pasywnym podejściem *Buy & Hold* dla wybranych ETF-ów w latach **2008–2025**.

---

## 📖 O strategii GEM

Strategia **Global Equity Momentum (GEM)** opiera się na efekcie *momentum* – tendencji do kontynuacji trendów cenowych.  
Idea jest prosta:
1. Raz w miesiącu sprawdzamy **12-miesięczną stopę zwrotu** (momentum) wybranych indeksów akcji.
2. Jeżeli oba rynki (USA i rynki poza USA) są na plusie, inwestujemy w ten, który ma wyższe momentum.
3. Jeżeli momentum jest ujemne – zamiast akcji wybieramy bezpieczniejszy portfel obligacji krótkoterminowych (proxy: ETF na Treasury 1–3Y).

Strategia łączy globalną dywersyfikację z prostym zarządzaniem ryzykiem i zmniejsza obsunięcia kapitału w trudnych okresach rynkowych.  

---

## 🎯 Analizowane aktywa

Do badania wybrano następujące ETF-y (dane od 2013-01-02 do 2025-02-02):

- **SP500** – iShares Core S&P 500 ETF (rynek USA)  
- **ACWI ex US** – SPDR MSCI ACWI ex-US ETF (rynki rozwinięte poza USA)    
- **Treasury 7–10Y** – iShares 7-10 Year Treasury Bond ETF (obligacje średnioterminowe)  
- **Treasury 1–3Y** – iShares 1-3 Year Treasury Bond ETF (obligacje krótkoterminowe)  

💡 W analizie przyjęto regularne **miesięczne wpłaty po 100 USD**. Pomijamy koszty prowizji i podatków, ponieważ w praktyce można je ograniczyć dzięki kontom takim jak **IKE/IKZE** lub brokerom bez prowizji (np. **XTB**).  

---

## 📈 Wyniki symulacji

### Porównanie wartości portfeli
![Porównanie GEM vs Buy & Hold](results/gem_vs_bh.png)

Na wykresie widoczna jest wartość portfela GEM w porównaniu do portfeli typu *Buy & Hold*.  
Dodano również linię pokazującą sumę wpłaconego kapitału (100 USD miesięcznie).

---

### Metryki wydajności

| Strategia / ETF            | Total Return | Annualized Return | Max Drawdown | Sharpe Ratio |
|-----------------------------|--------------|------------------|--------------|--------------|
| **Strategia GEM**           | 1.098729     | 0.079267         | -0.194226    | 1.272518     |
| **SP500 Buy & Hold**        | 2.711462     | 0.135457         | -0.224668    | 1.330105     |

---

## 📝 Wnioski

- **S&P 500** w badanym okresie osiągnął najwyższe stopy zwrotu.  
- **Strategia GEM** zapewniała niższe obsunięcia kapitału i większą dywersyfikację, kosztem niższej stopy zwrotu.  
- W praktyce GEM może być ciekawą alternatywą dla bardziej konserwatywnych inwestorów, którzy chcą ograniczać ryzyko spadków przy zachowaniu potencjału wzrostu.  

---
