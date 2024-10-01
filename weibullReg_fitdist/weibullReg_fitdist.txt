# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Weibull Regression for Survival Data And Fitting of the distribution weibull by maximum likelihood Use WeibullReg And fitdist With (In) R Software
install.packages("SurvRegCensCov")
install.packages("fitdistrplus")
library("SurvRegCensCov")
library("fitdistrplus")
weibullReg_fitdist = read.csv("https://raw.githubusercontent.com/timbulwidodostp/weibullReg_fitdist/main/weibullReg_fitdist/weibullReg_fitdist.csv",sep = ";")
# Estimation Weibull Regression for Survival Data And Fitting of the distribution weibull by maximum likelihood Use WeibullReg And fitdist With (In) R Software
WeibullReg <- WeibullReg(Surv(time, death) ~ factor(stage) + age, data = weibullReg_fitdist)
print(WeibullReg)
fitdist <- fitdist(weibullReg_fitdist$time, "weibull")
summary(fitdist) 
# Weibull Regression for Survival Data And Fitting of the distribution weibull by maximum likelihood Use WeibullReg And fitdist With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished