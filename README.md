**Here is some math!**

```math
\sqrt{3}
```

##Payload #1 - Xss - (doesn't fire - check later)

//$\(\newtagform{}{okays}\)$

##Payload #2 -- inline mathjax w/ ```math ref
```math
<script type="math/tex; mode=display">
  \sum_{n=1}^\infty {1\over n^2} = {\pi^2\over 6}
```

##Payload #3 - \newtagform option -- try this once we see how newtagform 

```math
\newtagform{}\sqrt{{\bf R}}
```

##Payload 4- Mathjax scripts

```math
\newtagform\sqrt_\sum{{\bf R}}
```

##New stuff
$$a := x^2-y^3 \tag{hi}\label{evil}$$

#1
$$a+y^3\stackrel{\eqref{evil}=x^2$$

#2
$\ref{evil}$


