1. Rifare labels.json con annotazioni corrette per prev/next
2. Definire e implementare un metrica di distanza tra FlowchartRepresentation. Aggregazione di due metriche: 
   - Struttura: nodi e archi senza informazioni sullo specifico nodo e arco
   - Similarità: considerare le proprietà (e.g. category, text, ...) di nodi e archi
3. Dividere dataset object detection in val e test
    - Train: trainare Faster RCNN e CNN threshold => 80%
    - Val: validazione CNN e Faster RCNN => 10%
    - Test: pipeline finale => 10%
4. Pipeline threshold: 
    - Optuna per trovare la combinazione migliore delle threshold per ogni immagine di train, la quale rappresenta la GT
    - Allenare una CNN che predica le threshold GT
    - Usare la CNN per la fase di inferenza
5. Cercare i competitor (tra cui https://cmp.felk.cvut.cz/ftp/articles/bresler/Bresler-Phan-Prusa-Nakagawa-Hlavac-ICFHR-2014.pdf)
6. Tirare fuori i dati dai competitor




