# OBGYN-Data-1-




```{r setup, packages}
install.packages("tidyverse")
library(tidyverse)
library(ggplot2)
library(dplyr)
```

```{r term and viability}
OBGYN_HN %>% 
  group_by(term_status, viable) %>% 
  count()
```

```{r term and c-section}
OBGYN_HN %>% 
  group_by(term_status, vaginal_status) %>% 
  count()
```

```{r}
OBGYN_HN %>% 
  group_by(vaginal_status) %>% 
  count()
```

```{r}
OBGYN_HN %>% 
  group_by(vaginal_status, support) %>% 
  count()
```



```{r}
OBGYN_HN %>% 
  group_by(support) %>% 
  count()
```

```{r}
OBGYN_HN %>% 
  group_by(complications) %>% 
  count()
```

```{r}
OBGYN_HN %>% 
  group_by(vaginal_status, complications) %>% 
  count()
```




