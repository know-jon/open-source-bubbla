Alla paths just nu förväntar sig att de sparas i en folder som heter data och en som heter output, strukturen på dessa är endast för demo och ingen större tanke bakom.

Innan man kan börja bör man ladda ner currency dataset själv länk finns i preparing_data, den är då i csv och konverterades till excel genom importera csv för demo skull.

# 3 notebooks

Generate new file är till för att visa hur man kan läsa in en excel fil och sedan spara datan

Explore är lite hur man kan göra utforskande arbete runt data

preparing data bör användas för att kolla att currency är korrekt, installerar rätt dependencys och bibliotek och laddar ner de två iso dataset automatiskt. 

# För att köra

Jag har valt att köra jupyter notebook genom en container, så om man har podman eller docker bör den komma igång genom att bara köra docker-compose up.

Man kan även öppna ipynb filerna i vs code om man har rätt plugin som till exempel jupyter plugin, då måste man se till att python miljön man vill köra i finns tillgänglig. Sök efter guider eller videos på youtube.
https://code.visualstudio.com/docs/datascience/jupyter-notebooks