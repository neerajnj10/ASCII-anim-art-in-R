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
 Pavel Khomski: How can I specify the random part in the GLMM-call (of the lme4 library) for compound matrices just in the the same way as they defined in the lme-Call (of the nlme library).
Martin Maechler: ''twice in such a short paragraph -- yikes !!'' ... I'm getting convulsive...
 Pavel Khomski and Martin Maechler
 R-help
 February 2005 
 ------ 
    \   
     \
                  ___
               ___)__|_
          .-*'          '*-,
         /      /|   |\     \
        ;      /_|   |_\     ;
        ;   |\           /|  ;
        ;   | ''--...--'' |  ;
         \  ''---.....--''  /
          ''*-.,_______,.-*'  [nosig]
