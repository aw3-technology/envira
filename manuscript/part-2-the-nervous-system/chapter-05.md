# Chapter 5: AI Meets Climate Science
## The Algorithm That Learned to Predict the Planet

**Part II: The Nervous System — Earth Learns to See**

**Word Count Target:** 8,000 words

**Central Argument:** Artificial intelligence is transforming environmental science from a data-rich but insight-poor field into one capable of real-time prediction and automated monitoring at planetary scale. This chapter examines the most significant AI applications in climate and environmental science — from weather forecasting to emissions tracking to biodiversity monitoring — while honestly confronting AI's own environmental footprint and limitations.

---

## Opening Scene

**Setting:** Google DeepMind's London offices, late 2022 / early 2023 — the period when the GraphCast team validated their model against ECMWF's HRES operational forecast.

**Scene Description:** Reconstruct the moment when Remi Lam and the DeepMind team ran GraphCast against the gold standard of weather prediction — ECMWF's Integrated Forecasting System (IFS), the best operational numerical weather prediction model in the world. GraphCast, trained on 39 years of ERA5 reanalysis data, produced 10-day global weather forecasts in under 60 seconds on a single Google TPU v4 machine. When they compared results across 1,380 verification targets, GraphCast outperformed HRES on 90% of them. Describe the significance: a machine learning model, trained purely on historical data with no explicit encoding of atmospheric physics equations, had learned to predict the weather better than the physics-based model that hundreds of scientists had spent decades building. Ground this in the published Science paper (Lam et al., 2023) and DeepMind's public blog posts.

**Narrative Purpose:** Illustrate the paradigm shift AI represents for environmental science. The weather forecasting breakthrough is the clearest, most verifiable example — a domain with decades of objective verification infrastructure — making it the ideal entry point for a broader discussion of AI's environmental applications.

---

## Section 1: The Weather Prediction Revolution

**Header:** When Machine Learning Outran the Supercomputers

**Content Notes:**

- **Traditional numerical weather prediction (NWP):** Brief explanation of how weather forecasting has worked since the 1950s — solving the Navier-Stokes equations and thermodynamic equations on a 3D grid of the atmosphere. Requires massive supercomputers (ECMWF's Atos system ranks among the world's most powerful). Each forecast takes hours of computation. Improvements have come slowly — roughly one day of additional forecast skill per decade.

- **The AI weather revolution of 2022-2023:** In rapid succession, multiple AI models demonstrated weather forecasting skill comparable to or exceeding NWP:
  - **GraphCast (DeepMind):** Graph neural network trained on ERA5 reanalysis data. 10-day forecasts in under 60 seconds. Published in Science, November 2023 (Lam et al.).
  - **Pangu-Weather (Huawei):** Transformer-based model, published in Nature, July 2023 (Bi et al.). First AI model to outperform ECMWF's operational forecast.
  - **FourCastNet (NVIDIA):** Fourier neural operator architecture. Emphasized speed — 45,000x faster than traditional NWP for comparable accuracy. (Pathak et al., 2022).
  - **GenCast (DeepMind):** Diffusion-based model for probabilistic weather forecasting, addressing the limitation of deterministic AI models. Published in Nature, December 2024.

- **What this means and what it does not mean:** AI models complement rather than replace NWP. They are fast enough to run large ensembles (critical for uncertainty quantification). But they cannot yet handle novel climate regimes outside training data, and they lack physical interpretability. ECMWF is integrating AI into its operational pipeline, not replacing its physics models.

- **Implications for developing countries:** AI weather models can run on modest hardware, potentially democratizing weather forecasting. Discuss the significance for nations that lack supercomputer access for NWP.

**Key Data Points:**
- GraphCast produces 10-day forecasts in under 60 seconds on a single TPU v4 vs. hours on a supercomputer for ECMWF HRES. (Source: Lam et al., Science, 2023)
- GraphCast outperformed HRES on 90% of 1,380 verification targets. (Source: Lam et al., Science, 2023)
- Pangu-Weather was the first AI model demonstrated to exceed operational NWP skill. (Source: Bi et al., Nature, 2023)
- FourCastNet achieved 45,000x speedup over traditional NWP. (Source: Pathak et al., arXiv, 2022)
- Traditional NWP forecast skill has improved at ~1 day per decade since the 1980s. (Source: Bauer et al., Nature, 2015)

**Profiles:**
- **Remi Lam and the GraphCast team (DeepMind):** The researchers who built GraphCast. Lam's background and the team's approach of treating weather forecasting as a learned mapping problem.
- **ECMWF's response:** How the world's leading weather prediction center is adapting to the AI revolution — hiring ML researchers, integrating AI into their forecasting pipeline, and viewing AI as a complement rather than a threat.

---

## Section 2: AI for Emissions Tracking

**Header:** Climate TRACE — Making the Invisible Visible

**Content Notes:**

- **The emissions data problem:** National greenhouse gas inventories are self-reported, often delayed by 2+ years, and vary enormously in quality. Many countries lack the capacity for detailed emissions accounting. Some may have incentives to underreport. The Paris Agreement's transparency framework depends on accurate, verifiable emissions data.

- **Climate TRACE coalition:** Founded in 2020 by Al Gore, Gavin McCormick (WattTime), and a coalition of AI and remote sensing organizations. Mission: use satellites, sensors, and AI to independently track global GHG emissions from every major source, in near-real-time. Launched comprehensive global inventory at COP27 in November 2022.

- **How it works:** AI analyzes satellite imagery (optical and infrared) to identify and quantify emissions from individual facilities — power plants, oil refineries, steel mills, shipping vessels, agricultural operations. For example: visible plumes from smokestacks can be correlated with emissions rates; nighttime thermal signatures from steel mills indicate production levels; ship AIS tracking combined with vessel characteristics estimates maritime emissions.

- **Scale and granularity:** Climate TRACE now tracks 80,000+ individual emissions sources across 250+ countries. This facility-level granularity is unprecedented — most national inventories report at the sector level.

- **Impact and controversy:** Some countries have pushed back on independent emissions monitoring as an infringement on sovereignty. Others welcome it as a way to verify their own reporting. Discuss the political dynamics at COP negotiations.

**Key Data Points:**
- Climate TRACE tracks 80,000+ individual emissions sources globally. (Source: Climate TRACE, climatetrace.org, 2024 data release)
- National GHG inventories are typically 2-3 years delayed. (Source: UNFCCC reporting guidelines)
- Climate TRACE covers 10 major economic sectors and dozens of subsectors. (Source: Climate TRACE methodology documentation)
- WattTime's AI can estimate power plant emissions from satellite imagery of visible and thermal signatures. (Source: WattTime publications)

**Profiles:**
- **Gavin McCormick, co-founder of WattTime and Climate TRACE:** The data scientist who realized satellite imagery could be used to independently verify power plant emissions. His journey from academic research to founding a coalition endorsed by Al Gore.
- **Al Gore's involvement:** His role in co-founding and championing Climate TRACE as a tool for accountability under the Paris Agreement. His presentations at COP27 and COP28 unveiling the data.

---

## Section 3: Predicting Deforestation Before It Happens

**Header:** PrevisIA and the Shift from Detection to Prevention

**Content Notes:**

- **From reactive to predictive:** Chapter 4 described how monitoring detects deforestation after it happens. This section explores how AI enables prediction — identifying where deforestation is likely to occur before it happens, enabling preemptive intervention.

- **PrevisIA (Brazil):** Developed by Imazon (Amazon Institute of People and the Environment) in partnership with Microsoft AI for Earth and others. Uses machine learning to analyze historical deforestation patterns, road networks, land tenure data, enforcement history, commodity prices, and other variables to generate monthly deforestation risk maps for the Brazilian Amazon. These maps are provided to IBAMA (Brazil's environmental enforcement agency) and state governments to guide patrol deployment.

- **How it works technically:** Random forest and gradient boosting models trained on historical PRODES/DETER deforestation data combined with 15+ spatial and temporal predictor variables. The model identifies areas with high probability of deforestation in the coming 1-3 months. Validated against actual deforestation outcomes.

- **Effectiveness evidence:** Studies showing that areas patrolled based on PrevisIA predictions had lower deforestation rates than areas selected through traditional methods. Discuss the counterfactual challenge — how do you prove that deforestation was prevented?

- **Broader applications:** Similar predictive deforestation models in Indonesia (Global Forest Watch + WRI), Central Africa, and Southeast Asia. Google's Dynamic World land use classification enabling near-real-time land cover monitoring globally.

**Key Data Points:**
- PrevisIA generates monthly deforestation risk maps covering the entire Legal Amazon (~5 million km2). (Source: Imazon/PrevisIA documentation)
- The model uses 15+ predictor variables including road proximity, previous deforestation, land tenure, and enforcement history. (Source: PrevisIA methodology papers)
- Brazil's Legal Amazon lost approximately 13,000 km2 of forest in 2021 (peak under Bolsonaro) but this dropped to ~4,500 km2 in 2024 under Lula. (Source: INPE PRODES annual data)
- Microsoft AI for Earth has awarded $75+ million in grants for AI-driven environmental projects. (Source: Microsoft AI for Earth program page)

**Profiles:**
- **Imazon (Amazon Institute of People and the Environment):** The Brazilian NGO that developed PrevisIA. Profile Carlos Souza Jr. and the team's decades of work on Amazon deforestation monitoring, from manual satellite image interpretation to AI prediction.
- **Microsoft AI for Earth:** The program's role in funding and providing compute resources for environmental AI projects globally. Broader portfolio of grantees working on similar problems.

---

## Section 4: AI for Wildlife and Biodiversity

**Header:** Listening to the Forest, Watching the Wild

**Content Notes:**

- **The biodiversity monitoring challenge:** Unlike climate (which has temperature as a single key metric), biodiversity is multidimensional and difficult to measure at scale. Traditional methods — field surveys, transects, point counts — are slow, expensive, and limited in coverage. AI is enabling new approaches.

- **Camera traps + AI:** TrailGuard AI (developed by RESOLVE and Intel) uses on-device AI to identify animals and humans in camera trap images, transmitting only relevant images via satellite. This reduces data transmission needs by 95%+ and enables near-real-time poaching detection. Wildlife Insights (Google + conservation partners) uses AI to automatically classify species in camera trap images — processing millions of images that would take human reviewers years.

- **Acoustic monitoring + AI:** Building on Chapter 4's acoustic monitoring discussion, detail how AI transforms raw audio into biodiversity data. The BirdNET app (Cornell Lab of Ornithology / Chemnitz University of Technology) can identify 6,000+ bird species from sound recordings. Arbimon (Rainforest Connection) provides automated species identification for tropical ecosystems. Discuss how acoustic indices (acoustic diversity, bioacoustic index) provide landscape-level biodiversity indicators.

- **Marine applications:** AI-powered analysis of underwater acoustic monitoring to track whale populations, detect vessel traffic in marine protected areas. OceanMind uses AI and satellite data to detect illegal fishing. Global Fishing Watch (partnership between Google, Oceana, and SkyTruth) tracks 70,000+ fishing vessels using AIS data and AI.

- **Conservation AI (open source):** The Conservation AI platform developed at Liverpool John Moores University — provides open-source AI tools for camera trap and drone image analysis, making AI accessible to conservation organizations that lack technical capacity.

**Key Data Points:**
- BirdNET can identify 6,000+ bird species from audio recordings. (Source: BirdNET, Cornell Lab of Ornithology)
- Wildlife Insights has processed 120+ million camera trap images using AI. (Source: Wildlife Insights, wildlifeinsights.org)
- Global Fishing Watch tracks 70,000+ commercial fishing vessels. (Source: Global Fishing Watch, globalfishingwatch.org)
- TrailGuard AI cameras reduce data transmission by 95%+ through on-device inference. (Source: RESOLVE / Intel TrailGuard publications)
- Camera trap studies using AI can process images 500x faster than manual review. (Source: Norouzzadeh et al., PNAS, 2018)

**Profiles:**
- **Eric Berger and the TrailGuard AI team (RESOLVE):** The story of developing AI-enabled camera traps that can detect poachers in real time and alert rangers.
- **Stefan Kahl (BirdNET / Cornell Lab):** The researcher behind BirdNET's neural network for bird sound identification. How citizen science and AI combine — millions of users contributing audio data that trains better models.
- **Global Fishing Watch:** How AI and satellite data created unprecedented transparency in global fishing activity, enabling detection of illegal, unreported, and unregulated (IUU) fishing.

---

## Section 5: Limitations and Risks

**Header:** The Costs, Blind Spots, and Dangers of AI for the Planet

**Content Notes:**

- **AI's own carbon footprint:** Training large AI models has a significant energy and carbon cost. Estimate the carbon cost of training models like GraphCast, GPT-4, etc. (Strubell et al., 2019 paper on NLP model training emissions as foundational reference; more recent estimates for LLMs). Discuss the tension between AI's potential environmental benefits and its own environmental cost. Note that inference costs are typically much lower than training costs.

- **Data biases:** AI models trained on historical data inherit historical biases. Weather models trained predominantly on data from well-observed regions (North America, Europe) may perform worse in data-sparse regions (Africa, parts of Asia, the oceans). Deforestation models trained on the Amazon may not transfer well to the Congo Basin. Biodiversity models trained on charismatic species may miss less-studied taxa.

- **Over-reliance on models:** The risk of trusting AI predictions uncritically. AI weather models can produce physically implausible results that physics-based models would not. The "black box" problem — when a model's prediction contradicts domain expertise, how should scientists respond?

- **Interpretability and trust:** Climate scientists need to understand why a model makes a prediction, not just what it predicts. Discuss the tension between accuracy and interpretability. Efforts in explainable AI (XAI) for environmental applications.

- **Access and equity:** Who builds and controls environmental AI? Concentration in a few large tech companies (Google, Microsoft, NVIDIA). The "AI divide" — well-resourced institutions benefit while those most affected by environmental crises may lack access. Open-source initiatives (HuggingFace climate models, Open Climate Fix) as partial solutions.

- **The automation trap:** If AI can monitor and predict environmental change, does it reduce pressure on humans to act? The risk that better data and predictions become substitutes for political action rather than catalysts for it.

**Key Data Points:**
- Training a single large AI model can emit as much CO2 as five cars over their lifetimes (early estimate; more nuanced recent data needed). (Source: Strubell et al., ACL 2019 — note: this figure is debated and may need updating)
- Google's total energy consumption was 18.3 TWh in 2022, with data centers being the largest component. (Source: Google Environmental Report, 2023)
- AI weather model inference: GraphCast uses ~0.001% of the energy required for a traditional NWP forecast. (Source: Lam et al., Science, 2023, supplementary materials)
- Africa has fewer weather observation stations per square kilometer than any other continent. (Source: WMO State of Climate Services reports)

**Profiles:**
- **Open Climate Fix (Jack Kelly):** A non-profit using open-source AI to optimize solar energy forecasting for the UK national grid. A model for making environmental AI accessible and equitable.
- **The AI Ethics in Climate Science debate:** Profile the ongoing academic debate about responsible AI use in climate science — key voices include researchers at Climate Change AI (David Rolnick, Priya Donti) who advocate for thoughtful, impactful AI deployment.

---

## Source References

1. Lam, R. et al. "Learning Skillful Medium-Range Global Weather Forecasting." Science 382, no. 6677 (2023): 1416-1421.
2. Bi, K. et al. "Accurate Medium-Range Global Weather Forecasting with 3D Neural Networks." Nature 619 (2023): 533-538.
3. Pathak, J. et al. "FourCastNet: A Global Data-Driven High-Resolution Weather Forecasting Model." arXiv:2202.11214 (2022).
4. Price, I. et al. "GenCast: Diffusion-Based Ensemble Forecasting for Medium-Range Weather." Nature 636 (2024): 1071-1078.
5. Climate TRACE. "Global Greenhouse Gas Emissions Inventory." climatetrace.org. 2024 data release.
6. Imazon. "PrevisIA: Predicting and Preventing Deforestation in the Amazon." imazon.org.br.
7. Strubell, E. et al. "Energy and Policy Considerations for Deep Learning in NLP." Proceedings of the 57th Annual Meeting of the ACL (2019).
8. Norouzzadeh, M.S. et al. "Automatically Identifying, Counting, and Describing Wild Animals in Camera-Trap Images." PNAS 115, no. 25 (2018): E5716-E5725.
9. Global Fishing Watch. "Tracking Global Fishing Activity." globalfishingwatch.org.
10. Wildlife Insights. "AI for Camera Trap Image Analysis." wildlifeinsights.org.
11. BirdNET. "Sound Identification for 6,000+ Bird Species." birdnet.cornell.edu.
12. Bauer, P. et al. "The Quiet Revolution of Numerical Weather Prediction." Nature 525 (2015): 47-55.
13. Google Environmental Report 2023. sustainability.google.
14. Microsoft AI for Earth. "AI for Earth Grants." microsoft.com/en-us/ai/ai-for-earth.
15. Rolnick, D. et al. "Tackling Climate Change with Machine Learning." ACM Computing Surveys 55, no. 2 (2022): 1-96.

---

**Transition to Chapter 6:** End with the observation that AI's greatest potential may lie not in any single application but in its ability to integrate diverse data streams into unified models of Earth's systems — setting up the concept of digital twins as the ultimate synthesis of monitoring, AI, and simulation.
