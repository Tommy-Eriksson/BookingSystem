<H1>YH utbildning systemintegratör</h1>
<a href="https://www.lernia.se/utbildning/yrkeshogskoleutbildning/systemintegrator/">Lernia systemintegratör</a>

<h2>Första uppgiften i den inledande kursen Java. </h2>


<h3>Hotellbokningssytem</h3>
<p>Ett hotell behöver ett mindre bokningssystem som kan checka in och ut gäster. Systemet skahålla reda på alla incheckadegäster, deras rumsnummeroch incheckningsdatum.</p> 
<p>Ett användargränssnitt måste först skapas som representeras av klassen UI som också innehållermain().</p> 
<p>Användargränssnittet skall kunna:</p>
<ul>
<li>Checka in personer</li>
<li>Checka ut personer</li>
<li>Skriva ut incheckade personer tillkonsolen</li>
<li>Skriva ut lediga rum till konsolen</li>
</ul>
<h4>Klasser och projektstruktur</h4>
<p>Programmet ska vara uppdelat i ett antal klasser:</p>
<ul>
<li>Person</li>
<li>Ticket</li>
<li>Hotel</li>
<li>UI</li>
</ul>
<h4>Person</h4>
<p>Klassen Person skall ha minsttvå privata instansvariabler för namn och ålder, men får gärna utökas med mer data.</p> 
<p>Klassen skall ha en argumentkonstruktor som tar emot minsttvå parametrar (namn och ålder).</p> 
<p>Ett Personobjekt kan skapas såhär:</p> 
<pre>Personp1 = newPerson("Lasse", 56);</pre>
<h4>Ticket</h4>
<p>Ticket innehållerminst fyrainstansvariabler:</p> 
<ul><li>privatePersonperson;</li>
<li>private int roomNr;</li>
<li>privatestringid;</li></ul>
<p>Samt ytterligare en variabler för datum, det kant.ex vara en sträng, eller färdiga typer som Date;</p>
https://docs.oracle.com/javase/8/docs/api/java/util/Date.html<p>En ticket kan skapas t.ex. såhär:</p> 
<pre>Ticketticket = newTicket(p,102);</pre>
<p>Och dess konstruktor kan delvis se ut såhär:</p>
<pre>publicTicket(Person p, introomNr){
  this.person = p;this.roomNr = roomNr; // din kod, generera unikt ID
  }</pre>
<p>I Tickets konstruktorskall ett unikt ID skapas som baseras på namn och ett slumpat nummer.Det skall också finnas en funktion som returnerar det unika ID</p>
<code>public string getUniqueId(){ returnid; }</code>
<h4>Hotel</h4>
<p>Klassen hotell kan lägga till och ta bort personer, skriva ut personer till konsolen, skriva ut lediga rum osv.</p> 
<p>Hotell måsteockså på något sätt vid en bokning kunna dela ut ett ledigt rumsnummer, detta kan förslagsvisgöras genom två arrayer, en vacantRoom array och en occupiedRoom array.</p> 
<h4>UI</h4>
<p>Klassen UI har ett Hotel-objekt som instansvariabel som sedermeraskallanvändasför att kopplaihop inmatningar från din meny.</p> 
<h4>Kravspec:</h4>
<ul><li>Variabler/funktionerskall ha meningsfulla namn</li>
<li>Använd rätt namnkonvention</li>
<li>Det behövs ingen felhantering, men är alltid positivt om det implementeras</li>
<li>Tydliga utskrifter i konsolen</li>
<li>Tydliga uppmaningar till inmatning i konsolen</li>
<li>Kommentera gärna kod, kolla javadoc, men är ingen nödvändighet</li>
</ul>
