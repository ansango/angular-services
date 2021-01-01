# PEC6_Ej3_respuestas_teoria.

Crea un documento de texto PEC6_Ej3_respuestas_teoria y responde a cada
uno de los siguientes puntos:

1. ¿Qué son los interceptores?
2. Analiza la siguiente cadena de operadores de RxJS, explica cada uno de los pasos que se están desarrollando y explica en qué caso usarías este código:
   
  ``` 
    this.wines$ = this.searchSubject
      .startWith(this.searchTerm)
      .debounceTime(300)
      .distinctUntilChanged()
      .merge(this.reloadProductsList)
      .switchMap((query) => 
    this.wineService.getWine(this.searchTerm));
  
  ```