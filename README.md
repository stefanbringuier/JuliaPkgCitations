# Julia Pkg Citations

This repo provides the file [`juliapkgs.bib`](juliapkgs.bib) (**WIP**) that contains several entries for many popular [Julia](https://julialang.org/) packages. The repo was inspired by [Miles Cranmer](https://github.com/MilesCranmer/python_citations) python repo.

> Note that if a peer-reviewed publication is available for a given Julia package, this is choosen as the default work to cite.

## List of citation keys

All keys use lowercase for the package name and contain the `.jl` extension. The year and author have been excluded.

| Citation Key | Package | Use |
| :-- | :-- | :-- |
| `\cite{julia}` | [Julia Language](https://github.com/JuliaLang/julia) | Programming Language |
| `\cite{plots.jl}` | [Plots.jl](https://github.com/JuliaPlots/Plots.jl) | High-level plotting |
| `\cite{pluto.jl}` | [Pluto.jl](https://github.com/fonsp/Pluto.jl)| Notebook environment |
| `\cite{flux.jl}` | [Flux.jl](https://github.com/FluxML/Flux.jl) | Deep learning framework |
| `\cite{jump.jl}` | [JuMP.jl](https://github.com/jump-dev/JuMP.jl) | Optimization |
| `\cite{turing.jl}` | [Turing.jl](https://github.com/TuringLang/Turing.jl)| Probablistic programming |
| `\cite{dataframes.jl}` | [DataFrames.jl](https://github.com/JuliaData/DataFrames.jl)| Data structures |
| `\cite{distributions.jl}` | [Distributions.jl](https://github.com/JuliaStats/Distributions.jl) | Probability |
| `\cite{franklin.jl}` | [Franklin.jl](https://github.com/tlienart/Franklin.jl)| Static websites |
| `\cite{makie.jl}` | [Makie.jl](https://github.com/MakieOrg/Makie.jl)| Plotting and visualization |
| `\cite{symbolics.jl}` | [Symbolics.jl](https://github.com/JuliaSymbolics/Symbolics.jl) | Symbolic programming |
| `\cite{mlj.jl}` | [MLJ.jl](https://github.com/alan-turing-institute/MLJ.jl) | Machine learning framework |
| `\cite{revise.jl}` | [Revise.jl](https://github.com/timholy/Revise.jl) | Julia REPL tool |
| `\cite{differentialequations.jl}` | [DifferentialEquations.jl](https://github.com/SciML/DifferentialEquations.jl) | Solver library |
| `\cite{zygote.jl}` | [Zygote.jl](https://github.com/FluxML/Zygote.jl) | Automatic differentiation|
| `\cite{drwatson.jl}` | [DrWatson.jl](https://github.com/JuliaDynamics/DrWatson.jl) | Workflow mangement |
| `\cite{scikitlearn.jl}` | [ScikitLearn.jl](https://github.com/cstjean/ScikitLearn.jl) | API for scikit-learn[^1]|
| `\cite{luxor.jl}` | [Luxor.jl](https://github.com/JuliaGraphics/Luxor.jl) | Drawing graphics |
| `\cite{latexify.jl}` | [Latexify.jl](https://github.com/korsbo/Latexify.jl) | Latex representations |
| `\cite{measurements.jl}` | [Measurements.jl](https://github.com/JuliaPhysics/Measurements.jl) | Uncertainty propagation |

## Cite all Packages

The following will cite all packages:

```latex
\cite{julia, plots.jl, pluto.jl, flux.jl, jump.jl, turing.jl, dataframes.jl, distributions.jl, franklin.jl, makie.jl, symbolics.jl, mlj.jl, differentialequations.jl, zygote.jl, drwatson.jl, scikitlearn.jl, luxor.jl, latexify.jl, measurements.jl}
```

## Standardization

The `juliapkgs.bib` file is checked using the command/github-action:
```sh
biber --tool --validate-datamodel juliapkgs.bib
```

The github-action will create a release with the processed `.bib` file.



[^1]: Citing this package also would likely require citing the python library.