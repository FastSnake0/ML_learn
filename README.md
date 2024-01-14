# ML_Learn
## LR 1
### Функции

Аналитическое решение
функция растригина:
- best x: 0 0
- best f(x): 0

Функция Стыбинского-Танга:
- best x: -2.9 -2.9
- best f(x): ~ (39 * 2)

![Функции](https://github.com/FastSnake0/ML_learn/blob/main/refs/funcs.png)

### GD

функция растригина:
- best x: 2.10159495e-09 -9.94958638e-01 
- best f(x): 9.94959057e-01

Функция Стыбинского-Танга:
- best x: 2.74680274   2.74680277
- best f(x): -50.05889331

![Обычный gd](https://github.com/FastSnake0/ML_learn/blob/main/refs/gd.png)

### Momentum GD

функция растригина:
- best x:  2.10159495e-09 -9.94958638e-01 
- best f(x): 9.94959057e-01

Функция Стыбинского-Танга:
- best x: -2.90353403   2.74680274
- best f(x): -64.19561236

![Обычный gd](https://github.com/FastSnake0/ML_learn/blob/main/refs/mgd.png)

### ADAM

функция растригина:
- best x: 5.75425118e-12 9.94958636e-01 
- best f(x): 9.94959057e-01

Функция Стыбинского-Танга:
- best x: -2.90353403  -2.903534  
- best f(x): -78.33233141

![Обычный gd](https://github.com/FastSnake0/ML_learn/blob/main/refs/adam.png)

## LR 2
### Алгоритмы
#### Differential Evolution:
Основан на идеях эволюционных стратегий. Использует популяцию векторов параметров и проводит операции мутации, кроссовера и селекции для поиска оптимальных параметров. Мутации производятся путем комбинирования различных индивидов в популяции.

#### Particle Swarm Optimization:
Моделирует поведение роя частиц в пространстве параметров. Каждая частица движется по пространству, обновляя свое положение в зависимости от своей лучшей позиции и лучшей позиции в рое. Таким образом, алгоритм старается найти оптимальное положение в пространстве параметров.

#### Self-Adaptive Differential Evolution:
Расширение Differential Evolution с механизмом автоматической настройки параметров мутации. Позволяет алгоритму самостоятельно адаптироваться к характеру задачи оптимизации в процессе выполнения.

### Таблица сравнений

Поколения: 100
Популяция: 15

Аналитическое решение
функция растригина:
- best x: 0 0
- best f(x): 0

Функция Стыбинского-Танга:
- best x: -2.9 -2.9
- best f(x): ~ (39 * 2)

Функция            | Алгоритм      | average MSE            | min MSE                | max MSE                | best y                 | worst y
-------------------| ------------- | ---------------------- | ---------------------- | ---------------------- | ---------------------- | -------------------
Растригина         | DE            | 3.4253546750433228e-12 | 2.3424227454860056e-15 | 1.787689519763457e-11  | 9.272582701669307e-13  | 7.0932699713921465e-09
Растригина         | PSO           | 8.778582741856919e-08  | 1.2054983156465441e-14 | 1.773907987077751e-11  | 4.781952611665474e-12  | 7.038586602448049e-09
Растригина         | SADE          | 1.943346231002873e-11  | 6.058458823101041e-15  | 1.3319527505567418e-11 | 2.4016344468691386e-12 | 5.2849742360194796e-09
Стыбинского-Танга  | DE            | 7.79889600333743e-12   | 3.524832656953125e-13  | 1.2954148578278026e-11 | -78.33233140753056     | -78.3323314070879
Стыбинского-Танга  | PSO           | 4.10618517578064e-13   | 5.9580917312904986e-15 | 7.449475991710594e-13  | -78.33233140754264     | -78.3323314075187
Стыбинского-Танга  | SADE          | 1.29203838066989e-12   | 7.571447264790601e-16  | 2.400597859069286e-12  | -78.33233140754282     | -78.33233140745686
