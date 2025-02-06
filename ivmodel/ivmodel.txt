# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Fitting instrumental variables (IV) models Use ivmodel With (In) R Software
install.packages("ivmodel")
library("ivmodel")
ivmodel = read.csv("https://raw.githubusercontent.com/timbulwidodostp/ivmodel/main/ivmodel/ivmodel.csv",sep = ";")
# Estimation Fitting instrumental variables (IV) models Use ivmodel With (In) R Software
Y=ivmodel[,"lwage"]
D=ivmodel[,"educ"]
Z=ivmodel[,"nearc4"]
Y=card.data[,"lwage"]
D=card.data[,"educ"]
Z=card.data[,"nearc4"]
Xname=c("exper", "expersq", "black", "south", "smsa", "reg661","reg662", "reg663", "reg664", "reg665", "reg666", "reg667", "reg668", "smsa66")
X=ivmodel[,Xname]
ivmodel = ivmodel(Y=Y,D=D,Z=Z,X=X)
ivmodel
# Fitting instrumental variables (IV) models Use ivmodel With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished