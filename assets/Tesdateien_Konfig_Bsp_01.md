## Konfigurationsbeispiele Testdateien

### Booklet-Xml

Mehrere Testhefte und Aufgaben außerhalb der Testlets:

```xml
<?xml version="1.0"?>
<Booklet xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xsi:noNamespaceSchemaLocation="https://raw.githubusercontent.com/iqb-berlin/testcenter-backend/master/definitions/vo_Booklet.xsd">
  
  <Metadata>
    <Id>booklet1</Id>
    <Label>Testheft 1</Label>
  </Metadata>

  <BookletConfig>
		<Config key="pagingMode">separate</Config>
		<Config key="unit_navibuttons">FULL</Config>
		<Config key="unit_menu">FULL</Config>
  </BookletConfig>

  <Units>
    
	<Unit id="Start" label="Begrüßung zur Testung"/>

    <Testlet id="MET1" label="Mein erstes Testlet">
      
      <Restrictions>
          <CodeToEnter code="Hase">Bitte gib das Freigabewort ein.</CodeToEnter>
          <TimeMax minutes="10"/>
      </Restrictions>
    
      <Unit id="MEA1" label="Aufgabe 1" labelshort="1"/>
	  <Unit id="MEA2" label="Aufgabe 2" labelshort="2"/>
	  <Unit id="MEA3" label="Aufgabe 3" labelshort="3"/>
	  
            
    </Testlet>
	
	<Unit id="Info1" label="Informationen zum Testlet 2"/>
	
	<Testlet id="MET2" label="Mein zweites Testlet">
      
      <Restrictions>
          <CodeToEnter code="Vogel">Bitte gib das Freigabewort ein.</CodeToEnter>
          <TimeMax minutes="5"/>
      </Restrictions>
    
      <Unit id="MEA4" label="Aufgabe 4" labelshort="4"/>
	  <Unit id="MEA5" label="Aufgabe 5" labelshort="5"/>
	  <Unit id="MEA6" label="Aufgabe 6" labelshort="6"/>
	  
            
    </Testlet>
	
	<Unit id="Ende" label="Verabschiedung"/>
	
  </Units>

</Booklet>
```

Die Unit-Navigationsleiste dazu würde so aussehen:

![Bsp1 Booklet Navileiste](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bsp1_Booklet_Navileiste_01.png)