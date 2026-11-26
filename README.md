# lanka-macro-coach

An AI nutrition coach for people on a budget who eat everyday Sri Lankan food: estimate the calories and protein in a meal from household portions (cups, plates, spoons), no food scale needed.

> 🚧 **Status: in development** (started Nov 2026). Features below are planned and will be ticked off as they're built.

## Why

Most calorie apps don't know what "a plate of rice with chicken curry and dhal" is worth, and general AI chatbots guess. Hiring a coach or dietitian isn't affordable for many students. This project grounds the answers in real Sri Lankan food composition data instead of guesses.

## Planned features

- [ ] Chat with a local LLM that remembers the conversation
- [ ] Look up calories, protein, carbs and fat for cooked Sri Lankan dishes
- [ ] Convert household portions (cups, plates, spoons) to grams
- [ ] Answer questions grounded in the data, with the source shown
- [ ] FastAPI backend with a simple web front end
- [ ] Stretch: exercise technique and progressive overload guidance

## Tech stack (planned)

- **Python**
- **Ollama** running `qwen3:8b` locally (switchable to a hosted API)
- **FastAPI** for the API
- **ChromaDB** + `nomic-embed-text` embeddings for retrieval (RAG)

## Data

Nutrient values for cooked Sri Lankan dishes come from:

> Opatha, J., Dissanayake, L., Herath, B., Jayaweera, K., Wijesinghe, H., Wijesinghe, H., Jabir, S., Sumathipala, A., Rijsdijk, F. V., Zavos, H. M. S., & Jayawardena, R. (2025). *Development of a country-specific food composition database for Sri Lanka.* Journal of Food Composition and Analysis, 140, 107230. https://doi.org/10.1016/j.jfca.2025.107230

The article is published under the [Creative Commons Attribution 4.0 (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/) licence. Values used here are taken from its Appendix A; any changes made to the data (e.g. corrections or unit conversions) are noted in the code.

Online database by the same team: [foodcompositiondb.lk](https://www.foodcompositiondb.lk/)

## Disclaimer

This is a student portfolio project. Estimates are approximate and are not medical or dietary advice.

## Author

Sanuda Samarajeewa — Computer Science student, IIT Sri Lanka / University of Westminster · [GitHub](https://github.com/FateOrByDesign)
