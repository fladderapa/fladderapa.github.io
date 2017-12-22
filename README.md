Jag använder mig av flex för att göra websidan responsiv. Jag har utgått mycket från 
att dela in sidan i 3 kolumner. Exempelvis när jag valde att visa teman och priser.
Jag tycker att det funkar bra i desktop och att det blir enkelt att bryta av när fönstret krymper.

Jag använder mig egentligen bara media queries vid ett tillfälle 
och det var för att lägga till värdet justify-content: center;
Anledningen till det var för att göra den kompatibel med internet explorer
och valet av breakpoint motiverades därefter. I övrigt kände jag inte att jag 
hade ett behov av att ändra något annat. 

Vad gäller den feedback jag fick så tyckte jag att mycket var possitivt och att det
egentligen inte fanns så mycket som krävde en förändring.

På feedbacken om html fick jag exempelvis:

		* Ja, jag har inte mycket att anmärka på. Snarare tvärtom, så är den lättläst och semantisk. Jag upptäckte själv att jag lagt header- och footer-taggarna utanför min egen body, så jag lärde mig något också. Så tack för det!

På css-delen stod det blandannat:

		* CSS:en är mycket minimalistisk, vilket gör den lättläst och snabbladdad.

		* Det enda jag kan anmärka på är att många element har stylats enbart genom sin element-tag, vilket kan krångla till det om man skulle fortsätta bygga ut sidan eftersom stylingen är såpass generell. Fördelen är dock att det blir lättläst, kortfattat och enhetligt, så det är en avvägning. 

		*För nuvarande utseende fungerar det bra, men selektorerna för t.ex. <span> och <ul> skulle kanske behöva göras mer specifika om sidan skulle byggas ut. 


Vad jag verkligen tog till mig var feedbacken jag fick gällande designen designen då jag märkte att 
det blev en skillnad på större skärmar än min 12-tummare.

		* Kortare textrader på desktop hade ökat läsbarheten. De är nu 173 tecken långa.
		* Smalare kontaktformulär.
		* Även en något smalare meny på desktop hade underlättat (Den sträcker sig nu över hela skärmen). 


Det gjorde att jag satte en class på navbaren och tilldelade den en max-width på 800px med margin: 0 auto;

		.navbar{
	 	 max-width: 800px;
	 	 margin: 0 auto;
		}

Jag gjorde en liknande ändring för mission-container som inehåller den inledande texten.

		.mission-container{
		  max-width: 800px;
		  margin: 0 auto;
		}


Samt även för contact-container som inehåller mina input-fält

		.contact-container{
		  max-width: 700px;
		  margin: 0 auto;
		}


		Jag har testat sidan med Internet explorer version 11,10, 9, 8. Edge. Chrome på Android. Ios på iphone. Och Chrome på datorn. Och i mina mått mätt funkar sidan på samtliga webbläsare.
