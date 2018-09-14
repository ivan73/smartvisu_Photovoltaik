# xy_page.html

```html
<div class="block">
    <div class="set-2" data-role="collapsible-set" data-theme="c" data-content-theme="a" data-mini="true">
	    <div data-role="collapsible" data-collapsed="false">
            {% import   "widget_mypv.html" as pv  %}
    
            <h3>Photovoltaik</h3>
            
            {{ pv.visu_smal('pv_index', 'Photovoltaik') }}
            <a href="https://monitoring.solaredge.com" target="_blank">solaredge monitoring</a>


            <h3>Photovoltaik Messwerte</h3>

            Modul-Leistung: {{ basic.print('', 'Photovoltaik.Modul_Leistung', '%01,2f kW') }} <br>
            InverterAC-Leistung: {{ basic.print('', 'Photovoltaik.AC_Leistung', '%01,2f kW') }} <br>
            InverterDC-Leistung: {{ basic.print('', 'Photovoltaik.DC_Leistung', '%01,2f kW') }} <br>
            Netz: {{ basic.print('', 'Photovoltaik.Zaehler_Leistung.StatusText', 'text') }}  {{ basic.print('', 'Photovoltaik.Zaehler_Leistung', '%01,2f kW') }} <br>
            NetzSpannung: {{ basic.print('', 'Photovoltaik.Zaehler_Spannung', '%01,2f V') }}<br>
            NetzStrom: {{ basic.print('', 'Photovoltaik.Zaehler_Strom', '%01,2f A') }}<br>
            NetzFrequenz: {{ basic.print('', 'Photovoltaik.Zaehler_Frequenz', '%01,2f Hz') }}<br>
            Speicher {{ basic.print('', 'Photovoltaik.Speicher_Status.Text', 'text') }}  {{ basic.print('', 'Photovoltaik.Speicher_Leistung', '%01,2f kW') }} <br>
            Speicher-Ladestand {{ basic.print('', 'Photovoltaik.Speicher_SOE', '%') }} <br>
            Verbrauch: {{ basic.print('', 'Photovoltaik.Verbrauch', '%01,2f kW') }} <br>
            Temperatur Inverter: {{ basic.print('', 'Photovoltaik.Inverter_Temperatur', '%01,1f °C') }} <br>
	    </div>
    </div>
</div> 
```
