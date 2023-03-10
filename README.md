# Pytania - Technologia Chmury Obliczeniowej

## Rozdział 1

### 1. Jakiego rodzaju chmura wymaga posiadania łącza internetowego i pozwala każdemu użytkownikowi korzystać z jej usług?

a) prywatna

b) hostowana

**c) publiczna**

<br />

**Wyjaśnienie:** 

***Chmura prywatna** — wszystkie zasoby są utrzymywane wewnętrznie we
własnym centrum danych.*

***Chmura hostowana** — coś pomiędzy chmurą prywatną a publiczną. Dostawca
usług tworzy w swoim centrum danych wydzielone, odizolowane środowisko
i oferuje je klientowi na jego wyłączny użytek.*

***Chmura publiczna** — dostawca usług oferuje usługę publiczną, czyli dostępną
dla każdego. Klienci są jednak w niej od siebie odizolowani.*

***Chmura hybrydowa** — połączenie chmury prywatnej i publicznej. Niektóre
usługi są dostępne w chmurze prywatnej, a inne w lokalnym centrum danych.
Co najmniej dwa tego rodzaju środowiska są ze sobą bezpośrednio połączone.*

<br/>

### 2. Jaki model usług daje największą kontrolę nad zasobami?

**a) IaaS**

b) PaaS

c) SaaS

<br />

**Wyjaśnienie:** 

***IaaS** -  Infrastructure as a Service*

***PaaS** -  Platform as a Service*

***SaaS** -  Software as a Service*

![IaaS SaaS PaaS](./IaaSPaaSSaaS.png "IaaS SaaS PaaS")

<br />

### 3. W jakim modelu usług zarządzanie infrastrukturą jest najprostsze?

a) IaaS

b) PaaS

**c) SaaS**

<br />

**Wyjaśnienie:** 

***IaaS** -  Infrastructure as a Service*

***PaaS** -  Platform as a Service*

***SaaS** -  Software as a Service*

![IaaS SaaS PaaS](./IaaSPaaSSaaS.png "IaaS SaaS PaaS")

<br />

### 4. Jaki model usług oferuje najnowsze funkcjonalności i aktualizacje?

a) IaaS

**b) PaaS**

c) SaaS

<br />

**Wyjaśnienie:**

***SaaS** wymaga minimalnego zaangażowania, ale możliwości jej dostosowywania też są minimalne. Aby w niej coś zmienić, trzeba się kontaktować z dostawcą usługi, bo tylko on może wprowadzać modyfikacje.*

***PaaS** daje większą swobodę pod względem administrowania, utrzymywania i dostosowywania infrastruktury. Zazwyczaj jednak zmiany ograniczają się do określonych ustalonych opcji konfiguracyjnych, ale to i tak więcej niż w przypadku modelu SaaS.*

***IaaS** wymaga największego zaangażowania klienta w administrowanie infrastrukturą i jej utrzymanie, ale też oferuje największe możliwości konfiguracyjne. Klient ma kontrolę nad wszystkim, co znajduje się na poziomie systemu operacyjnego i wyżej (może wybierać różne przygotowane wcześniej obrazy systemów, a nawet tworzyć własne). Może wybierać funkcjonalności,
które zamierza konfigurować, zarządzać rolami użytkowników na serwerach i instalować na maszynach wirtualnych dowolne oprogramowanie.*

*Przy wyborze modelu kluczową kwestią jest uświadomienie sobie, jakie funkcjonalności są najbardziej dopasowane do potrzeb w danej sytuacji. Czasami, gdy produkt oferuje wszystko, co trzeba, najprostszym rozwiązaniem jest wybranie modelu SaaS. **Jeżeli niezbędne są najnowsze ustawienia i funkcjonalności, prawdopodobnie najlepszy będzie PaaS.** Jeżeli natomiast wymagane są nietypowe rozwiązania, wtedy właściwym wyborem będzie IaaS, ponieważ w tym modelu można skonfigurować i zainstalować wszystko, co jest potrzebne do uruchomienia aplikacji.*

<br />

### 5. Co decyduje o izolowaniu środowisk klientów w chmurze Azure?

**a) usługa Azure Fabric**

b) podmiot

c) subskrypcja

<br />

**Wyjaśnienie:**

*Microsoft jest publicznym dostawcą usług i przechowywane przezeń dane poszczególnych klientów muszą być od siebie odizolowane. Do tego celu wykorzystywana jest usługa **Azure Fabric**. Mimo że klienci używają tych samych fizycznych zasobów, takich jak sieć, serwery i macierze, usługi są dostępne tylko dla ich właścicieli.*

*Z perspektywy Microsoft Azure, gdy użytkownik zaloguje się do swojego konta, usługa **Azure Fabric** określa, do których podmiotów ma on dostęp, i łączy go z domyślnym podmiotem. Użytkownik uzyskuje wtedy dostęp do subskrypcji i zasobów przypisanych temu podmiotowi i może nimi zarządzać. Przełączając się pomiędzy podmiotami, użytkownik uzyskuje dostęp do innych subskrypcji i grup zasobów. Cały proces jest kontrolowany przez **Azure Fabric**, aby środowiska różnych klientów były od siebie odizolowane.*

<br />

### 6. Jak nazywa się pierwszy poziom dostępu w chmurze Microsoft Azure?

a) usługa Azure Fabric

**b) podmiot**

c) subskrypcja

<br />

**Wyjaśnienie:**

*Najwyższą jednostką administracyjną w chmurze Azure jest **podmiot**.*

<br />

### 7. Jaki jest najniższy poziom szczegółowości dostępu do zasobów?

**a) zasób**

b) grupa zasobów

c) subskrypcja

**Wyjaśnienie:**

*Wszystkie sposoby dostępne w chmurze Azure tworzą hierarchiczną strukturę. Zasoby należą do grup, grupy do subskrypcji, a subskrypcje do podmiotu.*

<br />

### 8. Jaki jest zalecany poziom szczegółowości dostępu do zasobów Azure?

a) zasób

**b) grupa zasobów**

c) subskrypcja

<br />

**Wyjaśnienie:**

*Z perspektywy Microsoft Azure, gdy użytkownik zaloguje się do swojego konta, usługa Azure Fabric określa, do których podmiotów ma on dostęp, i łączy go z domyślnym podmiotem. Użytkownik uzyskuje wtedy dostęp do subskrypcji i zasobów przypisanych temu podmiotowi i może nimi zarządzać. Przełączając się pomiędzy podmiotami, użytkownik uzyskuje dostęp do innych subskrypcji i grup zasobów. Cały proces jest kontrolowany przez Azure Fabric, aby środowiska różnych klientów były od siebie odizolowane.*

*Od chwili wprowadzenia modelu ARM zarządzanie jest o wiele łatwiejsze. W poprzednim modelu, ASM, wszystko wyglądało zupełnie inaczej. Użytkownik po zalogowaniu uzyskiwał dostęp do wszystkich subskrypcji skojarzonych z jego kontem. System Azure Active Directory nie był przypisany do określonego podmiotu, więc mogło ich być kilka. Zarządzanie zasobami było trudniejsze, ponieważ nie było grup zasobów. Separacja zasobów była możliwa tylko na poziomie subskrypcji.*

*W podobny hierarchiczny sposób można administrować zasobami. Użytkownik może posiadać różnego rodzaju uprawnienia dostępu do zasobów, na przykład jako właściciel, udziałowiec, odbiorca itp. Za pomocą ról i polityk można definiować niestandardowe uprawnienia. Role użytkowników mogą dotyczyć podmiotu, grupy zasobów lub pojedynczego zasobu. Zarządzanie uprawnieniami użytkowników na poziomie zasobów jest trudne i czasochłonne, dlatego nie jest zalecane.*

<br />

### 9. Jaki jest system naliczania opłat w chmurze Azure?

a) roczny

b) miesięczny

**c) minutowy**

<br />

**Wyjaśnienie:** 

*W chmurze Microsoft Azure stosowany jest minutowy system rozliczania. Jeżeli na przykład klient utworzy maszynę wirtualną i usunie ją po 12 dniach, 11 godzinach i 13 minutach, to opłata zostanie naliczona dokładnie za ten okres. W systemie rozliczeń godzinowych opłata zostałaby naliczona za 12 dni i 12 godzin, a w przypadku rozliczeń dziennych — za 13 dni.*

<br />

### 10. Częścią jakiego modelu są szablony ARM? 

**a) IaC**

b) IaaS

c) konfiguracja jako kod

<br /> 

**Wyjaśnienie:** 

*Dzięki modelowi ARM i szablonom Microsoft poszedł mocno do przodu i znacząco zmienił branżę chmurową. W chmurze i metodyce DevOps bardzo ważne jest pojęcie **IaC (ang. Infrastructure as Code — infrastruktura jako kod)**, a szablony idealnie się w nie wpisują. Za pomocą raz przygotowanego szablonu można powielać środowiska. Automatyzuje się w ten sposób proces wdrażania i konfigurowania infrastruktury, unikając przy tym błędów.*

<br /><br />

## Rozdział 2

### 1. Jaki model usług wykorzystuje sieć Azure?

a) IaaS

b) PaaS

**c) obie powyższe odpowiedzi są poprawne**

<br />

### 2. Co definiuje zakres adresów IP?

a) maska podsieci

**b) CIDR**

c) RIP

**Wyjaśnienie:** 

*Kolejnym parametrem jest przestrzeń adresowa definiująca liczbę dostępnych adresów IP. Wykorzystywany jest tu format CIDR (ang. Classless Interdomain Routing — bezklasowe trasowanie międzydomenowe).*

<br />

### 3. Jakie usługi są dołączane do sieci wirtualnej za pomocą punktów końcowych?

a) maszyny wirtualne

**b) PaaS**

c) SaaS

<br />

**Wyjaśnienie:** 

*Za pomocą listy Punkty końcowe usługi możesz z podsiecią skojarzyć usługi PaaS.*

<br />

### 4. Domyślnym serwerem DNS w chmurze Azure jest:

**a) serwer Azure DNS**

b) publiczny serwer DNS

c) niestandardowy serwer DNS

<br />

**Wyjaśnienie:** 

*Opcja Serwery DNS umożliwia tworzenie własnych usług DNS w sieci wirtualnej. Jak już wspomniałem, domyślnie stosowana jest usługa oferowana przez Azure, ale można zdefiniować własną, wykorzystując maszynę wirtualną lub publiczny serwer.*

<br />

### 5. Kiedy można tworzyć punkty usług?

a) podczas tworzenia sieci wirtualnej

b) po utworzeniu sieci wirtualnej

**c) w dowolnym momencie**

<br />

### 6. Prywatny adres IP w sieci Azure jest:

a) dynamiczny

b) statyczny

**c) dynamiczny lub statyczny**

<br />

**Wyjaśnienie:**

*Ustawienia publicznego adresu IP są podobne do adresu prywatnego. **Domyślnie jest to adres dynamiczny**, który zmienia się po każdym uruchomieniu maszyny. **Można go zmienić na statyczny**, ale należy pamiętać o różnicy między adresem publicznym a prywatnym. Rezerwacja prywatnego adresu IP jest bezpłatna, ponieważ jest to adres wewnętrzny. Można więc bez obaw zarezerwować cały zakres adresów. Natomiast adres publiczny jest przydzielany z góry i nie można go zmienić na dowolny inny. Koszty rezerwacji pięciu pierwszych adresów publicznych są zawarte w cenie subskrypcji. Za każdy kolejny adres pobierana jest opłata. Nie jest ona wygórowana, bo wynosi ok. 3 euro miesięcznie, ale warto wiedzieć, za co się płaci.*

<br />

*7. Publiczny adres IP w sieci Azure jest:*

a) dynamiczny

b) statyczny

**c) dynamiczny lub statyczny**

<br />

**Wyjaśnienie:**

*Ustawienia publicznego adresu IP są podobne do adresu prywatnego. **Domyślnie jest to adres dynamiczny**, który zmienia się po każdym uruchomieniu maszyny. **Można go zmienić na statyczny**, ale należy pamiętać o różnicy między adresem publicznym a prywatnym. Rezerwacja prywatnego adresu IP jest bezpłatna, ponieważ jest to adres wewnętrzny. Można więc bez obaw zarezerwować cały zakres adresów. Natomiast adres publiczny jest przydzielany z góry i nie można go zmienić na dowolny inny. Koszty rezerwacji pięciu pierwszych adresów publicznych są zawarte w cenie subskrypcji. Za każdy kolejny adres pobierana jest opłata. Nie jest ona wygórowana, bo wynosi ok. 3 euro miesięcznie, ale warto wiedzieć, za co się płaci.*

<br />

### 8. Sieciowa grupa zabezpieczeń to:

**a) zbiór reguł bezpieczeństwa kontrolujących przepływ ruchu**

b) reguły rezerwacji adresów IP

c) obie powyższe odpowiedzi są poprawne

<br />

**Wyjaśnienie:**

*Sieciowa grupa zabezpieczeń jest to zestaw reguł bezpieczeństwa obowiązujących w sieci Azure. Jest to podstawowe narzędzie do kontrolowania komunikacji sieciowej pomiędzy zasobami. Grupy zabezpieczeń dotyczą dwóch rodzajów zasobów: podsieci i interfejsów. W pierwszym przypadku zabezpieczenia obejmują wszystkie urządzenia dołączone do wybranej podsieci, natomiast w drugim tylko jedno urządzenie posiadające dany interfejs.*

<br />

### 9. Co definiuje sieciowa grupa zabezpieczeń? 

a) reguły zabezpieczeń dla ruchu przychodzącego

b) reguły zabezpieczeń dla ruchu wychodzącego

**c) obie powyższe odpowiedzi są poprawne**

<br />

**Wyjaśnienie:** 

*W panelu ustawień sieciowej grupy zabezpieczeń widoczne są aktualnie zdefiniowane reguły dotyczące ruchu przychodzącego i wychodzącego.*

<br />

### 10. Do jakiego zasobu można przypisać sieciową grupę zabezpieczeń?*

**a) sieci wirtualnej**

b) interfejsu sieciowego

c) podsieci

<br />


## Rozdział 3


### 1. Jaka jest najstarsza dostępna wersja systemu operacyjnego Windows Server w chmurze Azure?

a) Windows Server 2003

**b) Windows Server 2008 R2 SP1**

c) Windows Server 2012 R2

<br />

**Wyjaśnienie:** 

*Dostępne są następujące wersje systemu Windows:*

*Windows Server 2019 Datacenter*

*Windows Server 2016 Datacenter,*

*Windows Server 2012 R2 Datacenter,*

*Windows Server 2012 Datacenter,*

*Windows Server 2008 R2,*

*Windows 10 Enterprise,*

*Windows 10 Pro,*

*Windows 8.1 Enterprise,*

*Windows 7.*


<br />

### 2. Jakie cechy ma maszyna wirtualna w podstawowej warstwie rozmiarów?

**a) niski wskaźnik IOPS**

b) równoważenie obciążenia

c) automatyczne skalowanie

<br />

**Wyjaśnienie:**

*Grupa podstawowa jest przeznaczona dla środowisk programistycznych i testowych. Maszyny podstawowe pod względem wydajności są podobne do standardowych, ale mają pewne ograniczenia, m.in. **niższe wskaźniki IOPS (ang. Input/Output Operations Per Second — liczba operacji wejścia/wyjścia na sekundę)** oraz brak możliwości równoważenia obciążenia i automatycznego skalowania.*

<br />

### 3. Jakie zastosowania ma maszyna wirtualna o niskim priorytecie?

a) usługi o wysokiej dostępności

**b) wsadowe przetwarzanie danych**

c) równoważenie obciążenia

<br />

**Wyjaśnienie:**

*Maszyny o niskim priorytecie są uruchamiane wtedy, gdy centrum danych Azure ma wolne zasoby. Ich cena jest niska, ale nie zawsze są dostępne, ponieważ zarezerwowane dla nich zasoby mogą być przydzielane maszynom o wyższych priorytetach. **Maszyny te są przeznaczone do wykonywania operacji wsadowych i doraźnych zadań.***

<br />

### 4. Opcja Rozmiar w widoku maszyny wirtualnej jest wykorzystywana do:

a) skalowania maszyny w górę

b) skalowania maszyny w dół

**c) oba powyższe**

<br />

**Wyjaśnienie:**

*Rozmiar maszyny określa liczba procesorów, wielkość pamięci i pojemność dysku.*

<br />

### 5. Element Runbook służy do:

a) wykonywania operacji utrzymaniowych

b) skalowania maszyny wirtualnej w górę i w dół

**c) oba powyższe**

<br />

**Wyjaśnienie:**

*Element Runbook wymaga posiadania konta Azure Automation i służy do wykonywania operacji według wcześniej zdefiniowanego planu lub do uruchamiania niestandardowych skryptów. Zdaniem większości administratorów elementy te są bardziej użyteczne niż aplikacje logiki, ponieważ umożliwiają wykonywanie dowolnych operacji za pomocą skryptów PowerShell. Według mnie oba narzędzia są bardzo przydatne, a elementy Runbook są preferowane dlatego, że interpreter PowerShell wykorzystuje się również do administrowania lokalną infrastrukturą.*

*W elemencie Runbook można wybrać źródło wbudowane lub źródło użytkownika. W drugim przypadku należy wybrać konto automatyzacji i niestandardowy element, którym może być dowolny skrypt obsługiwany przez maszynę wirtualną. We wbudowanym źródle dostępne są następujące opcje: **Restart VM, Stop VM, Scale Up VM, Scale Down VM i Remove VM (odpowiednio: uruchom ponownie, zatrzymaj, powiększ, pomniejsz i usuń maszynę).***

<br />

### 6. Moduł równoważenia obciążenia służy do:

**a) rozdzielania obciążenia pomiędzy maszyny wirtualne umieszczone w puli zaplecza**

b) izolowania ruchu sieciowego i zabezpieczania maszyny wirtualnej przez atakami

c) oba powyższe

<br />

**Wyjaśnienie:** 

*Moduł równoważenia obciążenia rozdziela ruch pomiędzy kilka maszyn umieszczonych w puli. Robi to bardzo szybko, minimalnie spowalniając ruch.*

<br />

*7. Efektem umieszczenia maszyn wirtualnych w tym samym zestawie dostępności jest:*

a) tworzenie maszyn w różnych centrach danych Azure

**b) tworzenie maszyn w różnych szafach**

c) tworzenie maszyn w tej samej szafie

<br />

### 8. Rozbudowa infrastruktury poprzez tworzenie dodatkowych maszyn wirtualnych nosi nazwę:

a) skalowania w górę

b) skalowania w dół

**c) powiększania**

<br />

*9. Powiększanie zestawu maszyn wirtualnych nosi nazwę:*

a) skalowania w pionie

**b) skalowania w poziomie**

c) skalowania ukośnego

<br />

**Wyjaśnienie:**

*"Problem ten nie istnieje w skalowaniu w poziomie. Definiując zestaw skalowania, nie trzeba zmieniać rozmiarów maszyn wirtualnych. Zamiast tego tworzy się dodatkowe instancje, a moduł równoważenia obciążenia zajmuje się ich optymalnym wykorzystaniem. Zestaw skalowania jest podobny do zestawu dostępności, ale różni się tym, że kolejne maszyny są uruchamiane na żądanie w zależności od obciążenia istniejących maszyn. Ponadto w zestawie dostępności maszyny są od siebie niezależne i awaria jednej z nich nie wpływa na działanie pozostałych. Natomiast w zestawie skalowania tworzone są kopie jednej maszyny podstawowej. Jeżeli zostanie ona uszkodzona, to problem rozprzestrzeni się na pozostałe maszyny w zestawie. Należy więc wyraźnie pokreślić, że zestaw skalowania nie jest tym samym co zestaw dostępności, a skalowanie w poziomie dotyczy obciążenia, a nie dostępności maszyn."*

<br />

*10. Do skalowania infrastruktury wykorzystuje się:*

a) strefę dostępności

b) zestaw dostępności

**c) zestaw skalowania**

<br />

**Wyjaśnienie:**

*"Problem ten nie istnieje w skalowaniu w poziomie. Definiując zestaw skalowania, nie trzeba zmieniać rozmiarów maszyn wirtualnych. Zamiast tego tworzy się dodatkowe instancje, a moduł równoważenia obciążenia zajmuje się ich optymalnym wykorzystaniem. Zestaw skalowania jest podobny do zestawu dostępności, ale różni się tym, że kolejne maszyny są uruchamiane na żądanie w zależności od obciążenia istniejących maszyn. Ponadto w zestawie dostępności maszyny są od siebie niezależne i awaria jednej z nich nie wpływa na działanie pozostałych. Natomiast w zestawie skalowania tworzone są kopie jednej maszyny podstawowej. Jeżeli zostanie ona uszkodzona, to problem rozprzestrzeni się na pozostałe maszyny w zestawie. Należy więc wyraźnie pokreślić, że zestaw skalowania nie jest tym samym co zestaw dostępności, a skalowanie w poziomie dotyczy obciążenia, a nie dostępności maszyn."*

<br /><br />


## Rozdział 4

### 1. Usługa aplikacji w chmurze Azure to przykład modelu:

a) IaaS

**b) PaaS**

c) SaaS

<br />

**Wyjaśnienie:** 

![IaaS SaaS PaaS](./IaaSPaaSSaaS.png "IaaS SaaS PaaS")

<br />

### 2. Jaką kontrolę nad aplikacją ma użytkownik w planie usługi aplikacji w porównaniu z wirtualną maszyną?

a) większą

**b) mniejszą**

c) taką samą

<br />

**Wyjaśnienie:** 

![IaaS SaaS PaaS](./IaaSPaaSSaaS.png "IaaS SaaS PaaS")

<br />

### 3. Jaki jest nakład pracy administracyjnej w planie usługi aplikacji w porównaniu z wirtualną maszyną? 

a) większy

**b) mniejszy**

c) taki sam

<br />

**Wyjaśnienie:** 

![IaaS SaaS PaaS](./IaaSPaaSSaaS.png "IaaS SaaS PaaS")

<br />

### 4. Plan usługi aplikacji stosuje się do udostępniania:

**a) aplikacji internetowych**

b) baz danych

c) obu usług

<br /> 

**Wyjaśnienie:**

*Aby udostępnić aplikację internetową w chmurze Azure, należy utworzyć plan usługi aplikacji, a następnie dodać do niego aplikację. Jeden plan, podobnie jak usługa IIS zainstalowana na serwerze, może obejmować kilka aplikacji. Plan usługi jest podobny do usługi IIS, ale pomiędzy nimi jest jedna istotna różnica: nad usługą IIS administrator ma pełną kontrolę, a w planie usługi ma do dyspozycji określone opcje konfiguracyjne. W zasadzie jest to różnica między modelami IaaS i PaaS.*

<br />

### 5. Miejsca wdrożenia aplikacji służą do:

**a) udostępniania różnych wersji aplikacji**

b) udostępniania aplikacji w różnych regionach

c) obsługiwania zwiększonego obciążenia

<br />

**Wyjaśnienie:**

*Bardzo ciekawa jest opcja Miejsca wdrożenia, za pomocą której można utworzyć kilka osobnych środowisk dla aplikacji. Dzięki temu można na przykład zmieniać wersje aplikacji.*

<br />

### 6. Wzrosty obciążenia obsługuje się w planie usługi aplikacji poprzez:

a) skalowanie aplikacji w pionie

**b) skalowanie aplikacji w poziomie**

c) uruchamianie zadań WebJob

<br />

### 7. Najlepszym narzędziem do monitorowania aplikacji internetowej w chmurze Azure jest:

a) Splunk

b) analiza dzienników

**c) usługa Application Insights**

<br />

**Wyjaśnienie:**

*W zakładce Monitorowanie zalecane jest włączenie usługi Application Insights (wgląd w aplikację), za pomocą której można monitorować wykorzystanie i wydajność aplikacji.*

<br />

### 8. Wysoką dostępność aplikacji internetowej uzyskuje się poprzez:

a) skalowanie aplikacji w pionie

b) skalowanie aplikacji w poziomie

**c) utworzenie menedżera ruchu**

<br />

**Wyjaśnienie:**

*Aby osiągnąć wysoką dostępność aplikacji, należy użyć kolejnej usługi: menedżera ruchu. Menedżer działa na poziomie usługi DNS, a jego zadaniem jest kierowanie odbieranych zapytań do odpowiednich punktów końcowych na podstawie zdefiniowanych reguł.*

<br />

### 9. Menedżer ruchu obsługuje:

a) punkty końcowe Azure

b) zewnętrzne punkty końcowe

**c) oba rodzaje**

<br />

### 10. Dedykowane, odizolowane środowisko aplikacji internetowej w chmurze Azure to:

a) plan usługi aplikacji

**b) środowisko ASE**

c) maszyna wirtualna

<br />

**Wyjaśnienie:**

*Jeżeli jednak wymagany jest limitowany dostęp, można utworzyć środowisko usługi aplikacji (ang. App Service Environment, ASE). Takie środowisko jest całkowicie odizolowane od innych usług i zapewnia dodatkową ochronę aplikacjom, które są poddawane bardzo dużemu obciążeniu, wymagają zabezpieczonego dostępu sieciowego i wykorzystują dużo pamięci.*

<br /><br />


## Rozdział 5

### 1. Bazy danych w chmurze Azure można tworzyć w modelu:

a) IaaS

b) PaaS

**c) w obu**

**Wyjaśnienie:**

*Serwer SQL Server można wdrożyć w chmurze Azure, wykorzystując IaaS lub PaaS. Baza danych w tym drugim modelu jest często określania mianem modelu DaaS.*

<br />

### 2. Maszyna wirtualna z serwerem SQL Server różni się od maszyny bez serwera:

**a) konfiguracją**

b) wielkością pamięci i liczbą rdzeni procesora

c) nazwą

<br />

### 3. Baza Azure SQL Database jest również określania mianem modelu:

**a) Database as a Service**

b) SQL as a Service

c) Data as a Service

<br />

### 4. Warstwę cenową bazy Azure SQL Database określa:

a) liczba jednostek DTU

b) liczba wirtualnych rdzeni procesora

**c) oba powyższe**

<br />

**Wyjaśnienie:**

*Ponieważ model oparty na jednostkach DTU okazał się zbyt skomplikowany dla użytkowników, Microsoft wprowadził inny model, oparty na wirtualnych rdzeniach procesorów*

<br />

### 5. Zapytania do bazy Azure SQL Database można wysyłać za pomocą:*

a) programu SQL Server Management Studio

b) edytora zapytań w portalu Azure

**c) obu narzędzi**

<br />

**Wyjaśnienie:**

*Pierwszą unikatową opcją w widoku bazy danych SQL jest Edytor zapytań (wersja zapoznawcza). Dzięki edytorowi nie jest potrzebny program SQL Server Management Studio, ponieważ za pomocą przeglądarki można wysyłać do bazy dowolne zapytania, jak również wykonywać inne operacje.*

<br />

### 6. Aby połączyć się z bazą Azure SQL Database, należy:*

**a) utworzyć regułę zapory zawierającą adres IP**

b) wskazać legalny adres IP w ustawieniach sieci wirtualnej

c) wskazać legalny adres IP w ustawieniach głównej bazy danych

<br />

**Wyjaśnienie:**

*Zarządzanie bazą Azure SQL Database należy zacząć od skonfigurowania zapory. Domyślnie z bazą mogą się łączyć jedynie usługi Azure. Aby baza mogła obsługiwać połączenia pochodzące od określonych adresów IP, należy skonfigurować regułę zapory*

<br />

### 7. Aby utworzyć replikę bazy Azure SQL Database, należy:*

a) utworzyć kopię bazy

b) wyeksportować bazę

**c) skonfigurować replikację geograficzną bazy**

<br />

**Wyjaśnienie:**

*Aby utworzyć wysokodostępną bazę danych, kliknij opcję **Replikacja geograficzna**. Pojawi się widok z mapą świata, na której będą zaznaczone centra danych, z których wszystkie można wykorzystać do replikowania bazy. Centra, w których znajdują się utworzone bazy, są wyróżnione kolorem niebieskim, a centra zalecane do replikacji — fioletowym. Widoczna jest też informacja o bazie podstawowej. Oto widok opcji Replikacja geograficzna (zobacz pierwszy rysunek na następnej stronie)*

<br />

### 8. Aby uzyskać wysoką dostępność bazy Azure SQL Database, należy:

**a) utworzyć grupę trybu failover**

b) utworzyć klaster trybu failover

c) użyć opcji Zawsze włączone

<br />

**Wyjaśnienie:**

*W razie awarii lub niedostępności bazy podstawowej trzeba ręcznie przestawić bazę zapasową w tryb odczytu i zapisu, jak również zastosować inny ciąg umożliwiający łączenie się z bazą. Rozwiązanie to nie zapewnia więc wysokiej dostępności. W tym celu trzeba wykonać dodatkową operację — **utworzyć grupę trybu failover**.*

<br />

### 9. Do maskowania kolumn danych w bazie Azure SQL Database wykorzystuje się:

a) przezroczyste szyfrowanie danych

**b) dynamiczne maskowanie danych**

c) klasyfikowanie danych

<br />

**Wyjaśnienie:**

*Opcja Dynamiczne maskowanie danych zawiera listę kolumn, których maskowanie jest zalecane. Można tu również zdefiniować własne reguły maskowania. Zwróć uwagę, że zabezpieczenie to nie dotyczy administratora. Można wskazać innych użytkowników, którzy będą wykluczeni z maskowania.*

<br />

### 10. Do wykrywania potencjalnych zagrożeń bazy danych stosuje się:

a) ocenę luk w zabezpieczeniach

**b) zaawansowaną ochronę przed zagrożeniami**

c) obie funkcjonalności

<br />

**Wyjaśnienie:**

*W funkcjonalnościach dostępnych w panelu Zaawansowana ochrona przed zagrożeniami wykorzystane są techniki uczenia maszynowego, które analizują działanie bazy i alarmują o odstępstwach od normy. Jeżeli na przykład logowanie do bazy zazwyczaj odbywa się w godzinach pracy i ktoś zaloguje się o innej porze, zostanie zgłoszony alarm.*

<br /><br />

## Rozdział 7

### 1. W niektórych sytuacjach chmura hybrydowa jest jedynym rozwiązaniem ze względu na:

a) obowiązujące przepisy

b) dokonane inwestycje

**c) obie powyższe odpowiedzi są poprawne**

<br />

**Wyjaśnienie:**

*W wielu organizacjach migracja całej infrastruktury do chmury nie wchodzi w grę, mimo że decydenci są świadomi korzyści wynikających z takiego kroku. Jest tak z kilku powodów. Na przykład trudno jest firmie zrezygnować z lokalnej infrastruktury, w którą zostały **zainwestowane znaczne środki**. Aby utworzyć lokalne centrum danych, trzeba było ponieść nakłady finansowe na odpowiednie pomieszczenie, sieć, serwery, macierze i oprogramowanie. Rezygnacja z tych zasobów i kolejne wydatki na usługi chmurowe nie mają żadnego uzasadnienia biznesowego.*

*Innym powodem są przepisy prawne, które nie pozwalają przenosić niektórych usług do chmury. Na przykład w niektórych krajach **nie wolno przechowywać danych osobowych obywateli poza granicami państwa**. Jeżeli centrum danych Azure znajduje się za granicą, przeniesienie danych nie jest możliwe i trzeba je przechowywać w lokalnej infrastrukturze*

<br />

### 2. Sieć lokalną z chmurą Azure można łączyć za pomocą:

a) połączenia typu lokacja – lokacja

b) usługi ExpressRoute

**c) obie powyższe odpowiedzi są poprawne**

<br />

**Wyjaśnienie:**

*Aby połączyć ze sobą infrastruktury lokalną i chmurową, należy skonfigurować połączenie między siecią lokalną a wirtualną siecią Azure. **Może to być połączenie typu punkt – lokacja lub lokacja – lokacja.** Pierwszy rodzaj pozwala łączyć się z siecią Azure za pomocą pojedynczego komputera, a więc stanowi raczej punkt dostępu do chmury. Dlatego nie jest to rzeczywista chmura hybrydowa.*

*Połączenie typu lokacja – lokacja można utworzyć na dwa sposoby: wykorzystując sieć VPN (ang. Virtual Private Network — wirtualna sieć prywatna) lub **usługę ExpressRoute**. Pierwsze rozwiązanie zapewnia szyfrowaną komunikację między dwiema sieciami. Usługa ExpressRoute idzie krok dalej i oferuje dedykowane połączenie pomiędzy sieciami lokalną a wirtualną. Takie połączenie jest bardziej stabilne, szybsze, wprowadza mniejsze opóźnienia i jest bezpieczniejsze. Jest to jednak płatna usługa oferowana przez operatora telekomunikacyjnego.*

<br />

### 3. Do utworzenia połączenia typu lokacja – lokacja potrzebna jest:

**a) brama sieci wirtualnej**

b) lokalna brama danych

c) obie powyższe odpowiedzi są poprawne

<br />

**Wyjaśnienie:**

*Aby utworzyć połączenie, należy przygotować dwa zasoby Azure: **bramy sieci wirtualnej i lokalnej**.*

<br />

### 4. Brama sieci lokalnej przechowuje konfigurację:

a) sieci wirtualnej

**b) sieci lokalnej**

c) obie powyższe odpowiedzi są poprawne

<br />

### 5. Czy z portalu Azure można pobrać konfigurację urządzenia VPN?

a) tak

**b) tak, ale tylko dla niektórych urządzeń**

c) nie

<br />

### 6. Jaki jest zalecany model wdrożenia połączenia równorzędnego?

**a) Resource Manager**

b) klasyczny

c) obie powyższe odpowiedzi są poprawne

<br />

**Wyjaśnienie:**

*Ustawienia komunikacji równorzędnej są dostępne w widoku sieci wirtualnej w opcji Komunikacje równorzędne. Po kliknięciu przycisku Dodaj należy podać nazwę komunikacji i wybrać model wdrożenia: **Resource Manager lub Klasyczny**. **Zalecany jest pierwszy model**, gdyż umożliwia podanie identyfikatora zasobu albo wybranie subskrypcji i sieci wirtualnej, z którą trzeba nawiązać komunikację.*

<br />

### 7. Aby móc zarządzać tożsamością użytkowników w chmurze hybrydowej, należy wdrożyć:

a) kontroler domeny w grupie odzyskiwania

**b) kontroler domeny w chmurze Azure**

c) grupę zawsze dostępnych maszyn

<br />

### 8. Lokalna brama danych może być używana:

a) ze wszystkimi usługami Azure

**b) z wybranymi usługami Azure**

c) z jedną usługą Azure

<br />

### 9. Azure Stack to:

**a) rozszerzenie chmury Azure na lokalne centrum danych**

b) rozszerzenie lokalnego centrum danych na chmurę Azure

c) rozszerzenie chmury Azure na inną chmurę publiczną

<br />

**Wyjaśnienie:**

*Azure Stack jest jedynym na rynku rozwiązaniem realizującym odwrotny scenariusz, czyli uruchamianie usług chmurowych w lokalnym środowisku. Dzięki temu IaaS i PaaS można stosować we własnej infrastrukturze. **Azure Stack w rzeczywistości rozszerza chmurę Azure na lokalne środowisko**.*

<br />

*10. Azure Stack oferuje modele:*

a) IaaS

b) PaaS

**c) obie powyższe odpowiedzi są poprawne**

<br />

**Wyjaśnienie:**

*Azure Stack jest jedynym na rynku rozwiązaniem realizującym odwrotny scenariusz, czyli uruchamianie usług chmurowych w lokalnym środowisku. **Dzięki temu IaaS i PaaS** można stosować we własnej infrastrukturze. Azure Stack w rzeczywistości rozszerza chmurę Azure na lokalne środowisko.*

<br /><br />

## Rozdział 8

### 1. Usługa Azure Active Directory znajduje się na szczycie hierarchii:

**a) podmiotu**

b) subskrypcji

c) grupy zasobów

<br />

### 2. Czy konto użytkownika może należeć do kilku podmiotów?

**a) tak**

b) nie

<br />

### 3. Czy usługę AAD można wykorzystywać wraz z kontami Microsoft Live?

**c) tak**

d) nie

<br />

### 4. Czy usługę AAD można synchronizować z usługą Windows Server AD?

**a) tak**

b) nie

<br />

### 5. W bezpłatnej warstwie usługi AAD można utworzyć:

a) 5000 obiektów

**b) 500 000 obiektów**

c) 5 000 000 obiektów

<br />

**Wyjaśnienie:**

*W tym rozdziale skupimy się na funkcjonalnościach oferowanych w bezpłatnej warstwie umożliwiającej tworzenie **maksymalnie 500 000 obiektów** katalogowych, zarządzanie użytkownikami i ich grupami, synchronizowanie katalogu z lokalnym kontrolerem oraz tworzenie podstawowych raportów bezpieczeństwa.*

<br />

### 6. Aby skonfigurować niestandardową domenę, należy:

a) podać dowolną nazwę domeny

**b) podać nazwę posiadanej domeny**

c) użyć sufiksu onmicrosoft.com

<br />

### 7. Do weryfikacji domeny niestandardowej wykorzystuje się:

a) rekord MX

b) rekord TXT

***c) jeden z powyższych***

d) oba powyższe

<br />

### 8. Mechanizm RBAC można wykorzystywać do przypisywania ról:

a) subskrypcjom

b) grupom zasobów

c) zasobom

**d) wszystkim powyższym**

<br />

### 9. Role można przypisywać:

a) użytkownikom

b) grupom użytkowników

**c) użytkownikom i grupom użytkowników**

<br />

### 10. Aby aplikacja mogła uwierzytelniać użytkowników za pomocą usługi AAD, należy:

**a) zarejestrować aplikację w usłudze AAD**

b) utworzyć grupę AAD w aplikacji

c) wykonać obie operacje
