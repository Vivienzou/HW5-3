HW5-3
=====
# (b) Crack my RSA cryptosystem by factoring n. HINT: The "factor" command will get you nowhere. 
I'll just tell you now that n=p*q with p and q a little "too close for comfort".

n = 465425223039311122698944982674100700648607800945086109507022243989832434235392755390925153223240
7850265642079868425916328810273416481567992145162141358151

q = n**0.5                    #start with sqrt(n), since factors are closed enough

int (q)                       #set q to integer so we can start rolling

q =  next_probable_prime(q)   #comfortable for rolling test below

p = n/q                       

int(p)

if (n == p*q)==True :
  print p
  print q

keep rolling this test until get p = 68222080226222296181917368518534332259513625527062166102114730123514248558349

q=68222080226222296181917368518534332259513625527062166102114730123514248558499
