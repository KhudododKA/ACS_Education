# Data_Incubator_Project
setwd(dir ="dir")
list.filenames<-list.files(pattern = ".csv")
d<-list()
for (i in 1:length(list.filenames))
{
  d[[i]]<-read.csv(list.filenames[i],header = TRUE,sep = ",")
}
names(d)<-list.filenames
