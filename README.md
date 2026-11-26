# Monitor-Motores-Python ⚙️

> Este é um sistema desenvolvido em python programado para fazer o monitoramento de motores, é um sistema básico que está na sua __*versão 1.0.0.*__ e pode ter futuras atualizações e melhorias de seu sistema, mas atualmente apresenta grande utilidade e praticidade em sua uso

### Primeira Parte 🖥️

> Nesta parte inicial é exibido as informações básicas do sistema e do monitoramento

Esse sitema exibe inicialemente o nome do sistema e a sua versão atual
logo abaixo é mostrado a **data** e **hora** da leitura exatamente como está abaixo:

```
================================================================
Monitoramento de Motores Industriais - v1.0.0
Data/Hora da leitura: 26/11/2026 12:25:08
================================================================
```

### Segunda Parte 🔢

> Nesta parte é apresentado os dados e é exibido na seguinte ordem:
1. Estado
2. Setor
3. Temperatura
4. Corrente
5. Vibração
6. RPM

- Antes das informações é mostrado o estado do motor se está (Normal, Critico, Atenção...);
- O setor é onde o motor que está sendo monitorado está;
- A temperatura é o valor em graus celcius que o motor se encontrar no horario da leitura;
- A corrente é o valor que está ligado o motor;
- Vibração é a quantidade em milimetros por segundos que está vibrando;
- RPM é a velocidade que este motor está operando;

Abaixo disto é mostrado o alerta de forma especifica indicando do que é e o valor (esse valor seria praticamento o porque está em alerta).

```
================================================================
[NORMAL ] MTR-01 (Estamparia) | Temp: 68.4 C | Corr: 14.2 A | Vib: 2.1 mm/s | RPM: 1750
[CRITICO] MTR-02 (Usinagem) | Temp: 84.7 C | Corr: 19.3 A | Vib: 5.2 mm/s | RPM: 1690
  -> Alerta: Superaquecimento (84.7 C)
  -> Alerta: Sobrecorrente (19.3 A)
  -> Alerta: Vibracao elevada (5.2 mm/s)
[ATENCAO] MTR-03 (Bobinagem) | Temp: 76.2 C | Corr: 17.8 A | Vib: 4.7 mm/s | RPM: 1520
  -> Alerta: Vibracao elevada (4.7 mm/s)
[NORMAL ] MTR-04 (Pintura) | Temp: 61.0 C | Corr: 11.5 A | Vib: 1.8 mm/s | RPM: 1780
----------------------------------------------------------------
```

### Final 🔧

> Na parte final é apresentado os calculos de média e um resumo seguindo a ordem:

1. Resumo de quantos motores foram monitorados
2. Temperatura média
3. Quantidade média de corrente
4. Potencia total
5. Maior temperatura registrada

```
----------------------------------------------------------------
Resumo: 4 motores | Temp. media: 72.58 C | Corr. media: 15.7 A | Potencia total: 31.5 kW |
Maior temp.: MTR-02
================================================================
```