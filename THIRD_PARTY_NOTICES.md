# Third-party notices

The generated five-letter dictionaries in `words.js` are derived from
[wordfreq](https://github.com/rspeer/wordfreq) by Robyn Speer and contributors.

- wordfreq code: Apache License 2.0
- Included corpus data: Creative Commons Attribution-ShareAlike 4.0 and the
  additional source terms documented by the wordfreq project

The generation script is available at `scripts/generate_words.py`. It filters
the frequency-ranked source lists to alphabetic, five-character words and
stores the highest-frequency candidates available for each supported language,
with a combined target of 100,000 accepted guesses. Answer selection is kept
separate and limited to 500 common candidates per language to protect puzzle
quality.
See the upstream
[wordfreq README](https://github.com/rspeer/wordfreq/blob/master/README.md)
for the complete source and attribution details.

The answer-only exclusion list in `scripts/answer_exclusions.json` is generated
from:

- [Onomaverse Most Popular Names by Country (2026)](https://github.com/onomaverse/datasets/tree/main/popular-names-by-country-2026),
  licensed under CC BY 4.0. Names data from Onomaverse.
- [GeoNames](https://www.geonames.org/), accessed through the MIT-licensed
  [geonamescache](https://github.com/yaph/geonamescache) package. GeoNames data
  is licensed under CC BY 4.0.
- Localized territory names from [Unicode CLDR](https://cldr.unicode.org/),
  accessed through the BSD-licensed [Babel](https://babel.pocoo.org/) package.

These sources are used only to keep personal names, cities, countries and
capitals out of the random answer pool. Excluded terms can still be submitted
as valid guesses when they exist in the frequency dictionary.
