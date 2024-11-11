		Analiza opłat pasażerów Titanica

Opis projektu:

	Projekt dotyczy analizy opłat (Fare) zapłaconych przez pasażerów na statku Titanic, z wykorzystaniem różnych technik statystycznych. Analiza obejmuje m.in. rozkład 		opłat, ich zależność od liczby towarzyszy podróży (SibSp),a także badanie symetrii rozkładu oraz korelacji między zmiennymi. Celem jest lepsze zrozumienie danych i zależności 	między opłatami a innymi zmiennymi.

Kroki analizy:

	1.Wczytanie i przygotowanie danych:
        	>Dane są wczytywane z pliku CSV, a następnie przygotowywane do analizy.
        	>Analiza dotyczy głównie zmiennej Fare, która przedstawia opłatę zapłaconą przez pasażera.

    	2.Analiza rozkładu zmiennej Fare:
        	>Obliczono podstawowe statystyki, takie jak średnia, mediana, moda oraz kwartyle.
       		>Na podstawie wykresu pudełkowego zidentyfikowano wartości odstające oraz rozkład opłat.
        	>Wykorzystano standaryzację, aby znormalizować zmienną Fare i lepiej zobaczyć jej rozkład.

    	3.Asymetria rozkładu:
        	>Obliczono współczynnik skośności (asymetrii) dla zmiennej Fare, który wskazuje na prawoskośny rozkład danych.
        	>Stwierdzono, że większość pasażerów zapłaciła niższe opłaty, a tylko nieliczni – wysokie, co wpływa na rozkład i podnosi średnią.

    	4.Relacja między Fare a SibSp:
        	>Przeanalizowano zależność między opłatą (Fare) a liczbą towarzyszy (SibSp).
        	>Wykres punktowy nie wykazał wyraźnej zależności między tymi zmiennymi.
        	>Obliczono współczynnik korelacji Pearsona, który wyniósł 0,16, wskazując na brak silnej korelacji.

Wymagania:

    Python 3.x
    Biblioteki:
        	pandas – do pracy z danymi w formie tabelarycznej,
        	matplotlib – do tworzenia wykresów,
        	scipy.stats – do obliczania statystyk (np.współczynnika skośności),
        	sklearn.preprocessing – do skalowania zmiennych.

	Możesz zainstalować wymagane biblioteki za pomocą poniższego polecenia:
		>pip install pandas matplotlib scipy scikit-learn
Wnioski:

    	>Zmienna Fare jest asymetryczna z dużą liczbą niskich opłat i kilkoma wysokimi wartościami odstającymi.
    	>Standaryzacja zmniejszyła skalę, ale nie zmieniła rozkładu- opłaty pozostały asymetryczne z dużą liczbą wartości blisko 0 po standaryzacji oraz nielicznymi wartościami 	odstającymi.
    	>Nie wykazano istotnej korelacji między opłatami a liczbą towarzyszy na pokładzie.
	>Bardzo słaba dodatnia korelacja (współczynnik 0,16) może wskazywać, że pasażerowie podróżujący samotnie lub z jednym towarzyszem płacili nieco wyższe opłaty (możliwe, że częściej 	podróżowali w wyższych klasach), ale wpływ ten jest minimalny.
	>Wykres punktowy pokazuje, że pasażerowie podróżujący w większych grupach (wysokie wartości SibSp) zazwyczaj płacili niższe ceny, co może wynikać z preferencji dla biletów 				grupowych lub wyboru tańszych klas przez duże rodziny
Autor:

Projekt wykonany w ramach zadania analizy statystycznej danych z Titanica.

