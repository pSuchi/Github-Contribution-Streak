<p align="center">
  <img src="https://i.imgur.com/GZHodUG.png" width="100px"/>
  <h3 align="center">Github Readme Streak Stats</h3>
</p>

<p align="center">
  Display your total contributions, current streak,
  <br/>
  and longest streak on your GitHub profile README
</p>

<p align="center">
  <a href="https://github.com/search?q=extension%3Amd+%22github+readme+streak+stats+herokuapp%22&type=Code" alt="Users" title="Repo users">
    <img src="https://freshidea.com/jonah/app/github-search-results/streak-stats"/></a>
  <a href="https://discord.gg/fPrdqh3Zfu" alt="Discord" title="Dev Pro Tips Discussion & Support Server">
    <img src="https://img.shields.io/discord/819650821314052106?color=7289DA&logo=discord&logoColor=white&style=for-the-badge"/></a>
</p>

## ⚡ Quick setup

1. Copy-paste the markdown below into your GitHub profile README
2. Replace the value after `?user=` with your GitHub username

```md
[![GitHub Streak](https://streak-stats.demolab.com/?user=DenverCoder1)](https://git.io/streak-stats)
```

3. Star the repo 😄


## ⚙ Demo Site

Here you can customize your Streak Stats card with a live preview.

<https://streak-stats.demolab.com>

[![Demo Site](https://user-images.githubusercontent.com/20955511/114579753-dbac8780-9c86-11eb-97dd-207039f67d20.gif "Demo Site")](http://streak-stats.demolab.com/demo/)

## 🔧 Options

The `user` field is the only required option. All other fields are optional.

If the `theme` parameter is specified, any color customizations specified will be applied on top of the theme, overriding the theme's values.

|         Parameter          |                     Details                      |                                              Example                                               |
| :------------------------: | :----------------------------------------------: | :------------------------------------------------------------------------------------------------: |
|           `user`           |        GitHub username to show stats for         |                                           `DenverCoder1`                                           |
|          `theme`           |     The theme to apply (Default: `default`)      |                          `dark`, `radical`, etc. [🎨➜](./docs/themes.md)                           |
|       `hide_border`        |  Make the border transparent (Default: `false`)  |                                         `true` or `false`                                          |
|      `border_radius`       | Set the roundness of the edges (Default: `4.5`)  |                           Number `0` (sharp corners) to `248` (ellipse)                            |
|        `background`        |  Background color (eg. `f2f2f2`, `35,d22,00f`)   | **hex code** without `#`, **css color**, or gradient in the form `angle,start_color,...,end_color` |
|          `border`          |                   Border color                   |                             **hex code** without `#` or **css color**                              |
|          `stroke`          |        Stroke line color between sections        |                             **hex code** without `#` or **css color**                              |
|           `ring`           |   Color of the ring around the current streak    |                             **hex code** without `#` or **css color**                              |
|           `fire`           |          Color of the fire in the ring           |                             **hex code** without `#` or **css color**                              |
|      `currStreakNum`       |              Current streak number               |                             **hex code** without `#` or **css color**                              |
|         `sideNums`         |         Total and longest streak numbers         |                             **hex code** without `#` or **css color**                              |
|     `currStreakLabel`      |               Current streak label               |                             **hex code** without `#` or **css color**                              |
|        `sideLabels`        |         Total and longest streak labels          |                             **hex code** without `#` or **css color**                              |
|          `dates`           |              Date range text color               |                             **hex code** without `#` or **css color**                              |
|     `excludeDaysLabel`     |       Excluded days of the week text color       |                             **hex code** without `#` or **css color**                              |
|       `date_format`        |  Date format pattern or empty for locale format  |                        See note below on [📅 Date Formats](#-date-formats)                         |
|          `locale`          |  Locale for labels and numbers (Default: `en`)   |                            ISO 639-1 code - See [🗪 Locales](#-locales)                             |
|           `type`           |          Output format (Default: `svg`)          |                              Current options: `svg`, `png` or `json`                               |
|           `mode`           |          Streak mode (Default: `daily`)          |             `daily` (contribute daily) or `weekly` (contribute once per Sun-Sat week)              |
|       `exclude_days`       | List of days of the week to exclude from streaks |    Comma-separated list of day abbreviations (Sun, Mon, Tue, Wed, Thu, Fri, Sat) e.g. `Sun,Sat`    |
|    `disable_animations`    |    Disable SVG animations (Default: `false`)     |                                         `true` or `false`                                          |
|        `card_width`        |   Width of the card in pixels (Default: `495`)   |                        Positive integer, minimum width is 100px per column                         |
|       `card_height`        |  Height of the card in pixels (Default: `195`)   |                             Positive integer, minimum height is 170px                              |
| `hide_total_contributions` | Hide the total contributions (Default: `false`)  |                                         `true` or `false`                                          |
|   `hide_current_streak`    |    Hide the current streak (Default: `false`)    |                                         `true` or `false`                                          |
|   `hide_longest_streak`    |    Hide the longest streak (Default: `false`)    |                                         `true` or `false`                                          |
|      `starting_year`       |          Starting year of contributions          |   Integer, must be `2005` or later, eg. `2017`. By default, your account creation year is used.    |

### 🖌 Themes

To enable a theme, append `&theme=` followed by the theme name to the end of the source URL:

```md
[![GitHub Streak](https://streak-stats.demolab.com/?user=DenverCoder1&theme=dark)](https://git.io/streak-stats)
```

|     Theme      |                            Preview                            |
| :------------: | :-----------------------------------------------------------: |
|   `default`    |          ![default](https://i.imgur.com/IaTuYdS.png)          |
|     `dark`     |           ![dark](https://i.imgur.com/bUrsjlp.png)            |
| `highcontrast` |       ![highcontrast](https://i.imgur.com/ovrVrTY.png)        |
|  More themes!  | **🎨 [See a list of all available themes](./docs/themes.md)** |

**If you have come up with a new theme you'd like to share with others, please see [Issue #32](https://github.com/DenverCoder1/github-readme-streak-stats/issues/32) for more information on how to contribute.**

### 🗪 Locales

The following are the locales that have labels translated in Streak Stats. The `locale` query parameter accepts any ISO language or locale code, see [here](https://gist.github.com/DenverCoder1/f61147ba26bfcf7c3bf605af7d3382d5) for a list of valid locales. The locale provided will be used for the date format and number format even if translations are not yet available.

<!-- This section is automatically generated by the `translation-progress.php` script. -->
<!-- prettier-ignore-start -->
<!-- TRANSLATION_PROGRESS_START -->
<table><tbody><tr><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L37"><code>en</code></a> - English<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L37"><img src="https://progress-bar.dev/100" alt="English 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L47"><code>am</code></a> - አማርኛ<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L47"><img src="https://progress-bar.dev/100" alt="አማርኛ 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L56"><code>ar</code></a> - العربية<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L56"><img src="https://progress-bar.dev/100" alt="العربية 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L83"><code>ca</code></a> - català<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L83"><img src="https://progress-bar.dev/100" alt="català 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L92"><code>ceb</code></a> - Binisaya<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L92"><img src="https://progress-bar.dev/100" alt="Binisaya 100%"></a></td></tr><tr><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L101"><code>da</code></a> - dansk<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L101"><img src="https://progress-bar.dev/100" alt="dansk 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L110"><code>de</code></a> - Deutsch<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L110"><img src="https://progress-bar.dev/100" alt="Deutsch 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L119"><code>el</code></a> - Ελληνικά<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L119"><img src="https://progress-bar.dev/100" alt="Ελληνικά 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L128"><code>es</code></a> - español<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L128"><img src="https://progress-bar.dev/100" alt="español 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L147"><code>fil</code></a> - Filipino<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L147"><img src="https://progress-bar.dev/100" alt="Filipino 100%"></a></td></tr><tr><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L156"><code>fr</code></a> - français<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L156"><img src="https://progress-bar.dev/100" alt="français 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L165"><code>gu</code></a> - ગુજરાતી<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L165"><img src="https://progress-bar.dev/100" alt="ગુજરાતી 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L174"><code>he</code></a> - עברית<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L174"><img src="https://progress-bar.dev/100" alt="עברית 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L184"><code>hi</code></a> - हिन्दी<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L184"><img src="https://progress-bar.dev/100" alt="हिन्दी 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L201"><code>hu</code></a> - magyar<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L201"><img src="https://progress-bar.dev/100" alt="magyar 100%"></a></td></tr><tr><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L218"><code>id</code></a> - Indonesia<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L218"><img src="https://progress-bar.dev/100" alt="Indonesia 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L227"><code>it</code></a> - italiano<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L227"><img src="https://progress-bar.dev/100" alt="italiano 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L236"><code>ja</code></a> - 日本語<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L236"><img src="https://progress-bar.dev/100" alt="日本語 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L247"><code>jv</code></a> - Jawa<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L247"><img src="https://progress-bar.dev/100" alt="Jawa 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L256"><code>kn</code></a> - ಕನ್ನಡ<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L256"><img src="https://progress-bar.dev/100" alt="ಕನ್ನಡ 100%"></a></td></tr><tr><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L265"><code>ko</code></a> - 한국어<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L265"><img src="https://progress-bar.dev/100" alt="한국어 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L274"><code>mr</code></a> - मराठी<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L274"><img src="https://progress-bar.dev/100" alt="मराठी 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L283"><code>ms</code></a> - Melayu<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L283"><img src="https://progress-bar.dev/100" alt="Melayu 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L292"><code>my</code></a> - မြန်မာ<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L292"><img src="https://progress-bar.dev/100" alt="မြန်မာ 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L301"><code>ne</code></a> - नेपाली<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L301"><img src="https://progress-bar.dev/100" alt="नेपाली 100%"></a></td></tr><tr><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L310"><code>nl</code></a> - Nederlands<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L310"><img src="https://progress-bar.dev/100" alt="Nederlands 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L319"><code>no</code></a> - norsk<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L319"><img src="https://progress-bar.dev/100" alt="norsk 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L328"><code>pl</code></a> - polski<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L328"><img src="https://progress-bar.dev/100" alt="polski 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L337"><code>ps</code></a> - پښتو<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L337"><img src="https://progress-bar.dev/100" alt="پښتو 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L348"><code>pt_BR</code></a> - português (Brasil)<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L348"><img src="https://progress-bar.dev/100" alt="português (Brasil) 100%"></a></td></tr><tr><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L357"><code>ru</code></a> - русский<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L357"><img src="https://progress-bar.dev/100" alt="русский 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L374"><code>sa</code></a> - संस्कृत भाषा<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L374"><img src="https://progress-bar.dev/100" alt="संस्कृत भाषा 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L383"><code>sd_PK</code></a> - سنڌي (پاڪستان)<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L383"><img src="https://progress-bar.dev/100" alt="سنڌي (پاڪستان) 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L394"><code>sr</code></a> - српски<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L394"><img src="https://progress-bar.dev/100" alt="српски 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L403"><code>su</code></a> - Basa Sunda<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L403"><img src="https://progress-bar.dev/100" alt="Basa Sunda 100%"></a></td></tr><tr><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L436"><code>th</code></a> - ไทย<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L436"><img src="https://progress-bar.dev/100" alt="ไทย 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L445"><code>tr</code></a> - Türkçe<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L445"><img src="https://progress-bar.dev/100" alt="Türkçe 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L454"><code>uk</code></a> - українська<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L454"><img src="https://progress-bar.dev/100" alt="українська 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L463"><code>ur_PK</code></a> - اردو (پاکستان)<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L463"><img src="https://progress-bar.dev/100" alt="اردو (پاکستان) 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L474"><code>vi</code></a> - Tiếng Việt<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L474"><img src="https://progress-bar.dev/100" alt="Tiếng Việt 100%"></a></td></tr><tr><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L483"><code>yo</code></a> - Èdè Yorùbá<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L483"><img src="https://progress-bar.dev/100" alt="Èdè Yorùbá 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L493"><code>zh_Hans</code></a> - 中文（简体）<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L493"><img src="https://progress-bar.dev/100" alt="中文（简体） 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L503"><code>zh_Hant</code></a> - 中文（繁體）<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L503"><img src="https://progress-bar.dev/100" alt="中文（繁體） 100%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L67"><code>bg</code></a> - български<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L67"><img src="https://progress-bar.dev/86" alt="български 86%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L75"><code>bn</code></a> - বাংলা<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L75"><img src="https://progress-bar.dev/86" alt="বাংলা 86%"></a></td></tr><tr><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L137"><code>fa</code></a> - فارسی<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L137"><img src="https://progress-bar.dev/86" alt="فارسی 86%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L193"><code>ht</code></a> - Haitian Creole<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L193"><img src="https://progress-bar.dev/86" alt="Haitian Creole 86%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L210"><code>hy</code></a> - հայերեն<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L210"><img src="https://progress-bar.dev/86" alt="հայերեն 86%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L366"><code>rw</code></a> - Kinyarwanda<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L366"><img src="https://progress-bar.dev/86" alt="Kinyarwanda 86%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L412"><code>sv</code></a> - svenska<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L412"><img src="https://progress-bar.dev/86" alt="svenska 86%"></a></td></tr><tr><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L420"><code>sw</code></a> - Kiswahili<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L420"><img src="https://progress-bar.dev/86" alt="Kiswahili 86%"></a></td><td><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L428"><code>ta</code></a> - தமிழ்<br /><a href="https://github.com/DenverCoder1/github-readme-streak-stats/blob/main/src/translations.php#L428"><img src="https://progress-bar.dev/86" alt="தமிழ் 86%"></a></td><td></td><td></td><td></td></tr></tbody></table>
<!-- TRANSLATION_PROGRESS_END -->
<!-- prettier-ignore-end -->

**If you would like to help translate the Streak Stats cards, please see [Issue #236](https://github.com/DenverCoder1/github-readme-streak-stats/issues/236) for more information.**

### 📅 Date Formats

If `date_format` is not provided or is empty, the PHP Intl library is used to determine the date format based on the locale specified in the `locale` query parameter.

A custom date format can be specified by passing a string to the `date_format` parameter.

The required format is to use format string characters from [PHP's date function](https://www.php.net/manual/en/datetime.format.php) with brackets around the part representing the year.

When the contribution year is equal to the current year, the characters in brackets will be omitted.

**Examples:**

|     Date Format     |                                     Result                                      |
| :-----------------: | :-----------------------------------------------------------------------------: |
| <pre>d F[, Y]</pre> | <pre>"2020-04-14" => "14 April, 2020"<br/><br/>"2024-04-14" => "14 April"</pre> |
|  <pre>j/n/Y</pre>   |   <pre>"2020-04-14" => "14/4/2020"<br/><br/>"2024-04-14" => "14/4/2024"</pre>   |
| <pre>[Y.]n.j</pre>  |     <pre>"2020-04-14" => "2020.4.14"<br/><br/>"2024-04-14" => "4.14"</pre>      |
| <pre>M j[, Y]</pre> |   <pre>"2020-04-14" => "Apr 14, 2020"<br/><br/>"2024-04-14" => "Apr 14"</pre>   |

### Example

```md
[![GitHub Streak](https://streak-stats.demolab.com/?user=denvercoder1&currStreakNum=2FD3EB&fire=pink&sideLabels=F00&date_format=[Y.]n.j)](https://git.io/streak-stats)
```

## ℹ️ How these stats are calculated

This tool uses the contribution graphs on your GitHub profile to calculate which days you have contributed.

To include contributions in private repositories, turn on the setting for "Private contributions" from the dropdown menu above the contribution graph on your profile page.

Contributions include commits, pull requests, and issues that you create in standalone repositories.

The longest streak is the highest number of consecutive days on which you have made at least one contribution.

The current streak is the number of consecutive days ending with the current day on which you have made at least one contribution. If you have made a contribution today, it will be counted towards the current streak, however, if you have not made a contribution today, the streak will only count days before today so that your streak will not be zero.

> [!NOTE]  
> You may need to wait up to 24 hours for new contributions to show up ([Learn how contributions are counted](https://docs.github.com/articles/why-are-my-contributions-not-showing-up-on-my-profile))
