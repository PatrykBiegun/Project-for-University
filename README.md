# Project-for-University
Projekt na studia z wykorzystaniem html, css, php oraz frameworku "Amelia" 

Projekt "jezioro"

Logi do admina: biegun, biegun

Używałem do niego frameworku „Amelia” oraz „Medoo” do połączeń z bazą

Layout strony zrobiłem za pomocą programu nicepage, jest on responsywny na inne rozdzielczości 

Baza prezentuje się w następujący sposób, każdy użytkownik na początku ma role którą potem można zmienić w panelu administratora. Ryby stanowią osobną tabelę z której czerpię informacje do tabeli.

Sprzęt ma kategorie w osobnej tabeli która pozwala na używanie ich wielokrotnie na podstawie ID.
Role są 3: stały klient, użytkownik oraz administrator
Używałem Timestampów do zapisywania czasu, są o tyle przydatne że same zapisują się w konkretnych momentach więc nie trzeba tego uwzględniać w kodzie.
Stronicowanie wprowadziłem do tabeli „ryby” wyświetla się po 5 sztuk każdej chyba że używamy filtrowania po nazwie, wtedy wyświetlają się wszystkie 
Wynajmowanie sprzętu to rzecz która pozwala na zmianę rodzaju konta, jeżeli użytkownik wynajmie sprzęt za łączną sumę 300zł (sumy są przypisane do konta) staje się użytkownikiem stałym i otrzymuje zniżkę 10% na wszystko. 
Administrator ma możliwość tworzenia i edytowania kont, dodawania i edytowania ryb oraz może „zatwierdzić” to że klient wynajął sprzęt. Jeżeli klient sam będzie oddawał swoje rzeczy to wtedy suma będzie się zmniejszać, a jeżeli suma spanie poniżej 300zł to straci zniżkę. 
W Panelu administratora widać datę oraz ID ostatniej modyfikacji 
Oraz listę tego co kto wynajmuje 

Ajax pyta czy jesteśmy pewni kiedy chcemy usunąć lub wynająć jakiś sprzęt, oraz wyświetla tabele ze sprzętem 
Anulowanie swojej rezerwacji obciąża konto sumą wysokości 10% ceny wynajmowanego sprzętu, tak że nawet po przejściu na użytkownika stałego można stracić ten status.
