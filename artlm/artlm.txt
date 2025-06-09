# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Approximate Randomization Tests with a Small Number of Clusters Use artlm (rART) With (In) R Software
install.packages("remotes")
remotes::install_github("mwt/rART")
library("rART")
artlm = read.csv("https://raw.githubusercontent.com/timbulwidodostp/artlm/main/artlm/artlm.csv",sep = ";")
# Estimation Approximate Randomization Tests with a Small Number of Clusters Use artlm (rART) With (In) R Software
artlm <- artlm(y ~ x1 + x2, cluster = group, data = artlm)
ARTHypothesis <- ARTHypothesis(artlm, "x1 = x2")
summary(artlm)
ARTHypothesis
# Approximate Randomization Tests with a Small Number of Clusters Use artlm (rART) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished