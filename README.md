# OnlineStats

Online algorithms for statistics.  The driving function in this package is  

```update!(obj, newdata)```  
- `obj`: subtype of `OnlineStat`  
- `newdata`: new observations


## Types 
Each type defined in OnlineStats contains the fields  

- `<<estimate>>`: Vector of saved estimates
- `n`: number of observations used (display with `n_obs(obj)`)
- `nb`: number of batches used (display with `n_batches(obj)`)

Other fields will be used to store sufficient statistics for online updates.

## Full Documentation
Documentation generated using [Docile.jl](https://github.com/MichaelHatherly/Docile.jl), [Lexicon.jl](https://github.com/MichaelHatherly/Lexicon.jl), and [MkDocs](http://www.mkdocs.org) is available [here](http://joshday.github.io/OnlineStats.jl/)

 

## Updating API documentation
Run the following:
```
julia> using Lexicon
julia> include("src/OnlineStats.jl")
julia> Lexicon.save("docs/OnlineStats.md", OnlineStats)
```

Make webpage changes only in **master**
```
mkdocs build  
```

Push website from **master/site** straight to **gh-pages**
```
git push origin `git subtree split --prefix site master`:gh-pages --force
```

