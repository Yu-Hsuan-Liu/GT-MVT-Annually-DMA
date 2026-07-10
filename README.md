# GT-MVT-Annually-DMA

Annual Google Trends search interest in motor vehicle theft terms at the DMA (media market) level, 2011-2022. Companion to [GT-MVT-Annually-State](https://github.com/Yu-Hsuan-Liu/GT-MVT-Annually-State); same design, pulled at DMA resolution instead of states.

Each completed pass over 2011-2022 lands in `data/` as a timestamped `DMA_2011_2022_annually_*.csv` with one row per DMA and one column per year. Google Trends resamples on every request, so the runs were repeated many times; average them before use.

Requires pandas, pytrends, and selenium with the Edge WebDriver (point `executable_path` in the `get_cookie` cell at your local copy). Long sleeps between requests are intentional, a full run takes days.

Monthly city-level version: [GT-MVT-Monthly-City](https://github.com/Yu-Hsuan-Liu/GT-MVT-Monthly-City).
