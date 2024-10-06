# QA engineer Alza
## Poznámky k úkolu na přijímací pohovor do Alzy.

Ke sdílení hlášení o chybách používám *verzovací kontrolní systém GitHub* kvůli jeho snadné dostupnosti. Očekávám, že ve firmě velikosti Alza.cz je v testovacím a QA oddělení využíván jeden z programů Jira, Asana, Sentry, apod., tzv. Buck tracking systems. Hlášení jsem napsala v češtině, protože zadání úlohy je rovněž v češtině. Nicméně v GitHub uvádím ze zvyku popisky v angličtině.

Dokument *README.md* by se hodil k uvedení **zadání úlohy**. Protože je ale můj GitHub účet veřejně dostupný a nejsem si jistá, jestli by autoři souhlasili s publikací zadání úkolu s ohledem na předpisy Alzy.cz a také s ohledem na použití zadání v budoucích výběrových řízeních, nečiním tak.

K zápisu chyb jsem použila **formulář**. Vyplněné formuláře jsou vhodné při řešení každé chyby zvlášť. Členové teamu vývojářů si tak mohou rozdělit řešení chyb nezávisle na dokončení řešení ostatních chyb. 
Ve formuláři hlášení o chybách jsem zahrnula **položky** podle svého nejlepšího úsudku. V závislosti na zvoleném přístupu k vývoji a aktualizaci produktu by se seznam lišil počtem a výběrem konktrétních položek.

Seznam chyb je seřazen podle jejich urgence.

Při vypracování úkolu jsem předpokládala, že pod termínem "pacient" je myšlena osoba ošetřovaná u doktora nezávisle na pohlaví ošetřovaného. Vyskytuje-li se popsaná chyba v závislosti na zaškrtnutí polí "Muž", "Žena", uvadím tuto závislost v hlášení o chybách.

### Upřesnění k položkám obsaženým ve formuláři:

Z pozice QA inženýrky jsem udala urgenci každé chyby. Priotitu řešení chyby jsem navrhla, ale počítám s tím, že konečnou prioritu zvolí teamleader vývojářského teamu podle domluvených pravidel v organizaci vývoje aplikace. **Urgenci** a **prioritu** řešení chyby jsem vybírala na *škálách*: 
+ urgence
   - blok - znemožňuje fungování aplikace
   - hlavní - nefunguje funkce požadovaná zákazníkem
   - normalní - nefunguje jiná než požadovaná funkce, která komplikuje využití aplikace
   - vedlejší - aplikace funguje bez řešení této chyby bez problémů, řešení této chyby je možné odložit
+ priorita
   - kritická - nutno vyřešit na prvním místě k zajištění fungování aplikace
   - urgentní - řešení této chyby náleduje po kritických chybách - zajistí základní požadavky obsažené v zadání funkcí aplikace
   - vysoká - řešení této chyby na třetím místě - zajistí pravděpodobně očekávanou funkčnost aplikace
   - nízká - řešení chyby na posledním místě - zajistí snazší praktické využití aplikace, ale i touto chybou aplikace funguje bez problému

Položky **"Vyřídí"** a **"Datum vyřešení"** jsou připraveny pro vyplnění členy teamu, kteří se řešení konkrétních chyb ujmou.

### Nejasnosti:

V zadání jsem se setkala s nejasností: "lékař může na recept přidávat léky ručně nebo z připraveného seznamu, kde jsou 
upřednostněny léky pacientem pravidelně užívané". Nejasnost spočívá ve způsobu upřednostnění léků pacientem pravidelně užívaných. **Chyba s ID: 7** se tohoto problému týká. Přepokládám, že hlášení o chybách není správné místo, kde navhovat způsob upřednostňování léků. Očekávám, že preference způsobu upřednostňování léků je nutné vyjednat se zákazníkem a zohlednit možnosti na základě použitých technologií. Možné řešení by bylo uvést v seznamu léků tučně názvy léků pacientem pravidelně užívané.

**Chyba ID 8** je praktický návrh na výběr léků na předpis ze seznamu. Stejně jako u chyby ID 7 nepovažuji hlášení o chybách za vhodné místo k navrhování řešení. Představuji si, že by mohl být umožněn výběr více názvů léků pomocí držení tlačíka "Shift" a současného klikání na názvy léků.

**Chyba ID 12**: Není mi jasné, jestli slovem "Celá" v zadání ve větě: "Celá karta pacienta lze exportovat do textového souboru" je myšleno kompletně vyplněná, tedy obsahující všechny povinné údaje. Jestli textový soubor má obsahovat všechny povinné údaje, má chyba urgenci hlavní, prioritu urgentní.