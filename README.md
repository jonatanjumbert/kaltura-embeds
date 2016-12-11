# Kaltura Embeds for AT-Internet Video Tracking
HTML estático que es capaz de reproducir un video de Kaltura y enviar datos de consumo de video a AT-Internet según lo especificado en el Tagging Plan.

## Ejemplo de Uso
 ```html
 <iframe 
	src="{DOMAIN_URL}/embed.min.html"
	data-entry="0_nj1aswnx"
	data-siteid="577958"
	data-type="world"
	data-name="sakharov-prize-2016-two-yazidi-women-tell-the-world-their-story"
	data-url="https://www.europarltv.europa.eu/es/programme/world/sakharov-prize-2016-two-yazidi-women-tell-the-world-their-story/"
	width="640" 
	height="320" 
	allowfullscreen 
	webkitallowfullscreen 
	mozAllowFullScreen 
	frameborder="0">
</iframe>
```

### Parámetros que acepta el iframe

| Param       	| Mandatory  | Default Value 						| Description |
| ------------- |:----------:| -------------------------------------|:------------|
| data-lang   	| No         | EN 							        | Idioma del vídeo actual, se pasa como flashvar al player Kaltura: **_closedCaptions.defaultLanguageKey_** |
| data-url 		| No         | https://www.europarltv.europa.eu/home| URL actual del vídeo en la web. El logo personalizado del player enlazará a esta URL. Para ello se pasa como flashvar al player de Kaltura: **_logo.href_** |
| data-wid    	| No         | 102  					 	 		| Kaltura también define unos IDs para diferenciar los entornos de DEV/PRE/PRO. Añadir el ID que corresponda al site donde se muestre el Iframe. |
| data-uiconf 	| No         | 23448355 					        | ID del Player de Kaltura que mostrará el video. |
| data-entry  	| No         | 0_w2pfb6wl  					        | ID del vídeo de Kaltura a reproducir. |
| data-siteid 	| No         | 577958         						| AT-Internet, define unos identificadores para diferenciar el site de DEV/PRE/PRO. Añadir el ID que corresponda al site donde se muestre el Iframe. |
| data-producer | No         | producer_name       					| Dato que se enviará a AT-Internet. Nombre del productor del vídeo. |
| data-type 	| No         | programme_type				        | Dato que se enviará a AT-Internet. Corresponde a la categoría de la web del video actual. |
| data-name 	| No         | programme_name        				| Dato que se enviará a AT-Internet. Corresponde con el nombre del video actual (el que aparece en la URL) |
| data-debug	| No         | false         						| Si se activa a TRUE, se podrá ver los valores enviados a AT-Internet durante los eventos de play/pause/seek del player de Kaltura. |

### Testado con los siguientes navegadores

| Browser | Version | Operating System |
|---------|:-------:|:----------------:|
|Google Chrome| 54.0.2840.99 m | Windows 10 |
|Microsoft Edge | 38.14393.0.0 | Windows 10 |
|Internet Explorer 11 | 11.447.14393.0 | Windows 10 |