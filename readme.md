# JULIA WORKSHOP
2022 07

# Tutorial
## sandbox
+ VSCODE
+ GIT
  + https://www.youtube.com/watch?v=F2DBSH2VoHQ
  
## Referencias
+ The Fast Track to Julia, a quick and dirty overview > Juliahttps://juliadocs.github.io/Julia-Cheat-Sheet/
+ Data Science using Julia > https://juliadatascience.io/
+ Setting Up VS Code for Julia | Talk Julia #11 > https://www.youtube.com/watch?v=KesuPOlBB_o
+ JULIA BASIC, INT, ADVANCE tutorials by DJ's Office Hours > https://www.youtube.com/watch?v=xxOUOkhHhTU&list=PLOU8LxhyFylLYpkd3WgEmblTUiwrZ719y&index=4
+ julia basics cheat sheeet | datacamp 2022 > https://datacamp.com/cheat-sheet/julia-basics-cheat-sheet
+ video: "Why Julia?" A high level description of the features and benefits of programming in Julia https://www.youtube.com/watch?v=x4oi0IKf52w


Ver los paquetes
```
pkg status
```

```
  [6e4b80f9] BenchmarkTools v1.3.1
  [a93c6f00] DataFrames v1.3.4
  [e9467ef8] GLMakie v0.5.5
  [c91e804a] Gadfly v1.3.4
  [7073ff75] IJulia v1.23.2
  [6218d12a] ImageMagick v1.2.2
  [b964fa9f] LaTeXStrings v1.3.0
  [eadc2687] Pandas v1.5.3
  [91a5bcdd] Plots v1.25.7
  [c3e4b0f8] Pluto v0.19.9
  [7f904dfe] PlutoUI v0.7.39
  [d330b81b] PyPlot v2.10.0
  [f3b207a7] StatsPlots v0.14.33
  [24249f21] SymPy v1.1.3
  [bd369af6] Tables v1.7.0
  [37e2e46d] LinearAlgebra
```
Para usar los paquetes 
```
using Plots, LinearAlgebra, LaTeXStrings, (otros)
```
## Actualizar

```
julia> ]
pkg> add UpdateJulia
# Presionar ']' para habilitar el pkg mode en el REPL(read–eval–print-loop)
# Presionar 'delete' para salir  
julia> using UpdateJulia
julia> update_julia()
```
to update packages
```
pkg> up
```

Después de actualizar hacer esto:
salir de julia
> Iniciar julia
> versioninfo()
```
versioninfo()
Julia Version 1.9.1
Commit 147bdf428c (2023-06-07 08:27 UTC)
Platform Info:
  OS: Windows (x86_64-w64-mingw32)
  CPU: 16 × AMD Ryzen 9 5900HS with Radeon Graphics
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-14.0.6 (ORCJIT, znver3)
  Threads: 1 on 16 virtual cores
  ```

```
julia> using Pkg
julia> Pkg.update()
julia> Pkg.build("IJulia")
```
