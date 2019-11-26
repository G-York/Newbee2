# 哑铃图和多重折线图 #

![image1](https://github.com/G-York/Newbee2/blob/master/%E8%B4%9F%E5%88%91%E4%BA%8B%E8%B4%A3%E4%BB%BB%E5%B9%B4%E9%BE%84.png)

```
library(ggplot2)
library(ggalt)
lawage <- read.csv("lawage.csv")
lawage$country <- factor(lawage$country)
theme_set(theme_classic())
gg <- ggplot(lawage,aes(x=agebegin,xend=agefull,
y=country,group=country))+
geom_dumbbell(color="#bdbdbe",
size=0.75,size_x=2,size_xend = 2,
colour_x = "#4fc3f7",colour_xend = "#01579b")+
+ labs(x=NULL,y=NULL,"lowest/full age for criminal responsibility",
subtitle = "EU Countries and China")+
+ theme(plot.title = element_text(hjust=0.5, family="kai"),
plot.background=element_rect(fill="#ffffff"),
panel.background=element_rect(fill="#ffffff"),
panel.grid.minor=element_line(colour = "#eeeeee"),
panel.grid.major.y=element_line(colour"#eeeeee"),
panel.grid.major.x=element_line(),
axis.ticks=element_blank(),
legend.position="top",
panel.border=element_blank())
plot(gg)
```


![image2](https://github.com/G-York/Newbee2/blob/master/%E5%B7%A5%E8%AF%BB%E5%AD%A6%E6%A0%A1.png)
```
library(“ggplot2”)
library("scales")
read.csv("rate.csv")
rate <- read.csv("rate.csv")
rate$year <- factor(rate$year)
gg2 <- ggplot(rate,aes(x=year,y=rates,colour=cases,group=cases))
+geom_line()+scale_y_continuous(label=percent,
limits = c(0,0.5))+geom_point(size=2) + 
scale_fill_manual(values=c("#87473c","#d65641"))+
scale_colour_manual(values=c("#87473c","#d65641"))+
theme(panel.grid.major = element_blank(),
panel.grid.minor = element_blank())+
geom_text(aes(label=percent(rates)),vjust=-1.5)+
ggtitle("ratios of non-arrest/non-prosecution cases in juvenile crimes")+
labs(x=NULL,y=NULL)
plot(gg2)
```


