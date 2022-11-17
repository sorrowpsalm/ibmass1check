setwd("D:")
getwd()
sampleData = read.csv("cbb.csv")
head(sampleData)

summary(sampleData)
summary(sampleData$W)
hist.default(sampleData$W,col='gray')
table(sampleData$W)
plot(table(sampleData$W))

plot(sampleData$G~sampleData$W,col='blue')
t.test(sampleData$G)