###starting up


```{r}
install.packages("devtools")
devtools::install_github("sckott/cowsay")
library("cowsay")
```

```{r}
say('time')
```

 -------------- 
2015-08-16 02:51:22 
 --------------
    \
      \
        \
            |\___/|
          ==) ^Y^ (==
            \  ^  /
             )=*=(
            /     \
            |     |
           /| | | |\
           \| | |_|/\
      jgs  //_// ___/
               \_)
  

**Following are set of options available from the package.**


```{r}
#match.arg(by, c(choices = names(animals), "rms", "random")) : 
#'arg' should be one of “cow”, “chicken”, “clippy”, “poop”, “bigcat”, “ant”,
#“pumpkin”, “ghost”, 
#“spider”, “rabbit”, “pig”, “snowman”, “frog”, “hypnotoad”, 
#“facecat”, “behindcat”, “cat”, “trilobite”, “shark”, “buffalo”, “smallcat”, “yoda”,
#“endlesshorse”, “rms”, “random”
```

```{r}
say("boo!", "ghost")
```

 ----- 
 boo! 
 ------ 
    \   
     \
     .-.
    (o o)
    | O \
     \   \
      `~~~' [nosig]
      

```{r}
say("it's caturday", "bigcat")
```
----- 
 it's caturday 
 ------ 
    \   
     \
                \`*-.
                 )  _`-.
                .  : `. .
                : _   '  \
                ; *` _.   `*-._
                `-.-'          `-.
                  ;       `       `.
                  :.       .       \
                  .\  .   :   .-'   .
                  '  `+.;  ;  '      :
                  :  '  |    ;       ;-.
                  ; '   : :`-:     _.`* ;
               .*' /  .*' ; .*`- +'  `*'
     [bug]     `*-*   `*-*  `*-*



- Using piping

```{r}
library("magrittr")
"Game over" %>% say('spider')
```

 ----- 
 Game over 
 ------ 
    \   
     \
              |
              |
              |
             __
          | /  \ |
         \_\\  //_/
          .'/()\'.
           \\  //  [nosig]






```{r}
say('Fun starts here, because winters !', by='snowman')
```
 ----- 
 Fun starts here, because winters ! 
 ------ 
    \   
     \
     _[_]_
      (")
  >--( : )--<
    (__:__) [nosig]



```{r}
say(fortune='random', by="clippy")
```


 ----- 
 Frank Harrell: Here is an easy approach that will yield results only slightly less valid than one actually using the response variable:
  x <- data.frame(x1, x2, x3, x4, ..., other potential predictors)
  x[ , sample(ncol(x))]
Andy Liaw: Hmm... Shouldn't that be something like:
  x[, sample(ncol(x), ceiling(ncol(x) * runif(1)))]
 Frank Harrell and Andy Liaw
 about alternative strategies for stepwise regression and 'random parsimony'
 R-help
 May 2005 
 ------ 
    \   
     \
   __
   / \
   | |
   @ @
  || ||
  || ||
  |\_/|
  \___/ GB
