# Trimmed-mean  
#This code finds out the trimmed mean of a list of numbers


from scipy import stats
Estimates=[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26]
Estimates.sort()
print(Estimates)
tv=int(0.1*len(Estimates))
Estimates=Estimates[tv:]
print(Estimates)
Estimates=Estimates[:len(Estimates)-tv]
print(Estimates)
Sumation=sum(Estimates)
print(Sumation)
length=len(Estimates)
print(length)
mean=(Sumation/length)
print("mean value=",mean)
a=stats.trim_mean(Estimates,0.1)
print(a)
