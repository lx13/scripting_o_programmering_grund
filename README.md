# Scripting och Programmering grundkurs #

Här kan vi lägga upp gemensamma grejer. Observera att alla i LX13 då kan skriva 
och ändra filerna här. Tänk också på att alla kan se vad vi skriver här, d.v.s. 
alla i hela världen.


## Skapa egna repos ##

Det enklaste är om man skapar sin egen repo och gör allt sitt arbete där.
Sedan kan alla forka scripten och sen göra en pull request tillbaks.
För att skapa din egen repo på ditt egna konto klicka på "Create a new repo" 
till höger om Ert namn upp i högra hörnet på GitHub. Fyll i uppgifterna så som 
namn och beskrivning av repon (t.ex. scripts\_grund eller liknande). Därefter 
kan du på din dator skapa en katalog som du vill spara dina scripts in, t.ex. 
scripts\_grund. CD:a in i katalogen och ange följande kommandon för att initiera 
katalogen som en git repo och lägga till din GitHub repo som en remote.
Byt ut "dittnamn" mot ditt username på GitHub och scripts\_grund.git mot namnet
på din repo (observera att .git måste vara med).

Först och främst måste vi ange vårt namn och den e-post adress som ska 
associeras med dina commits (observera att ditt namn och e-post adress kommer 
att ses i alla loggar).

	git config --global user.name ”Ditt Namn”
	git config --global user.email ”dinepost@example.com”

Nu kan vi gå vidare till att initiera git repon.

	mkdir bash_grundkurs
	cd bash_grundkurs
	git init
	git add -A
	git commit -m "Första commiten"
	git remote add origin https://github.com/dittnamn/scripts_grund.git
	git push -u origin master

Alla dessa steg behövs bara första gången!

## Arbeta med ditt förråd ##

Nu när du börjar ändra på dina filer så kanske du vill se vilka ändringar du har
gjort - Detta kan du göra med hjälp av följande kommando:

	git diff
	
Detta gör att du ser exakt vilka ändringar som är gjorda till förrådet. För att
få en lite mer allmän översikt kan du använda dig av

	git status

som även ger lite exempel på kommandon som kan utnyttjas för att checka in,
eller ångra ändringarna.

## Pusha ändringar till befintlig repo ##

När du ändrat eller lagt till något till din repo på din dator och vill att de 
ska synas på GitHub behövs bara följande tre steg.

	git add -A
	git commit -m "En kommentar till commiten"
	git push

## Hjälp ##

Även git har bra manual-sidor - för att få hjälp med ett specifikt kommando
skriver man 

	man git-kommando
	
(notera bindestrecket medllan git och kommandot), så om man vill ha hjälp med 
exempelvis kommandot git add så är kommandot

	man git-add

## Allmänt om GitHub och våra arbeten ##

Det hade varit bra om alla (som vill och inte har hemlig identitet) hade velat 
ange sit riktiga namn i GitHub-inställningnarna för sitt konto. På så sätt vet 
Victor vem alla är, annars har han inte en aning om vem som är vem. Kanske bara 
förnamnet om man inte vill ange hela sitt namn?
