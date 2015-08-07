---
title       : Sequía Agrícola
subtitle    : Exámen de Calificación
author      : Francisco Zambrano Bigiarini
job         : Doctorando en Ingeniería Agrícola c/m en Recursos Hídricos
logo        : escudo_udec3.png
biglogo     : escudo_udec.png
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax, bootstrap, quiz]        # {mathjax, quiz, bootstrap}
ext_widgets : {rCharts: [libraries/nvd3]}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---.segue bg:grey

## 1.- Contexto

---

## Definición de Sequía

>- Es un fenómeno rastrero __(Gillette, 1950)__
>- La sequía es el desastre natural más complejo de identificar, analizar, monitorear y manejar **(Burton, Kates, & White, 1978, p. 240; Wilhite,1993)**.
>- Las diferentes variables hidrometeorológicas y factores socioeconómicos, así como la naturaleza estocástica de la demanda de agua, es un obstaculo para una definición precisa **(Mishra and Singh, 2010)**.
>- En una forma realista la definición de sequía debe ser para una región y aplicación (o impacto) específico __(Wilhite and Glantz, 1985)__.
>- _"The impracticality of a universal drought definition" **(Lloyd, 2014)**_

---

## Tipos de Sequía

<iframe src="diagram_type_drought.html" width=100% height=100% allowtransparency="true" style="background: #FFCCFF;"> </iframe>

---

## Investigaciones Relevantes

>1. Standarized Precipitation Index (SPI) (**Mckee, 1993**) *"The relationship of drought frecuency and duration to time scales"*
>2. Vegetation Condition Index (VCI) (**Kogan, 1990**) *"Remote sensing of weather impacts on vegetation in non-homogeneous areas"*
>3. Temperature Condition Index (TCI) (**Kogan, 1995**) *"Application of vegetation index and brightness temperature for drought detection"*
>4. Vegetation Health Index (VHI) (**Kogan, 1997**) *"Global drought watch from space"*
>5. Standarized Vegetation Index (SVI) (**Peters et al, 2002**) *"Drought Monitoring with NDVI-Based Standarized Vegetation Index"*
>6. Precipitation Condition Index (PCI) and Scaled Drought Condition Index (SDCI) (**Rhee et al, 2010**) *"Monitoring agricultural drought for arid and humid regions using multi-sensor remote sensing data"*
>7. Synthesized Drought Index (SDI) (**Du et al, 2013**) *"A comprehensive drought monitoring method integrating MODIS and TRMM data"*

---

## Investigaciones Relevantes

<script>
$("#foo ol").attr('start', 8)
</script>

>8. Standarized Precipitation Evapotranspiration Index (SPEI) (**Vicente-Serrano et al, 2010**) *"A Multiscalar Drought Index Sensitive to Global Warming: The Standardized Precipitation Evapotranspiration Index"*

---

## Indicadores de Sequía

<iframe src="diagram_clases_drought.html" width=100% height=100% allowtransparency="true" style="background: #FFCCFF;"> </iframe>

---

## Tipos de Indicadores (Forma de Cálculo)

>- __<span style="color: red"> Estandarizados </span>__
  - SPI
  - SPEI
  - SVI
  - Zratio
>- __<span style="color: red"> Escalados </span>__
  - VCI
  - TCI
  - PCI
>- __<span style="color: red"> Combinados </span>__
  - VHI
  - SDCI

---&twocol

## Índice Estandarizado de Precipitación (SPI)

*** =left

<img src="assets/fig/unnamed-chunk-1-1.png" title="plot of chunk unnamed-chunk-1" alt="plot of chunk unnamed-chunk-1" style="display: block; margin: auto;" />

*** =right

## Características

>1. Sólo utiliza precipitación
>2. Permite utilizar diferentes escalas de tiempo
>3. Comparable espacialmente

---

## SPI Estación UdeC Chillán, 1, 3, 6 , 12 meses

<iframe src="dygraphs_spi.html" width=100% height=100% allowtransparency="true"> </iframe>

--- 

## Índice de Condición de la Vegetación (VCI)

$$
VCI = \frac{NDVI-NDVI_{min}}{NDVI_{max}-NDVI_{min}}
$$

### Caracteristica ###

<q> "Separa la componente climática de la vegetacional"</q>

<style>
.dark q {
  color: white;
}
</style>

---

## Índice de Condición de la Vegetación (VCI)

<iframe src="dygraphs_vci.html" width=100% height=80% allowtransparency="true"> </iframe>

---.segue bg:grey

## 2.- Declaración del Problema 

---&twocol

## ¿Que hay en Chile?

*** =left

- La Dirección Meteorológica de Chile (DMC) realiza el calculo del SPI

<div style='text-align: center;'>
    <img width='500' src='./assets/img/ipe_dmc.png' />
</div>

*** =right

- Atlas de Sequía ALC (CAZALAC) (**Nuñez et al.,2011**)
  - Periodo de Retorno
  - Máxima precipitación esperada
  - Mínima precipitación esperada

<div style='text-align: center;'>
    <img width='300' src='./assets/img/atlas_sequia_cazalac.png' />
</div>

---

## ¿Que hay en Chile?

_ClimateDataLibrary (www.climatedatalibrary.cl/maproom)_

<div style='text-align: center;'>
    <img width='800' src='./assets/img/datalibrary_chile.png' />
</div>

---{.build}

## ¿Qué hace falta?

>1. Evaluación conjunta entre los déficit de precipitaciones y la respuesta de la vegetación.
>2. Evaluación de la sequía agrícola a diferentes escalas temporales y espaciales.
>3. Una mejor compresión de la sequía desde el punto de vista de la componente agrícola.

## ¿Qué se propone?

>- __"Evaluar multiples indicadores de sequía meteorológia y agrícola a diferentes escalas temporales y espaciales en la zona agrícola centro sur de Chile"__

---.segue bg:grey

## 3.- Avances de la Investigación

---&twocol

## Fuentes de información utilizada

*** =left

**Satelital**

>- MODIS
  - MOD13 (Vegetación)
  - MOD11 (T° Superficial de Suelo)
  - MCD12 (Cubierta Terrestre) 

>- TRMM
  - 3B42 versión 7

*** =right

**Puntual**

>- Datos de precipitación
  - Dirección Meteorológica de Chile (DGA)
  - Dirección General de Aguas (DGA)
  - Otras fuentes

---

## Herramientas de análisis de datos

__Software Libre "R"__

>- Packages
  - raster (análisis de datos raster) (**Hijmans, 2015**)
  - maptools (mapas) (**Bivand and Lewin-Koh, 2015**)
  - plyr (manejo de gran cantidad de datos) (**Wickham, 2011**)
  - ggplot2 (gráfica) (**Wickham, 2011**)
  - SPEI (indicadores de sequía) (**Begueria and Vicente-Serrano,2013**)
  - Slidify (presentaciónes) (**Vaidyanathan, 2012**)
  - Knitr (investigación reproducible) (**Xie, 2014**)

---

## Indicadores de sequía seleccionados

>- SPI (precipitación, estandarizada)
>- VCI (vegetación, escalado)
>- TCI (T° superficial de suelo, escalada)
>- VHI (VCI+TCI, combinado)
>- SVI (vegetación, estandarizado)
>- PCI (precipitación TRMM, escalado)
>- SDCI (VCI+TCI+PCI, combinado)

---

## Área de estudio evaluada

__Región del Bío-Bío__

<div style='text-align: center;'>
    <img width='550' src='./assets/img/landcover_type.png'/>
</div>

---.segue bg:grey

## 4.- Algunos resultados

---

## Índice VHI temporada agrícola (sept-abrl)

<iframe src="vhi_biobio.html" width=100% height=100% allowtransparency="true"> </iframe>

---

## Correlación entre SPI-3 (puntual) e indicadores satelitales


<div id = 'chart1' class = 'rChart nvd3'></div>
<script type='text/javascript'>
 $(document).ready(function(){
      drawchart1()
    });
    function drawchart1(){  
      var opts = {
 "dom": "chart1",
"width":    800,
"height":    400,
"x": "mes",
"y": "value",
"group": "variable",
"type": "multiBarChart",
"id": "chart1" 
},
        data = [
 {
 "mes": "September",
"index": "SPI-3",
"variable": "SVI",
"value": 0.1144776950508 
},
{
 "mes": "October",
"index": "SPI-3",
"variable": "SVI",
"value": 0.2522825838416 
},
{
 "mes": "November",
"index": "SPI-3",
"variable": "SVI",
"value": 0.4750338878325 
},
{
 "mes": "December",
"index": "SPI-3",
"variable": "SVI",
"value": 0.5707268692162 
},
{
 "mes": "January",
"index": "SPI-3",
"variable": "SVI",
"value": 0.5480258247467 
},
{
 "mes": "Febraury",
"index": "SPI-3",
"variable": "SVI",
"value": 0.3984448172491 
},
{
 "mes": "March",
"index": "SPI-3",
"variable": "SVI",
"value": 0.4712123449805 
},
{
 "mes": "April",
"index": "SPI-3",
"variable": "SVI",
"value": 0.6900331165987 
},
{
 "mes": "September",
"index": "SPI-3",
"variable": "VCI",
"value": 0.2079265934033 
},
{
 "mes": "October",
"index": "SPI-3",
"variable": "VCI",
"value": 0.3364787137643 
},
{
 "mes": "November",
"index": "SPI-3",
"variable": "VCI",
"value": 0.503376545968 
},
{
 "mes": "December",
"index": "SPI-3",
"variable": "VCI",
"value": 0.5318929432826 
},
{
 "mes": "January",
"index": "SPI-3",
"variable": "VCI",
"value": 0.5088176254527 
},
{
 "mes": "Febraury",
"index": "SPI-3",
"variable": "VCI",
"value": 0.4436775557382 
},
{
 "mes": "March",
"index": "SPI-3",
"variable": "VCI",
"value": 0.4813491595241 
},
{
 "mes": "April",
"index": "SPI-3",
"variable": "VCI",
"value": 0.6338229839099 
},
{
 "mes": "September",
"index": "SPI-3",
"variable": "TCI",
"value": 0.2873679539568 
},
{
 "mes": "October",
"index": "SPI-3",
"variable": "TCI",
"value": 0.466621634574 
},
{
 "mes": "November",
"index": "SPI-3",
"variable": "TCI",
"value": 0.5159388274422 
},
{
 "mes": "December",
"index": "SPI-3",
"variable": "TCI",
"value": 0.7622824063565 
},
{
 "mes": "January",
"index": "SPI-3",
"variable": "TCI",
"value": 0.5260461698232 
},
{
 "mes": "Febraury",
"index": "SPI-3",
"variable": "TCI",
"value": 0.3494515936061 
},
{
 "mes": "March",
"index": "SPI-3",
"variable": "TCI",
"value": 0.6099373844151 
},
{
 "mes": "April",
"index": "SPI-3",
"variable": "TCI",
"value": 0.5904021954506 
},
{
 "mes": "September",
"index": "SPI-3",
"variable": "VHI",
"value": 0.3158147137792 
},
{
 "mes": "October",
"index": "SPI-3",
"variable": "VHI",
"value": 0.4519204956903 
},
{
 "mes": "November",
"index": "SPI-3",
"variable": "VHI",
"value": 0.6072260498192 
},
{
 "mes": "December",
"index": "SPI-3",
"variable": "VHI",
"value": 0.7303409442764 
},
{
 "mes": "January",
"index": "SPI-3",
"variable": "VHI",
"value": 0.5681036927617 
},
{
 "mes": "Febraury",
"index": "SPI-3",
"variable": "VHI",
"value": 0.4421078936472 
},
{
 "mes": "March",
"index": "SPI-3",
"variable": "VHI",
"value": 0.6183688930249 
},
{
 "mes": "April",
"index": "SPI-3",
"variable": "VHI",
"value": 0.7223737915289 
},
{
 "mes": "September",
"index": "SPI-3",
"variable": "SDCI1",
"value": 0.1806508833062 
},
{
 "mes": "October",
"index": "SPI-3",
"variable": "SDCI1",
"value": 0.5212626233134 
},
{
 "mes": "November",
"index": "SPI-3",
"variable": "SDCI1",
"value": 0.6058970381357 
},
{
 "mes": "December",
"index": "SPI-3",
"variable": "SDCI1",
"value": 0.6925989426192 
},
{
 "mes": "January",
"index": "SPI-3",
"variable": "SDCI1",
"value": 0.4793930454543 
},
{
 "mes": "Febraury",
"index": "SPI-3",
"variable": "SDCI1",
"value": 0.6152611389656 
},
{
 "mes": "March",
"index": "SPI-3",
"variable": "SDCI1",
"value": 0.7500306698073 
},
{
 "mes": "April",
"index": "SPI-3",
"variable": "SDCI1",
"value": 0.7590192584743 
},
{
 "mes": "September",
"index": "SPI-3",
"variable": "SDCI3",
"value": 0.6390735458739 
},
{
 "mes": "October",
"index": "SPI-3",
"variable": "SDCI3",
"value": 0.6841193042483 
},
{
 "mes": "November",
"index": "SPI-3",
"variable": "SDCI3",
"value": 0.8000790726125 
},
{
 "mes": "December",
"index": "SPI-3",
"variable": "SDCI3",
"value": 0.8712692669557 
},
{
 "mes": "January",
"index": "SPI-3",
"variable": "SDCI3",
"value": 0.7021896203072 
},
{
 "mes": "Febraury",
"index": "SPI-3",
"variable": "SDCI3",
"value": 0.4971053565785 
},
{
 "mes": "March",
"index": "SPI-3",
"variable": "SDCI3",
"value": 0.5257792705726 
},
{
 "mes": "April",
"index": "SPI-3",
"variable": "SDCI3",
"value": 0.7243497932786 
},
{
 "mes": "September",
"index": "SPI-3",
"variable": "SDCI6",
"value": 0.4110654530772 
},
{
 "mes": "October",
"index": "SPI-3",
"variable": "SDCI6",
"value": 0.3640857671958 
},
{
 "mes": "November",
"index": "SPI-3",
"variable": "SDCI6",
"value": 0.6400569017056 
},
{
 "mes": "December",
"index": "SPI-3",
"variable": "SDCI6",
"value": 0.4545171974973 
},
{
 "mes": "January",
"index": "SPI-3",
"variable": "SDCI6",
"value": 0.5495916975228 
},
{
 "mes": "Febraury",
"index": "SPI-3",
"variable": "SDCI6",
"value": 0.3176426540036 
},
{
 "mes": "March",
"index": "SPI-3",
"variable": "SDCI6",
"value": 0.1429131843862 
},
{
 "mes": "April",
"index": "SPI-3",
"variable": "SDCI6",
"value": 0.3627947389138 
},
{
 "mes": "September",
"index": "SPI-3",
"variable": "TRMM1",
"value": 0.03293483251634 
},
{
 "mes": "October",
"index": "SPI-3",
"variable": "TRMM1",
"value": 0.4961599750408 
},
{
 "mes": "November",
"index": "SPI-3",
"variable": "TRMM1",
"value": 0.472246454024 
},
{
 "mes": "December",
"index": "SPI-3",
"variable": "TRMM1",
"value": 0.475152159562 
},
{
 "mes": "January",
"index": "SPI-3",
"variable": "TRMM1",
"value": 0.2543048467632 
},
{
 "mes": "Febraury",
"index": "SPI-3",
"variable": "TRMM1",
"value": 0.4809252195863 
},
{
 "mes": "March",
"index": "SPI-3",
"variable": "TRMM1",
"value": 0.5836243003779 
},
{
 "mes": "April",
"index": "SPI-3",
"variable": "TRMM1",
"value": 0.600210342871 
},
{
 "mes": "September",
"index": "SPI-3",
"variable": "TRMM3",
"value": 0.6270611564294 
},
{
 "mes": "October",
"index": "SPI-3",
"variable": "TRMM3",
"value": 0.6421594183896 
},
{
 "mes": "November",
"index": "SPI-3",
"variable": "TRMM3",
"value": 0.5536963661336 
},
{
 "mes": "December",
"index": "SPI-3",
"variable": "TRMM3",
"value": 0.6949073178329 
},
{
 "mes": "January",
"index": "SPI-3",
"variable": "TRMM3",
"value": 0.5198788925335 
},
{
 "mes": "Febraury",
"index": "SPI-3",
"variable": "TRMM3",
"value": 0.3241961639703 
},
{
 "mes": "March",
"index": "SPI-3",
"variable": "TRMM3",
"value": 0.2285188663149 
},
{
 "mes": "April",
"index": "SPI-3",
"variable": "TRMM3",
"value": 0.4494028813185 
},
{
 "mes": "September",
"index": "SPI-3",
"variable": "TRMM6",
"value": 0.3867682436659 
},
{
 "mes": "October",
"index": "SPI-3",
"variable": "TRMM6",
"value": 0.1225452470298 
},
{
 "mes": "November",
"index": "SPI-3",
"variable": "TRMM6",
"value": 0.4228259153693 
},
{
 "mes": "December",
"index": "SPI-3",
"variable": "TRMM6",
"value": -0.1488083695327 
},
{
 "mes": "January",
"index": "SPI-3",
"variable": "TRMM6",
"value": 0.322898715003 
},
{
 "mes": "Febraury",
"index": "SPI-3",
"variable": "TRMM6",
"value": -0.02218185762586 
},
{
 "mes": "March",
"index": "SPI-3",
"variable": "TRMM6",
"value": -0.4281395377902 
},
{
 "mes": "April",
"index": "SPI-3",
"variable": "TRMM6",
"value": -0.07959047756163 
} 
]
  
      if(!(opts.type==="pieChart" || opts.type==="sparklinePlus" || opts.type==="bulletChart")) {
        var data = d3.nest()
          .key(function(d){
            //return opts.group === undefined ? 'main' : d[opts.group]
            //instead of main would think a better default is opts.x
            return opts.group === undefined ? opts.y : d[opts.group];
          })
          .entries(data);
      }
      
      if (opts.disabled != undefined){
        data.map(function(d, i){
          d.disabled = opts.disabled[i]
        })
      }
      
      nv.addGraph(function() {
        var chart = nv.models[opts.type]()
          .width(opts.width)
          .height(opts.height)
          
        if (opts.type != "bulletChart"){
          chart
            .x(function(d) { return d[opts.x] })
            .y(function(d) { return d[opts.y] })
        }
          
         
        
          
        

        
        
        
      
       d3.select("#" + opts.id)
        .append('svg')
        .datum(data)
        .transition().duration(500)
        .call(chart);

       nv.utils.windowResize(chart.update);
       return chart;
      });
    };
</script>

---.segue bg:grey

## Gracias

