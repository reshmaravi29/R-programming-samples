# R-programming-samples
#R program that tests the law of large numbers
#Problem:Test the law of large numbers for N randomly distributed normal numbers with mean=0,std dev=1,Find how many of these 
#numbers fall between 1 and -1 .Divide this answer by N.
#Solution
N=100
counter<-i
for(i in rnorm(100)){
  if (counter>-1 & counter<1){
    counter<-counter+1
  }
}
answer<-counter/N
answer
