# Weather App

Search a city and get its current weather from OpenWeatherMap: temperature,
humidity, wind speed and a matching icon, with an error state for unknown cities.

A single-page HTML/CSS/JS exercise - one inline script, no framework and no build
step.

## How it works

- `checkWeather(city)` calls
  `https://api.openweathermap.org/data/2.5/weather?units=metric&q=<city>`
  and fills the `.city`, `.temp`, `.humidity` and `.wind` elements.
- A 404 flips on the `.error` block and hides the weather panel.
- The icon is swapped from `images/` based on the condition (Clouds, Clear,
  Rain, Drizzle, Mist).
- Runs once on load, and again on the search button.

## Live demo

https://erfan-revenant.github.io/Weather-App/

## Run

```bash
git clone https://github.com/ErfanBagheri404/Weather-App.git
cd Weather-App
```

Open `index.html`. An OpenWeatherMap API key is required; the key currently sits
inline near the top of the `<script>` block in `index.html` - move it out and
rotate it if this repo stays public.

## Files

| file | role |
|---|---|
| `index.html` | markup, styles are external, weather fetch + render |
| `style.css` | card layout, search bar, typography |
| `images/` | weather and UI icons |
