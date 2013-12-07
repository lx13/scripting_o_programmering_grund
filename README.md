# Scripting och Programmering grundkurs #

Här kan vi lägga upp gemensamma grejer. Observera att alla i LX13 då kan skriva och ändra filerna här. Tänk också på att alla kan se vad vi skriver här, d.v.s. alla i hela världen.


## Skapa egna repos ##

Det enklaste är om man skapar sin egen repo och gör allt sitt arbete där.
Sedan kan alla forka scripten och sen göra en pull request tillbaks.
För att skapa din egen repo på ditt egna konto klicka på "Create a new repo" till höger om Ert namn upp i högra hörnet på GitHub. Fyll i uppgifterna så som namn och beskrivning av repon (t.ex. scripts\_grund eller liknande). Därefter kan du på din dator skapa en katalog som du vill spara dina scripts in, t.ex. scripts\_grund. CD:a in i katalogen och ange följande kommandon för att initiera katalogen som en git repo och lägga till din GitHub repo som en remote.
Byt ut "dittnamn" mot ditt username på GitHub och scripts\_grund.git mot namnet på din repo (observera att .git måste vara med).

Först och främst måste vi ange vårt namn och den e-post adress som ska associeras med dina commits (observera att ditt namn och e-post adress kommer att ses i alla loggar).

	git config --global user.name ”Ditt Namn”
	git config --global user.email ”dinepost@example.com”

Nu kan vi gå vidare till att initiera git repon.

	git init
	git add -A
	git commit -m "Första commiten"
	git remote add origin https://github.com/dittnamn/scripts_grund.git
	git push -u origin master

Alla dessa steg behövs bara första gången!

## Pusha ändringar till befintlig repo ##

När du ändrat eller lagt till något till din repo på din dator och vill att de ska synas på GitHub behövs bara följande tre steg.

	git add -A
	git commit -m "En kommentar till commiten"
	git push
