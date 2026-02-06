<div align="center">
    <h1>Water Loss Prediction ML with Bayesian Optimization</h1>
    <p>
        <strong>Projeto de Pesquisa Científica - UDESC 2025</strong><br>
        <em>Evolução do modelo preditivo para perdas de água, introduzindo algoritmos de Boosting avançados e Otimização Bayesiana.</em>
    </p>
</div>

<br>

<h3>Contexto e Evolução</h3>
<p>
    Este repositório representa a segunda fase da minha pesquisa como bolsista de pesquisa na UDESC. Enquanto o projeto anterior estabeleceu uma base com Random Forest e Gradient Boosting, esta etapa foca na maximização da performance.
</p>
<p>
    O desafio de negócio permanece: mitigar o desperdício de 40% de água potável no Brasil. O objetivo técnico foi superar a barreira de 0.73 de R² atingida anteriormente, além de diminuir as métricas de erros.
</p>

<h3>Tecnológica & Novas Implementações</h3>
<p>
    Para elevar a precisão do modelo, expandi as bibliotecas focadas em alta performance:
</p>
<ul>
    <li> Linguagem Python 3.13</li>
    <li> Novos Algoritmos (Boosting): <br>
      - <code>XGBoost</code><br>
      - <code>LightGBM</code>)<br>
      - <code>CatBoost</code> (Melhor performance
    </li>
    <li><strong>AutoML & Otimização:</strong> <br>
        - <code>MLJAR</code> (Automated Machine Learning)<br>
        - <strong>Otimização Bayesiana</strong> (substituindo o GridSearch tradicional para ajuste fino de hiperparâmetros).
    </li>
</ul>

<h3>Resultados Comparativos</h3>
<p>
    Testamos 5 arquiteturas diferentes. O <strong>CatBoost</strong> demonstrou superioridade, atingindo o menor erro (RMSE) e a maior capacidade explicativa.
</p>

<table>
    <thead>
        <tr>
            <th>Modelo</th>
            <th>R² (Precisão)</th>
            <th>RMSE (Erro)</th>
            <th>MAPE (Erro %)</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Floresta Aleatória (Baseline)</td>
            <td>0.514</td>
            <td>7.29</td>
            <td>20.11%</td>
        </tr>
        <tr>
            <td>Gradient Boosting (Versão Anterior)</td>
            <td>0.716</td>
            <td>5.57</td>
            <td>13.14%</td>
        </tr>
        <tr>
            <td>XGBoost</td>
            <td>0.732</td>
            <td>5.41</td>
            <td>12.28%</td>
        </tr>
        <tr>
            <td><strong>CatBoost (Novo Vencedor) </strong></td>
            <td><strong>0.750</strong></td>
            <td><strong>5.23</strong></td>
            <td><strong>11.56%</strong></td>
        </tr>
    </tbody>
</table>


<h3> Insights</h3>
<p>
    A interpretação do modelo CatBoost confirmou hipóteses críticas para a gestão pública:
</p>
<ul>
    <li><strong>Fatores Operacionais são Decisivos:</strong> Variáveis como <em>Volume de Água Produzido</em> e <em>Índice de Hidrometração</em> têm peso muito superior a fatores econômicos.</li>
    <li><strong>Decisão Estratégica:</strong> Investir na eficiência da rede (infraestrutura) traz mais retorno na redução de perdas do que intervenções baseadas apenas no perfil econômico (PIB) da região.</li>
</ul>

<h3>Referências</h3>
<p>
    Projeto apresentado no <strong>35º Seminário de Iniciação Científica (SIC UDESC 2025)</strong>.<br>
    Autores: João Pedro Felicio Prudencio, Andreza Kalbusch, Daniel Veitex Prates, Elisa Henning.
</p>
