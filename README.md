<p align="center">
  <img src="image/PZH_Basislogo.svg" width="50%">
</p>

## Inleiding

In het kader van het WOB/WOO hebben wij algoritmes ontwikkeld om persoonsgegevens te identificeren in documenten. Geïdentificeerd gegevens kunnen worden gebruikt om documenten te markeren en weg te lakken in Adobe Acrobat.
Het bestandstype van de documenten moet wel pdf zijn. Om documenten naar pdf te converteren kan de [PDF-conversion-tool](https://github.com/Provincie-Zuid-Holland/PDF-conversion-tool) gebruikt worden. 

De volgende persoonsgegevens kunnen worden herkend:
- Email adressen
- Straatnamen met huisnummers en postcodes
- Voor‐ en achternamen
- Geldbedragen
- KvK‐nummer, IBAN, BRS‐nummer, telefoonnummers
- Persoonlijk beleidsopvattingen (indicatie van waar het in de tekst zou kunnen zijn)

Twee Databricks notebooks zijn gebruikt om verschillende stappen te verrichten:
- Notebook1_ocr_tika.py: 
	- OCR (Optical Character Recognition) kan gedaan worden om afbeeldingen over te zetten naar tekst
	- parsen is gebruikt on tekst in pdf's te herkennen en deze op te slaan als .txt
- Notebook2_weglakken.py: in deze notebook worden op basis van verschillende regex (reguliere expressies) persoonsgegevens herkent. Een dictionary wordt gemaakt van alle herkent gegevens. Bestanden voor het markeren van de pdf documenten in Adobe Acrobat en voor het installeren van de juiste adobe settings worden ook gecreëerd.

## Contact
Voor meer informatie en toegang tot de code contact opnemen met vdwh@pzh.nl.

## Auteurs
- Joana Cardoso
- Michael de Winter
- Dennis van Muijen
