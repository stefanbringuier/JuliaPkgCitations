# Julia Pkg Citations
[![Valid .bib file](https://github.com/stefanbringuier/JuliaPkgCitations/actions/workflows/biber-check.yml/badge.svg)](https://github.com/stefanbringuier/JuliaPkgCitations/actions/workflows/biber-check.yml)

This repo provides the file [`juliapkgs.bib`](juliapkgs.bib) (**WIP**) that contains several entries for many popular and personally useful [Julia](https://julialang.org/) packages. The repo was inspired by [Miles Cranmer](https://github.com/MilesCranmer/python_citations) python repo.

> Note that if a peer-reviewed publication is available for a given Julia package, this is choosen as the default work to cite. Otherwise the github repo or other sources are used.

## List of citation keys

All keys use lowercase for the package name and contain the `.jl` extension, the only exception is the julia language itself which is just `\cite{julia}`. The year and author have been excluded.

| Citation Key                      | Package                                                                       				  | Use                        |
| :-------------------------------- | :---------------------------------------------------------------------------------------------------------- | :------------------------- |
| `\cite{julia}`                    | [Julia Language](https://github.com/JuliaLang/julia)                          				  | Programming Language       |
| `\cite{chemistryfeaturization.jl}`| [ChemistryFeaturization.jl](https://github.com/Chemellia/ChemistryFeaturization.jl)                         | Featurization schema       |
| `\cite{dataframes.jl}`            | [DataFrames.jl](https://github.com/JuliaData/DataFrames.jl)                   				  | Data structures            |
| `\cite{dftk.jl}`                  | [DFTK.jl](https://github.com/JuliaMolSim/DFTK.jl)                             				  | Electronic structure       |
| `\cite{differentialequations.jl}` | [DifferentialEquations.jl](https://github.com/SciML/DifferentialEquations.jl) 				  | Solver library             |
| `\cite{distributions.jl}`         | [Distributions.jl](https://github.com/JuliaStats/Distributions.jl)            				  | Probability                |
| `\cite{drwatson.jl}`              | [DrWatson.jl](https://github.com/JuliaDynamics/DrWatson.jl)                   				  | Workflow mangement         |
| `\cite{flux.jl}`                  | [Flux.jl](https://github.com/FluxML/Flux.jl)                                  				  | Deep learning framework    |
| `\cite{franklin.jl}`              | [Franklin.jl](https://github.com/tlienart/Franklin.jl)                        				  | Static websites            |
| `\cite{geometricflux.jl}`         | [GeometricFlux.jl](https://github.com/FluxML/GeometricFlux.jl)                                              | Graph neural networks      |
| `\cite{jump.jl}`                  | [JuMP.jl](https://github.com/jump-dev/JuMP.jl)                                				  | Optimization               |
| `\cite{latexify.jl}`              | [Latexify.jl](https://github.com/korsbo/Latexify.jl)                          				  | Latex representations      |
| `\cite{luxor.jl}`                 | [Luxor.jl](https://github.com/JuliaGraphics/Luxor.jl)                         				  | Drawing graphics           |
| `\cite{makie.jl}`                 | [Makie.jl](https://github.com/MakieOrg/Makie.jl)                              				  | Plotting and visualization |
| `\cite{measurements.jl}`          | [Measurements.jl](https://github.com/JuliaPhysics/Measurements.jl)            				  | Uncertainty propagation    |
| `\cite{metaheuristics.jl}`        | [Metaheuristics.jl](https://github.com/jmejia8/Metaheuristics.jl)             				  | Advanced optimization      |
| `\cite{mlj.jl}`                   | [MLJ.jl](https://github.com/alan-turing-institute/MLJ.jl)                     				  | Machine learning framework |
| `\cite{ohmyrepl.jl}`              | [OhMyREPL.jl](https://github.com/KristofferC/OhMyREPL.jl)                                                   | REPL enhancement           |
| `\cite{plots.jl}`                 | [Plots.jl](https://github.com/JuliaPlots/Plots.jl)                            				  | High-level plotting        |
| `\cite{pluto.jl}`                 | [Pluto.jl](https://github.com/fonsp/Pluto.jl)                                 				  | Notebook environment       |
| `\cite{pptx.jl}`                  | [PPTX.jl](https://github.com/ASML-Labs/PPTX.jl)                               				  | Presentation slides        |
| `\cite{revise.jl}`                | [Revise.jl](https://github.com/timholy/Revise.jl)                             				  | Julia REPL tool            |
| `\cite{scikitlearn.jl}`           | [ScikitLearn.jl](https://github.com/cstjean/ScikitLearn.jl)                   				  | API for scikit-learn[^1]   |
| `\cite{symbolics.jl}`             | [Symbolics.jl](https://github.com/JuliaSymbolics/Symbolics.jl)                				  | Symbolic programming       |
| `\cite{symbolicregression.jl}`    | [SymbolicRegression.jl](https://github.com/MilesCranmer/SymbolicRegression.jl)				  | Symbolic expression search |
| `\cite{taylorseries.jl}`          | [TaylorSeries.jl](https://github.com/JuliaDiff/TaylorSeries.jl)               				  | Polynomial expansion       |
| `\cite{turing.jl}`                | [Turing.jl](https://github.com/TuringLang/Turing.jl)                          				  | Probablistic programming   |
| `\cite{unitful.jl}`               | [Unitful.jl](https://github.com/PainterQubits/Unitful.jl)                     				  | Physical units             |
| `\cite{zygote.jl}`                | [Zygote.jl](https://github.com/FluxML/Zygote.jl)                              				  | Automatic differentiation  |

## Notes on Usage

- The `bib` entries contain unicode so its recommended to use `LuaLaTeX` or `XeLaTeX` when compiling.
- Many `\bibliographystyle` settings/styles won't handle `@misc` or `@software` entries very well (#1), therefore, I suggest using `BibLaTeX`.

Here is an example on [Overleaf](https://www.overleaf.com/read/xxtccjjzyygc).

### Cite all Packages

The following will cite all packages:

```latex
\cite{julia, chemistryfeaturization.jl, dataframes.jl, dftk.jl, differentialequations.jl, distributions.jl, drwatson.jl, flux.jl, franklin.jl, geometricflux.jl, jump.jl, latexify.jl, luxor.jl, makie.jl, measurements.jl, metaheuristics.jl, mlj.jl, ohmyrepl.jl, plots.jl, pluto.jl, pptx.jl, scikitlearn.jl, symbolics.jl, symbolicregression.jl, taylorseries.jl, turing.jl, unitful.jl, zygote.jl} 
```

## Standardization

There are four classes of `bibtex` entries used in [`juliapkgs.bib`](juliapkgs.bib): `@article`, `@software`, `@misc`, and `@inproceedings`. The use of `@misc` instead of `@software` is a bit arbitary.

The `juliapkgs.bib` file is checked and reformatted using the command/github-action:

```sh
biber --tool --validate-datamodel juliapkgs.bib
```

The github-action will create a [release](https://github.com/stefanbringuier/JuliaPkgCitations/releases) with the processed `.bib` file.

[^1]: Citing this package also would likely require citing the python library.

## Contributing

Pull request for updates/edits to existing entries or adding new entries are most certainly welcomed. Please be sure to use one of the classes indicated in the [standardization section](#standardization) above. For any major restructuring of the [`juliapkgs.bib`](juliapkgs.bib) or the [`README.md`](README.md) files, please open an issue first to discuss changes.
