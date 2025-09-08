# lab5_professora

A implementacao atual e a que funciona melhor, embora nao use uma funcao void de barreira.

Eu testei dois tipos de barreiras diferentes, uma que contava o numero de threads menos o numero de thredds terminadas para saber quando desbloquear as threads(desbloqueia quando todas estiverem bloqueadas, ou seja, atingiu multiplo de 1000)

No outro caso a barreira2 aceitava um argumento dizendo se havia sido imprimido ou nao o valor e ajia de acordo, as threads de execucao invocavam a barreira com argumento 0 e a de log com argumento 1;

Ambos os casos aconteceu o problema de pular alguns multiplos e imprimir alguns numeros logo apos um multiplo, entao optei pelo codigo sem uma funcao especializada de barreira.

Finalmente, modifiquei ligeiramente a thread de log para parar de executar quando as outras forem finalizadas.
