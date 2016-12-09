# Kaltura Embeds for AT-Internet Video Tracking
HTML est�tico que es capaz de reproducir un video de Kaltura y enviar datos de consumo de video a AT-Internet seg�n lo especificado en el Tagging Plan.

## Ejemplo de Uso
 [Ver embed](container.html)
 ```html
 <iframe 
	src="embed.min.html"
	data-siteid="577958"
	data-lang="ES"
	data-wid="106"
	data-uiconf="23448356"
	data-entry=""
	data-type=""
	data-name=""
	data-url=""
	width="640" 
	height="320" 
	allowfullscreen 
	webkitallowfullscreen 
	mozAllowFullScreen 
	frameborder="0">
</iframe>
```

### Par�metros que acepta el iframe

| Param       	| Mandatory  | Default Value 						| Description |
| ------------- |:----------:| -------------------------------------|:------------|
| data-siteid 	| No         | 577958         						| AT-Internet, define unos identificadores para diferenciar el site de DEV/PRE/PRO. A�adir el ID que corresponda al site donde se muestre el Iframe. |
| data-lang   	| No         | ES 							        | Idioma del v�deo actual, se pasa como flashvar al player Kaltura: **_closedCaptions.defaultLanguageKey_** |
| data-wid    	| No         | 106  					 	 		| Kaltura tambi�n define unos IDs para diferenciar los players de DEV/PRE/PRO. A�adir el ID que corresponda al site donde se muestre el Iframe. |
| data-uiconf 	| No         | 23448356 					        |             |
| data-entry  	| No         | 0_w2pfb6wl  					        |             |
| data-producer | No         | producer_name       					|             |
| data-type 	| No         | programme_type				        |             |
| data-name 	| No         | programme_name        				|             |
| data-url 		| No         | https://www.europarltv.europa.eu/es/	|             |
| data-debug	| No         | false         						|             |
