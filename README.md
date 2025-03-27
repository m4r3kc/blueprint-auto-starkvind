# blueprint-auto-starkvind
<h3>Opis Projektu</h3>
Blueprint ten służy do automatyzacji sterowania prędkością oczyszczacza powietrza IKEA Starkvind na podstawie poziomu zanieczyszczenia powietrza cząstkami PM2.5. Projekt ten pozwala na efektywne zarządzanie jakością powietrza w pomieszczeniu, dostosowując moc oczyszczacza do aktualnych potrzeb.
<h3>Struktura Blueprintu</h3>
<ul>
<li><strong>Nazwa</strong>: Sterowanie mocą oczyszczacza powietrza IKEA Starkvind na podstawie PM2.5</li>
<li><strong>Opis</strong>: Automatyczna regulacja mocy oczyszczacza powietrza IKEA Starkvind w zależności od odczytu PM2.5.</li>
<li><strong>Domena</strong>: Automatyzacja (automation)</li>
</ul>
<h3>Wejścia</h3>
<ul>
<li><p><strong>pm2_5_sensor</strong>: </p>
<ul>
<li><strong>Nazwa</strong>: Czujnik PM2.5</li>
<li><strong>Opis</strong>: Czujnik odpowiedzialny za pomiar cząsteczek PM2.5.</li>
<li><strong>Selector</strong>: Wybór encji z domeny sensor.</li>
</ul>
</li>
<li><p><strong>fan_entities</strong>: </p>
<ul>
<li><strong>Nazwa</strong>: Oczyszczacze powietrza</li>
<li><strong>Opis</strong>: Wybierz encje, obszary lub urządzenia dotyczące oczyszczacza powietrza.</li>
<li><strong>Selector</strong>: Wybór encji z domeny fan.</li>
</ul>
</li>
</ul>
<h3>Mechanizm Działania</h3>
<ol>
<li><p><strong>Trigger</strong>: Zmiana stanu czujnika PM2.5 inicjuje automatyzację.</p>
</li>
<li><p><strong>Akcja</strong>: W oparciu o odczyt PM2.5, blueprint wykonuje odpowiednią akcję:</p>
<ul>
<li><strong>&lt;10</strong>: Uruchamia tryb automatyczny oczyszczacza.</li>
<li><strong>10-14</strong>: Ustala prędkość na 20%.</li>
<li><strong>14-18</strong>: Ustala prędkość na 30%.</li>
<li><strong>18-24</strong>: Ustala prędkość na 40%.</li>
<li><strong>24-31</strong>: Ustala prędkość na 60%.</li>
<li><strong>31-50</strong>: Ustala prędkość na 80%.</li>
<li><strong>&gt;50</strong>: Ustala prędkość na 100%.</li>
</ul>
</li>
</ol>
<h3>Tryb</h3>
<ul>
<li><strong>Mode</strong>: single - zapewnia, że automatyzacja nie zostanie ponownie zainicjowana dopóki bieżące zadanie nie zostanie zakończone.</li>
</ul>
<h3>Konfiguracja</h3>
<p>Aby skonfigurować ten blueprint w Home Assistant:</p>
<ol>
<li>Włącz integrację dla czujników PM2.5 oraz dla oczyszczaczy powietrza.</li>
<li>Importuj blueprint do konfiguracji Home Assistant.</li>
<li>Ustaw wymagane wejścia przy użyciu interfejsu Home Assistant, wybierając odpowiednie czujniki PM2.5 oraz urządzenia z domeny fan.</li>
</ol>
<h3>Uwagi</h3>
<ul>
<li>Upewnij się, że czujniki PM2.5 i oczyszczacze powietrza są prawidłowo zintegrowane i skonfigurowane w Home Assistant, aby blueprint działał zgodnie z oczekiwaniami.</li>
</ul>
<p>(TAGI: HomeAssistant, IkeaStarkvind, Automation, PM2_5, AirPurifier, Blueprint)</p>

<a href="https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fraw.githubusercontent.com%2Fm4r3kc%2Fblueprint-auto-starkvind%2Frefs%2Fheads%2Fmain%2Fikea-starkvind-control.yaml">
  <img width="250" alt="blueprint" src="https://github.com/user-attachments/assets/fa01530a-1d52-4b2b-b637-1269bd0cd747">
</a>
