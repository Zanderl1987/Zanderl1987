# Zander Luke

Data scientist in Charlottesville, Virginia. I have a never ending quest to build things that are useful. Most of what I build is shaped by understanding the fundamental business or scientific need for a problem. That's one of my strengths. I think that part of why this field is so exciting is learning the context behind the data and getting exposure to learning about new concepts, industries, and new problems that need to be solved. I enjoy the challenge of wrangling messy data and the satisfaction of creating a wonderfully formatted dataset, dashboard or whatever the final product is. Then it gets more fun if we build machine learning models on that data that produce statistically significant and actionable insights that move the needle, solve a problem, or prevent a problem. I enjoy new challenges and my natural curiosity drives my appetite for constantly learning new things. I would love to collaborate with anybody that is interested so please reach out!

Currently looking for data science, AI engineering, or ML engineering work, remote or hybrid.

## What I've been working on

**[financial-data-pipeline](https://github.com/Zanderl1987/financial-data-pipeline)** is the
large one. Around 90 ingestion pipelines feed a Hive-partitioned Parquet store, which gets
deduplicated into 130+ curated tables behind a DuckDB query layer, with cross-sectional factor
signals and event-study backtests running on top of that. The part I care most about is the
point-in-time correctness: features join on publication date with explicit lags, so a backtest
can't quietly learn from numbers that hadn't been released yet. There are 761 tests, a fair
number of which exist because a new pipeline once went missing from the query layer and nothing
complained. Adding one now fails the suite until it's wired into every layer it belongs in.

**[earnings_sentiment_tool](https://github.com/Zanderl1987/earnings_sentiment_tool)** looks at
what companies say on earnings calls, scoring sentiment and verbosity across transcripts. It
started as a question about whether executives get wordier when the news is bad. On the
evidence so far they don't, or at least not detectably: one of 90 correlations clears p < 0.05,
which is roughly what you'd get from nothing at all. Writing that up honestly seemed more
useful than hunting for a specification that said otherwise.

**[consumer-goods-price-pipeline](https://github.com/Zanderl1987/consumer-goods-price-pipeline)**
takes the same architecture in a different direction: 26 tables of consumer prices assembled from
BLS, USDA, EIA, FRED, and crowdsourced grocery data, covering everything from eggs to gas to used
cars. Most of it runs without an API key at all, which took some hunting.

**[freight-rail-data-pipeline](https://github.com/Zanderl1987/freight-rail-data-pipeline)** pulls
freight rail and ocean container shipping rates together from ten-plus public sources that all
disagree about units, geography, and how often they update.

**[ClinicalTrialsGovParser](https://github.com/Zanderl1987/ClinicalTrialsGovParser)** parses
ClinicalTrials.gov and AACT records into a structured store worth querying.

## Tools I reach for

Python, mostly, with pandas, DuckDB, and Parquet doing the heavy lifting. NumPy and SciPy for the
statistics, scikit-learn and PyTorch when a model is warranted, transformers and LLM APIs for
text work. pytest throughout, because the failures I care about are the silent ones.

## Elsewhere

zander.s.luke@gmail.com · [LinkedIn](https://www.linkedin.com/in/zander-luke-06790049)


<!-- profile readme -->
