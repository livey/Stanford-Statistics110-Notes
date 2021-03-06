#Normal distribution 

Z~N(0,1), E(Z)=0, Var(Z)=E(Z^2)=1; 
E(Z^3)=0; 
-Z ~ N(0,1) (symmetry). 

Let X=\mu+\sigma*Z, \mu\in R (mean location), \sigma>0 (standard derivation,scale) 
Then we say X~N(\mu,\sigma^2) 
E(X)= \mu; Var(X)= Var(\mu+\sigma*Z)=
[Var(X)=E(X-EX)^2]=EX^2-E^2X 
Var(X+c)=Var(X) , Var(cX)= c^2*Var(X)  ]

Var(X+Y) !=Var(X)+Var(Y) (in general, equal if X,Y are independent) 
Var(X+X) = Var(2X)=4Var(X). 

So V(\mu+\sigma*Z)=\sigma^2*Var(Z) =\sigma^2; 

Z=(X-\mu)/\sigma Z~N(0,1) 

Find PDF of X~N(\mu,\sigma^2) ?
CDF:
P(X<=x) =P((X-\mu)/\sigma< (x-\mu)/\sigma)) =\Phi((x-\mu)/\sigma) 
PDF: 
\partial \Phi(.)= 

-X = -\mu - \sigma*Z so -X ~ N(-\mu,\sigma^2). 
Later we'll show if X_j ~ N(\mu_j,\sigma_j^2) independent, X_1+X_2 ~ N(\mu_1+\mu_2,\sigma_1^2+\sigma_2^2) 
X1-X2 ~ N(\mu_1-\mu_2, \sigma_^2+\sigma_2^2) 

68-95-99.7% Rule X~N(\mu,\sigma^2) 
P(|X-\mu|<\sigma)\approx 0.68 
P(|X-\mu|<2\sigma)\approx 0.95 
P(|X-\mu|<3\sigma)\approx 0.997

#The variance of Poisson 
X \in {0,1,2....} and P_0,P_1,P_2,....
X^2 \in {0, 1,4,9,...} 
E(X^2)=\sum x^2*P(X=x)

X~ Pois(\lambda) 
E(X^2) = \sum_{k=0} k^2 \lambda^k/k! e^{-\lambda} = 

\sum_k \lamda^k/k! = e^\lambda 

\sum_k k\lambda^{k-1}/k!  = e^\lambda 
multiply \lambda on both sides 
\lambda \sum_k k*\lambda^{k-1}/k! = \lambda e^\lambda 
\sum_k k\lambda^k/k!=\lambda*e^\lambda 

Var(X)=\lambda^2+\lambda-\lambda^2 = \lambda 

##Binomial Variance 
X~Bin(n,p) use if X, Y are independent, then V(X+Y) =Var(X)+Var(Y) Binomail is n independent Bernoulli trials 
Var(X)=Var(X1)+Var(X2)+...+Var(Xn) = npq 
or 
X= I1+I2+...In
X^2=I1^2+I2^2+..+In^2+2I1I2+2I1I3+..+2In-1*In 
E(X^2) = nE(I1^2) + 2*(n,2)E(I1I2) (for symmetry property) 
       =np + n(n-1)p^2 =np.
So, 
Var(X)=E(X^2)-E(X)^2=np-(np)^2 = npq. 

##Prove LOTUS for discrete sample space 
E(g(x))= \sum g(x)P(X=x) 
  
\sum_x g(x)P(X=x) = \sum_s g(X(s))P({s}) 
\sum_x \sum_{s:X(s)=x} g(X(s))P({s}) = \sum_x g(x) \sum_{s:X(s)=x} P({s})=\sum_x g(x) P(X=x) 





