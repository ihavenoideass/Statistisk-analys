
# Statistisk analys
Denna repository innehåller HTML-exporterade filer från mina statistiska analyser utförda i R Markdown. GitHub visar tyvärr endast HTML-koden för dessa filer direkt. För att se och interagera med filerna på ett korrekt sätt kan du använda nbviewer.

```shell
pip install yfinance
pip install requests


```

## Instruktioner

För att se filerna i interaktivt format, klicka på länkarna nedan. De öppnas via nbviewer, som renderar HTML-filerna korrekt

```shell
https://nbviewer.org/

https://nbviewer.org/github/ihavenoideass/Statistisk-analys/blob/main/Inferens/Klassificering_predektion/Klassificeringsstudie_H1N1_Flue.nb.html

https://nbviewer.org/github/ihavenoideass/Statistisk-analys/blob/main/Inferens/Bootstrapping/Bootstrapping_umut.html



```

## Varför nbviewer?
GitHub renderar inte HTML-exporter från notebooks interaktivt. nbviewer tillåter dig att se innehållet som det var tänkt att visas, inklusive interaktiva element som grafer och tabeller.

```shell

from api import API
api = API()
data = api.fetch_data()

```

## Hämtning av data via min api klass (Avanza)

```shell

from avanza_api import fetch_avanza_data
avanza_data = fetch_avanza_data()

```

## Rengörning av data

```shell

from datacleaner import DataCleaner
cleaner = DataCleaner()
cleaned_data = cleaner.clean_data(data)

```

## Nedsparning av data

```shell

from datasaver import DataSaver
saver = DataSaver()
saver.save_data(cleaned_data)

```
