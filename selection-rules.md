# Literature screening profile — journals, topics and selection rules

Derived from the group's monthly journal reviews, **March 2020 – October 2026** (~4,200 selected papers). Person names of the posters have been disregarded throughout, as requested.

This file is written to be pasted into an AI assistant as a standing instruction for monthly screening. Sections 1–4 are the profile; section 5 is the task prompt; section 6 lists the points you may want to correct before first use.

---

## 1. Scope in one paragraph

The group works on **evolutionary and population genomics applied to conservation and to wild populations**, with strong secondary interests in (a) theoretical/statistical population genetics, (b) methods and software for genomic and biodiversity data, (c) human and medical genetics as a source of methods and comparative results, and (d) domestication and applied breeding in animals and plants. Study systems are overwhelmingly non-model vertebrates (mammals, birds, amphibians, fish, reptiles), with regular plants, insects and humans.

---

## 2. Journals to monitor

### Tier A — screened every month without exception (appear in nearly every review)

| Journal | Typical focus in the reviews |
|---|---|
| Evolution | core evolutionary genetics, theory and empirical |
| Molecular Ecology | population/landscape genomics of wild populations |
| Molecular Ecology Resources | methods, markers, pipelines |
| Heredity | population and quantitative genetics |
| Journal of Heredity | conservation and applied genetics |
| Genetics | theory, methods, model systems |
| G3: Genes, Genomes, Genetics | genomic resources, assemblies, mapping |
| Genome Biology and Evolution (GBE) | comparative/genome evolution |
| Molecular Biology and Evolution (MBE) | molecular evolution, phylogenomics |
| Genome Research | genomics methods and resources |
| Bioinformatics | tools, algorithms |
| PLOS Genetics | genetics across systems |
| PLOS Computational Biology | models, inference |
| PLOS Biology | broad, selected |
| eLife | broad, selected |
| PNAS | broad, selected |
| Nature, Science, Nature Communications, Science Advances | high-profile, selected |
| Nature Ecology & Evolution | ecology and evolution |
| Nature Genetics | genetics, mostly human/method relevance |
| Nature Reviews Genetics | reviews |
| Trends in Ecology & Evolution | reviews and opinion |
| Proceedings of the Royal Society B | broad evolution/ecology |
| Biology Letters | short reports |
| Ecology Letters | ecology with evolutionary angle |
| Journal of Animal Ecology | population ecology, demography |
| Evolution Letters | short-format evolution |
| Journal of Evolutionary Biology | core evolution |
| Evolutionary Applications | applied conservation/management genetics |
| Conservation Biology | conservation science |
| Biological Conservation | conservation science |
| Conservation Genetics | conservation genetics |
| Animal Conservation | conservation, species-level |
| Biodiversity and Conservation | conservation, biodiversity |
| Methods in Ecology and Evolution | field and analytical methods |
| Ecology and Evolution | broad, high volume — screen strictly |
| BMC Ecology and Evolution | broad |
| BMC Genomics | genomic resources |
| American Naturalist | theory, natural history |
| Theoretical Population Biology | population genetic theory |
| American Journal of Human Genetics | human genetics, method transfer |
| Philosophical Transactions of the Royal Society B | themed issues |
| Current Biology | selected |
| Evolution, Medicine and Public Health | evolutionary medicine |
| American Journal of Botany | plant evolution |

### Tier B — screened when they publish something in scope (appeared occasionally)

Annual Review of Genetics · Annual Review of Ecology, Evolution and Systematics · Trends in Genetics · PLOS ONE · Scientific Reports · Behavioral Ecology · Journal of Applied Ecology · Horticulture Research · Cell · bioRxiv / EcoEvoRxiv preprints (flag as preprint)

> PLOS ONE, Scientific Reports and Ecology and Evolution have the loosest fit — only include when the topic match is strong (score ≥ 4 in section 4).

---

## 3. Topic taxonomy

Topics are listed by how often they drive a selection, strongest first. Keywords in `code` are the terms to match in title/abstract.

**T1. Conservation genetics and genomics of threatened populations** — `inbreeding`, `inbreeding depression`, `genetic load`, `deleterious variation`, `runs of homozygosity`, `heterozygosity`, `effective population size`, `Ne`, `bottleneck`, `genetic rescue`, `translocation`, `reintroduction`, `captive breeding`, `ex situ`, `population viability`, `extinction risk`, `genetic monitoring`, `conservation unit`, `management unit`

**T2. Population and landscape genomics of wild populations** — `population structure`, `gene flow`, `connectivity`, `dispersal`, `landscape genomics`, `isolation by distance`, `demographic history`, `coalescent inference`, `local adaptation`, `selective sweep`, `adaptive variation`, `genotype–environment association`

**T3. Hybridisation, introgression and speciation** — `hybridisation`, `hybrid zone`, `introgression`, `admixture`, `reproductive isolation`, `speciation`, `species delimitation`, `contact zone`, `anthropogenic hybridisation`

**T4. Evolutionary theory, quantitative and statistical population genetics** — `recombination landscape`, `linked selection`, `Hill–Robertson`, `mutation rate`, `distribution of fitness effects`, `polygenic adaptation`, `heritability`, `G matrix`, `selfing`, `mating system evolution`, `fitness landscape`, `simulation study`, `forward simulation`, `SLiM`, `assortative mating`

**T5. Methods, software and genomic resources** — `R package`, `pipeline`, `benchmark`, `genome assembly`, `reference genome`, `pangenome`, `long-read`, `structural variant`, `variant calling`, `imputation`, `machine learning`, `deep learning`, `low-coverage sequencing`, `SNP array`, `target capture`, `museum specimen`, `historical DNA`

**6. T6. Biodiversity assessment and monitoring technology** — `eDNA`, `environmental DNA`, `metabarcoding`, `biomonitoring`, `camera trap`, `bioacoustics`, `ecoacoustics`, `citizen science`, `iNaturalist`, `species distribution model`, `occupancy model`, `computer vision`

**T7. Domestication, breeding and agrobiodiversity** — `domestication`, `livestock`, `breed`, `crop`, `landrace`, `signatures of selection in domestic`, `dog`, `cattle`, `sheep`, `horse`, `yeast`

**T8. Ancient DNA and temporal genomics** — `ancient DNA`, `aDNA`, `palaeogenomics`, `sedaDNA`, `temporal sampling`, `time series genomics`, `extinct`

**T9. Eco-evolutionary responses to global change** — `climate change`, `range shift`, `invasive species`, `fragmentation`, `land use`, `protected areas`, `urbanisation`, `adaptive potential`, `evolutionary rescue`

**T10. Host–pathogen, immunogenetics and disease** — `host–pathogen`, `pathogen genomics`, `MHC`, `immunogenetics`, `disease susceptibility`, `wildlife disease`, `chytrid`, `zoonotic`, `epidemiological genomics`

**T11. Epigenetics and gene regulation in natural populations** — `methylation`, `epigenetic clock`, `transgenerational`, `plasticity`, `gene expression variation`, `eQTL`, `transcriptomics`

**T12. Life history, ageing, behaviour and sexual selection with a genetic or evolutionary angle** — `senescence`, `ageing`, `life history trade-off`, `reproductive success`, `sexual selection`, `mate choice`, `parentage`, `kinship`, `social structure`, `cultural evolution`

**T13. Human and medical genetics as method/comparative source** — `GWAS`, `polygenic score`, `human demographic history`, `pleiotropy`, `somatic evolution`, `human evolution`, `lncRNA`, `complex trait architecture`

**T14. Chromosome and genome biology** — `sex chromosome`, `polyploidy`, `karyotype`, `supergene`, `inversion`, `gene drive`, `holocentric`

---

## 4. Selection rules

### 4.1 Hard includes (select whenever the journal is in scope)

1. Study combines **genomic data with a conservation or management question** in a wild population (T1 + T2).
2. New **method, software, R package or benchmark** usable on population-genomic or biodiversity data (T5, T6).
3. **Theory or simulation** on recombination, selection, drift, mating systems or inference of demography (T4).
4. **Genome-wide study of hybridisation or introgression**, especially anthropogenic (T3).
5. **Review or synthesis** in Nature Reviews Genetics, TREE, Annual Reviews or a themed Phil Trans B issue on any T1–T14 topic.
6. **New reference genome or genomic resource** for a wild, threatened or domesticated non-model organism (T5, T7).
7. **Ancient or historical DNA** study of population change over time (T8).

### 4.2 Conditional includes (select only if also tied to genetics, evolution or quantitative methods)

- Pure ecology, behaviour or physiology → include only when there is a genetic, genomic, evolutionary, or clearly novel quantitative component (e.g. a demographic model, a monitoring method).
- Human/medical genetics → include when the method, statistical approach or result generalises beyond humans (T13), not for clinical findings as such.
- Plant science → include for evolution, population genetics, polyploidy, domestication; not for physiology or agronomy alone.
- Molecular and cell biology → include only when it bears on evolutionary process (e.g. mutation, recombination, gene regulation evolution).

### 4.3 Hard excludes

- Clinical trials, therapeutics, drug discovery, biomedical case reports.
- Cancer biology, unless framed as somatic evolution with population-genetic methods.
- Neuroscience, psychology and cognition without an evolutionary or genetic component.
- Biochemistry, structural biology, microbial physiology, biotechnology and bioengineering.
- Descriptive taxonomy or single-locus barcoding of one taxon with no population or methodological content.
- Local species checklists, single-site inventories, short natural-history notes.
- Corrections, retractions, editorials, obituaries, errata.
- Opinion pieces on science policy, funding or careers.

### 4.4 Scoring, for ranking within a month

Score each candidate 0–6 and report the score:

- +2 topic falls in T1–T5
- +1 topic falls in T6–T14
- +1 Tier A journal
- +1 non-model, wild or threatened organism
- +1 new method, tool, dataset or resource the group could reuse
- +1 broad conceptual significance (would be discussed beyond its own subfield)
- −2 matches a conditional-include category with no genetic/evolutionary/quantitative hook

Report everything scoring ≥ 3; report score 2 items only in a short "borderline" list; drop ≤ 1.

### 4.5 Volume guidance

The reviews average **25–40 papers per month** across all journals. If a month yields far more, raise the cutoff to score ≥ 4 rather than dropping journals, so that coverage stays even.

---

## 5. Task prompt for the monthly run

> Using the journal list, topic taxonomy and selection rules in this file, screen the tables of contents of the Tier A journals (and Tier B where relevant) published in `<month, year>`. Apply the hard includes, conditional includes and hard excludes, score each selected paper per section 4.4, and return the results grouped by journal, in this format:
>
> ```
> ## <Journal name> (Volume, Issue, Month Year)
> ### <Full paper title>
> <Author list>
> <DOI link>
> <One or two sentences: what was done and the main finding.>
> Topics: <T-codes and keywords>  |  Score: <n>
> ```
>
> Use "NONE" under a journal with nothing in scope. Add a final "Borderline" section for score-2 items, one line each with the reason they are borderline. Do not include author affiliations or the names of anyone who posted or recommended a paper.

---

## 6. Points to check before first use

1. **Journal list drift.** Some journals appear only in the early years (BMC Genetics, BMC Evolutionary Biology — both since renamed/merged; Horticulture Research; American Journal of Botany, which is frequent until ~2022 and rare after). Confirm whether these are still wanted, or whether they lapsed only because of who was covering them.
2. **Deliberately broad journals.** Nature, Science, PNAS, Current Biology and PLOS ONE entries include off-topic "for fun" picks (religion, diet and mortality, carbon budgets). I have treated those as not part of the profile. Say if you want a "general interest" slot kept.
3. **Preprints.** bioRxiv appears a handful of times. Currently Tier B with a preprint flag — tell me to drop or promote it.
4. **Taxonomic balance.** Mammals, birds, amphibians and fish dominate; insects, plants and marine invertebrates are thinner. If that reflects who was writing rather than the group's interests, the T-list should be rebalanced.
5. **The abstract/summary line.** Later reviews include a one- or two-sentence plain summary per paper; earlier ones only keyword tags. The task prompt above asks for the summary style, which is the current practice.
