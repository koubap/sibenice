7 - Šibenice

Naprogramujte známou hru Šibenice, kterou si s vámi zahraje váš vlastní počítač.

Program obsahuje zadané věty ve stringovém poli (podobně jako v úkolu Analýza věty). Při spuštění programu je vybrána jedna z těchto vět a její obsah se zakóduje prostřednictvím symbolu "-" za každé písmeno, které obsahuje.

Uživatel hádá písmeno, které program načte a projde si hádanou větu. Pokud věta písmeno obsahovala, budou tato písmena odkryta, což poslouží jako nápověda pro další hádání. Pokud ale uživatel neuhádne správně, začne se mu stavět osudná šibenice. Uživatel má tedy asi 5 životů, než je šibenice celá a bude viset. Uživatel vyhrál, pokud stihne uhádnout všechna písmena dříve, než mu bude dostavena šibenice.

Tip 1: Pomocné hlášky "Nenalezeno!" případně "Úspěch!" určitě vylepší pocit  ze hry. Hru programujte postupně, postupujte po částech asi takto:

jedna věta "natvrdo" a její zamaskování
načtení písmene od uživatele a jeho odmaskování
vyhodnocení špatných tref a "výstavba" šibenice
volba věty - buďto náhodně nebo si uživatel zvolí číslo ještě před začátkem hry
Tip 2: Pro určité zjednodušení je možno použít věty bez hacku a carek, písmena ve větě i vstup od uživatele vždy nejprve převést na malá písmená, to zjednoduší vzájemné porovnávání

Tip 3: Pro správný chod programu musí program znát aktuální stav hádané věty (-> proměnná) i původní větu (-> ještě jedna proměnná), aby měl s čím porovnávat přicházející písmena od uživatele.

Tip 4: Pro vykreslování šibenice je určitě potřeba využít nějaké vylepšené vykreslování. Použít můžete například víceřádkový výpis pomocí symbolu "@" před vypisovaným stringem takto (příkaz je odsazen normálně, ale všechny další řádky až do "); se zobrazí přesně tak, jak jsou v kódu včetně počátečního odsazení):

Console.WriteLine(@"

     ╔═════+
     ║              Q
     ║             \ /
     ║              #
     ║             / \  
     ║       
  .....................
  
");

Přiložené screenshoty jsou opět jen pro ilustraci, určitě dokážete program dotáhnout dál.


