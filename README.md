# test6
Words (to dot or not to dot)
В качестве обучающего я взял датасет, основанный на файле news.words. Файлы news2.words и speech.words послужили для создания
тестовых датасетов. В качестве параметров использовались паузы после слов и скорость произнесения. Была идея использовать скользящие для различения
разгона и замедления темпа от начала к концу предложения, но она себя не оправдала. Была использована логистическая регрессия.

Для обучения и проверки знаки препинания были
расставлены вручную. Файл news2.words отличался низким качеством, что вызвало затруднение даже при ручной расстановке. Несмотря на достаточно 
высокий accuracy, не везде где надо, расставлены точки, но я бы не взялся оценивать precision по этому примеру.
В файле speech.words визуально результат получился лучше. Хотя оценить его сложно с позиции того, стоят ли там на самом
деле восклицательные знаки (которые я учёл как точки), а может и правда точки или запятые.
