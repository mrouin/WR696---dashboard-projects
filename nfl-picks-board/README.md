# NFL Picks Board

An R Shiny (R Markdown) dashboard that pulls live NFL picks for the selected week and averages them into one consensus pick per game.

**Sources:** NFL.com editors, CBS Sports experts, ESPN scoreboard + FPI, and (optional) sportsbook odds via The Odds API. Manual picks can be added in `picks.csv`.

## Run
```r
install.packages(c("shiny","rmarkdown","jsonlite","httr","rvest","xml2"))
rmarkdown::run("nfl-picks-dashboard.Rmd")
```

Optional multi-sportsbook odds: `Sys.setenv(ODDS_API_KEY = "your-key")` (free key at the-odds-api.com). Never commit your key; use `~/.Renviron`.

For information only, not betting advice.
