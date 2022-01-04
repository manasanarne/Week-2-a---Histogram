#histogram.
Names <- c("Sreya","Manasa","Saswitha","Varsha","Pragna")
Rollno <- c("Y20CS176","Y20CS110","Y20CS135","Y20CS124","Y20CS093")
Gender <- c("Female","Female","Female","Female","Female")
Marks <-c(2,4,6,8,10)
Fee <-c(69400,57892,58903,69400,67390)
Section <-c("C","B","C","B","B")

rvrstudents <-data.frame(Names,Rollno,Gender,Marks,Fee,Section)
rvrstudents
write.csv(rvrstudents,"Rvr_Students.csv",row.names=F)

a <- read.csv("Rvr_Students.csv")



hist(rvrstudents$Marks,xlab="students names",ylab="students marks",xlim=c(1,5),ylim=c(1,5),col="blue",main="RVRJCCE",breaks=7)


OUTPUT:
> #histogram.
> Names <- c("Sreya","Manasa","Saswitha","Varsha","Pragna")
> Rollno <- c("Y20CS176","Y20CS110","Y20CS135","Y20CS124","Y20CS093")
> Gender <- c("Female","Female","Female","Female","Female")
> Marks <-c(2,4,6,8,10)
> Fee <-c(69400,57892,58903,69400,67390)
> Section <-c("C","B","C","B","B")
> rvrstudents <-data.frame(Names,Rollno,Gender,Marks,Fee,Section)
> rvrstudents
    Names    Rollno     Gender   Marks   Fee      Section
1   Sreya    Y20CS134   Female     2    69400       C
2   Manasa   Y20CS145   Female     4    57892       B
3 Saswitha   Y20CS149   Female     6    58903       C
4  Varsha    Y20CS127   Female     8    69400       B
5   Pragna   Y20CS129   Female    10    67390       B
> write.csv(rvrstudents,"Rvr_Students.csv",row.names=F)
> a <- read.csv("Rvr_Students.csv")
> hist(rvrstudents$Marks,xlab="students names",ylab="students marks",xlim=c(1,5),ylim=c(1,5),col="blue",main="RVRJCCE",breaks=7)
>
