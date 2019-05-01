# Bitcoin Futures
## Basic Introduction of Bitcoin Futures
Bitcoin futures are futures contracts that speculate on the price of Bitcoin without participants actually having to own Bitcoin. Entities that participate in Bitcoin futures are essentially making a bet on the price of Bitcoin over a specified period. Bitcoin futures work the same way as any futures contract on a traditional financial asset. Investors can either go long on Bitcoin — expecting the price to increase — or short it, mitigating potential losses if they actually own some Bitcoin.

In December 2017 trading in futures contracts on Bitcoins commenced on the Chicago Mercantile Exchange and the Chicago Board Options Exchange. On the December 1st, both exchanges announced a Bitcoin futures contract. Bitcoin futures opened for trading on the CBOE December 10th, 2017. This is one of the biggest milestones for bitcoin since it emerged in the wake of the 2008-2009 financial crisis. CBOE was soon joined by CME Group as it launched bitcoin futures contracts on December 18th, 2017.

| | CBOE | CME |
|:------:|:------:|:------:|
|Listing Date|December 10, 2017|Effective December 17, 2017 for trade date of December 18, 2017|
|Ticker|XBT|BTC|
|Contract Unit|Equal to 1 bitcoin|Equal to 5 bitcoins|
|Description|Cboe bitcoin (USD) futures are cash-settled futures contracts that are based on the Gemini Exchange auction price for bitcoin in U.S. dollars.|CME Group's Bitcoin futures will be cash-settled, based on the CME CF Bitcoin Reference Rate (BRR) which serves as a once-a-day reference rate of the U.S. dollar price of bitcoin.|
|Pricing|USD|USD|
|Settlement|The final settlement value will be the auction price for bitcoin in U.S. dollars determined at 4:00 p.m. Eastern Time (2100 GMT) on the final settlement date by the Gemini Exchange.|The contract will be prices off of the CME CF Bitcoin Reference Rate (BRR) which has been designed around the IOSCO Principles for Financial Benchmarks. Bitstamp, GDAX, itBit and Kraken are the constituent exchanges that currently contribute the pricing data for calculating the BRR.|
|Trading Hours|Regular: 8:30 a.m. to 3:15 p.m.(Mon), 8:30 a.m. to 3:15 p.m. (Tue-Fri) Extended: 5:00 p.m. (Sun) to 8:30 a.m. 3:30 p.m. (previous day) to 8:30 a.m. (Tue-Fri)|CME Globex and CME ClearPort: Sun-Fri 6:00 p.m. to 5:00 p.m. (5:00 p.m. to 4:00 p.m. CT) with one-hour break beginning at 5:00 p.m. (4:00 p.m. CT)|
|Margin Rates|40%|35%|
|Clearing|Options Clearing Corporation|CME ClearPort|
|Contract Expirations|Initially the exchange will list three near-term serial months Eventually, CFE may list for trading up to four near-term expiration weekly contracts, three near-term serial months, and three months on the March Quarterly Cycle|Nearest 2 months in the March Quarterly cycle (Mar, Jun, Sep, Dec) plus the nearest two “serial” months not in the March Quarterly Cycle|

For investors looking to speculate on the price of Bitcoin without having to actually own any directly, Bitcoin futures provide a viable, regulated means to do so effectively. Further, futures can help hedge against risk against the volatile price fluctuations of Bitcoin. Bitcoin futures will bring much-needed transparency, greater liquidity and efficient price discovery to the ecosystem.

Bitcoin futures provide several advantages for investors. First, they are traded on regulated exchanges, making the process much more familiar and comfortable for mainstream and institutional investors who may not want to deal directly with cryptocurrency exchanges. Second, the contracts allow for speculation on the underlying price of the asset without having to go through the process of properly storing bitcoins, which is a high barrier to entry for many people unfamiliar with how Bitcoin works. Third, by granting Bitcoin more exposure to investors, more liquidity is added to the market. Finally, futures trading can lead to less volatility of Bitcoin’s price in the long-term and enable investors to protect themselves from adverse price swings.


## Platforms Offering Bitcoin Futures Trading

## Method
### Basic idea
Dynamic Conditional Correlation (DCC-) GARCH,one of the multivariate GARCH models, was introduced by Engle and Sheppard in 2001.
GARCH is the good model to successfully capture the volatility clustreing and predicting future volatilities. Multivariate GARCH is the extend from univariate GARCH.<br>
<br>
The basic idea to extend from univariate to multivariate is as following:
* In financial econometrics and management understanding, predicting the dependence in the comovements of asset returns is important. For example, asset pricing depends on the covariance of the assets in a portfolio. Hence it is important to consider the comovements in the portfolio. <br>
* Financial volatilities move together more or less closely over time across assets and markets. <br>
* Recognizing this feature through a multivariate model should lead to more relevant empirical models than working with separate univariate models. <br>
* In financial applications, extending from univariate to multivariate modelling opens the door to better decision tools in various areas such as asset pricing models, portfolio selection, hedging, and Value-at-Risk forecasts. <br>
  
The different specifications of MGARCH models can be divided into four categories as suggested in: <br>
1. `Models of the conditional covariance matrix`: In this class the conditional covariance matrices, Ht, are modelled directly. This class includes the VEC and BEKK models. These models were among the first parametric MGARCH models. <br>
2. `Factor models`: The idea of factor models comes from economic theory. In this class the conditional covariance matrices are motivated by parsimony. The process at is assumed to be generated by a (small) number of unobserved heteroskedastic factors, hence these models are called factor models. These factors can be studied and one may make assumptions that some characteristics of the data is captured, similar as for principal component analysis. This approach has the advantage that it reduces the dimensionality of the problem when the number of factors relative to the dimension of the return vector at is small. <br>
3. `Models of conditional variances and correlations`: The models in this class are built on the idea of modelling the conditional variances and correlations instead of straightforward modelling the conditional covariance matrix. <br>
4. `Nonparametric and semiparametric approaches`: Models in this class form an alternative to parametric estimation of the conditional covariance structure. The advantage of these models is that they do not impose a particular structure (that can be misspecified) on the data.<br>
  
The DCC-GARCH model belongs to the category 3 above.
### Models
Suppose we have returns,_a<sub>t</sub>_, from _n_ assets with expected value 0 and covariance matrix _H<sub>t</sub>_. The the Dynamic Conditional Correlation GARCH Model is defined as:<br>
 _r<sub>t</sub>_ = _μ<sub>t</sub>_ + _a<sub>t</sub>_  <br> 
              
 _a<sub>t</sub>_ = _H<sub>t</sub><sup>1/2</sup>_ * _z<sub>t</sub>_  <br>
               
 _H<sub>t</sub>_ = _D<sub>t</sub>_ * _R<sub>t</sub>_ * _D<sub>t</sub>_  <br>
      
The notation is as following: <br>
_r<sub>t</sub>_:  n * 1 vector which represents the returns of  _n_ assets at time _t_ <br>
_a<sub>t</sub>_:  n * 1 vector which is the mean-corrected returns of  _n_ assets at time _t_ <br>
_μ<sub>t</sub>_:  n * 1 vector which is the ecpected value of the conditional _r<sub>t</sub>_ <br>
_H<sub>t</sub>_:  n * n conditional variances of _a<sub>t</sub>_ <br>
_D<sub>t</sub>_:  n * n diagonal matrix of conditional standard deviations of _a<sub>t</sub>_ at time _t_ <br>
_R<sub>t</sub>_:  n * n diagnoalcorrelation matrix of _a<sub>t</sub>_ at time _t_ <br>
_z<sub>t</sub>_:  n * 1 vector of i.i.d errors <br>

    
h<sub>it</sub>= ω<sub>i</sub>+∑α<sub>iq</sub>a<sub>i,t-q</sub><sup>2</sup>+∑β<sub>ip</sub>h<sub>i,t-p</sub>
                  
 
## Emprical Analysis
### Statistical View of Data
|Cryptocuurency return| Min|1st Qu|Median|Mean|3rd Qu|Max|skewness|kurtosis|
|:------:|:------:|:------:|:------:|:------:|:------:|:------:|:------:|:------:|
|Bitcoin|-0.207530|-0.010107|0.002263|0.002162|0.017238|0.225119|-0.2214035|4.964624|
|Ether|-1.3065294|-0.0260256|-0.0007707|0.0030592|0.0298530|0.4101490|-3.427667|66.89897|
|Litecoin|-0.395151|-0.017611|0.000000|0.002279|0.018920|0.510348|1.271129|12.16704|
        
As it shows in the table, we can conclude that Bitcoin's return and Ether's return are left-skewed with negative skewness. On the contratry, Litecoin's return has the right-skewed distribution. All of them own the heavy-tailed distributions. <br>
### Unit Root Test
* Bitcoin return unit root test <br>
![bitcoinreturnunitroottest](https://github.com/WangJiajia-0901/PHBS_BlockChain_2018/blob/master/Image/adfbitcoinreturn.bmp) <br>
`Augmented Dickey-Fuller Test` <br>
Dickey-Fuller = -9.7392, Lag order = 11, p-value = 0.01 <br>
*Alternative hypothesis: stationary* <br>
    
* Ether return unit root test <br>
![etherreturnunitroottest](https://github.com/WangJiajia-0901/PHBS_BlockChain_2018/blob/master/Image/adfetherreturn.bmp) <br>
`Augmented Dickey-Fuller Test` <br>
Dickey-Fuller = -9.8653, Lag order = 11, p-value = 0.01 <br>
*Alternative hypothesis: stationary* <br>
   
* Litecoin return unit root test <br>
![litecoinreturnunitroottest](https://github.com/WangJiajia-0901/PHBS_BlockChain_2018/blob/master/Image/adflitecoinreturn.bmp) <br>
`Augmented Dickey-Fuller Test` <br>
Dickey-Fuller = -10.15, Lag order = 11, p-value = 0.01 <br>
*Alternative hypothesis: stationary* <br>
            
All the ADF tests present the small p-value rejecting the null hypothesis of unit root which means that all the three cryptocurrencies' returns are stationary. <br> 

### Arch Test
* Bitcoin return Arch Test <br>
`ARCH LM Test` <br>
Chi-squared = 110.91, df = 12, p-value < 2.2e-16 <br>
*Null hypothesis: no ARCH effects* <br>
   
* Ether return Arch Test <br>
` ARCH LM Test` <br>
Chi-squared = 135.77, df = 12, p-value < 2.2e-16 <br>
*Null hypothesis: no ARCH effects* <br>
    
* Litecoin return Arch Test <br>
`ARCH LM Test` <br>
Chi-squared = 76.184, df = 12, p-value = 2.193e-11 <br>
*Null hypothesis: no ARCH effects* <br>

All the ARCH-LM tests reach the small p-value which means that there are truly ARCH effects in returns of cryptocurrencies.

### Pearson correlation 
| |Bitcoin return| Ether| Litecoin|
|:------:|:------:|:------:|:------:|
|Bitcoin| 1.0000000|0.9001795|0.9400632|
|Ether| 0.9001795|1.0000000|0.9356845|
|Litecoin|0.9400632|0.9356845|1.0000000|
              
The Pearson correlation matrix further shows that the significantly positive correlation in the three crptocurrencies with  nearly 1 correlation coefficients. 

### Multivariate GARCH Fit
Now, estimating the three bivariate ARMA(1,1)-DCC-GARCH(1,1) models. <br>
#### Bitcoin and Ether
| |Estimated|Std.Error|t value| p value|
|:------:|:------:|:------:|:------:|:------:|
|bitcoinomega |7.476703  | 10.242742 | 0.72995 |0.465420|
|bitcoinalpha1 |0.080691 |0.031054 |  2.59845 | 0.009365 |
|bitcoinbeta1|0.918309|0.044749|20.52117|0.000000 |
|etheromega|0.005664|0.003738|1.51496|0.129783 |
|etheralpha1|0.169568|0.024274|6.98553|0.000000 |
|etherbeta1|0.829432|0.031814|26.07168|0.000000 |
|Jointdcca1|0.089803|0.011608|7.73622|0.000000 |
|Jointdccb1|0.905648|0.012416|72.94382|0.000000 |
|Jointmshape|4.513015|0.255703|17.64946|0.000000 |
                          
|Information criteria|value|
|:------:|:------:|
|Akaike    |   16.417|
|Bayes    |    16.479|
|Shibata  |    16.416|
|Hannan-Quinn| 16.440|
               
                  
The the coefficients are signicant except the omega of bitcoin and omega of ether which means that there truly exists the dynamic correlations in Bitcoin return and Ether return.
              
![2](https://github.com/WangJiajia-0901/PHBS_BlockChain_2018/blob/master/Image/be.png) <br>
        
From the dynamic conditional correlation plot between Bitcoin return and Ether return, we can further conclude that they are co-related most of time, especially after mid-2017. <br>

#### Bitcoin and Litecoin
| |Estimated|Std.Error|t value| p value|
|:------:|:------:|:------:|:------:|:------:|
|bitcoinomega   | 6.012333   | 4.151115 |  1.4484 | 0.14752|
|bitcoinalpha1 |  0.148902  |  0.026379  | 5.6448 | 0.00000|
|bitcoin].beta1  |  0.850098   | 0.042624 | 19.9442 | 0.00000|
|litecoinomega  | 0.002274 |   0.001860 |  1.2227 | 0.22146|
|litecoinalpha1 | 0.089735 |   0.017098  | 5.2482|  0.00000|
|litecoin].beta1  | 0.909265 |   0.024931 | 36.4718 | 0.00000|
|Jointdcca1    |   0.101047  |  0.016398   |6.1621 | 0.00000|
|Jointdccb1    |   0.892507  |  0.017998 | 49.5883 | 0.00000|
|Jointmshape  |    4.609205  |  0.307277 | 15.0001 | 0.00000|
                    
|Information criteria|value|
|:------:|:------:|
|Akaike    |   14.074|
|Bayes    |    14.136|
|Shibata  |    14.074|
|Hannan-Quinn| 14.098|
                 
The the coefficients are signicant except the omega of bitcoin and omega of litecoin which means that there truly exists the dynamic correlations in Bitcoin return and Litecoin return. <br>

![bl](https://github.com/WangJiajia-0901/PHBS_BlockChain_2018/blob/master/Image/bl.png) <br>
Also, the dynamic conditional correlation plot shows the correlations between Bitcoin return and Litecoin return, especially from the second quarter of 2017. <br>

#### Ether and Litecoin
| |Estimated|Std.Error|t value| p value|
|:------:|:------:|:------:|:------:|:------:|
|etheromega    |  0.018801  |  0.013171  |1.42744 | 0.15345|
|etheralpha1  |   0.126511  |  0.017359|  7.28812 | 0.00000|
|etherbeta1    |  0.872489 |   0.022616 |38.57800 | 0.00000|
|litecoinomega  | 0.003782  |  0.003792 | 0.99721 | 0.31866|
|litecoinalpha1 | 0.088651  |  0.015605 | 5.68104 | 0.00000|
|litecoinbeta1  | 0.910349  |  0.024512 |37.13929 | 0.00000|
|Jointdcca1      | 0.112778 |   0.017238  |6.54238|  0.00000|
|Jointdccb1    |   0.884633  |  0.017867 |49.51105  |0.00000|
|Jointmshape   |   4.807511  |  0.282406| 17.02342 | 0.00000|
                
|Information criteria|value|
|:------:|:------:|
|Akaike    |   8.5011|
|Bayes    |  8.5633|
|Shibata  |    8.5008|
|Hannan-Quinn| 8.5224|
                
Similarily, except the omega of ether and omega of litecoin all the coefficients are significant which proves the dynamic relations between ether return and litecoin return. <br>
               
![el](https://github.com/WangJiajia-0901/PHBS_BlockChain_2018/blob/master/Image/el.png)

Similar as the above two plots, this figure also confirms the correlations between ether return and litecoin return. Moreover, the most of time the correlations are positive. <br>

## Conclusion 
The  emprical analysis of the time-varying conditional correlation in returns of Bitcoin, Ether and Litecoin with pair-wise DCC-GARCH models proves my original guess about that. There are comovements  in the three cryptocurrencies and most time are positively correlated. With this conculsion, we can make better investment decisions in cryptocurrencies. The future study is to deeper this project to find more detailed relationship and analyze the ceration changes in different certain period instead of getting the overall conclusion.
## References
[1]  Mandelbrot, B. B.(1963) The Variation of Certain Speculative Prices. The Journal of Business 36, No. 4,394-419.<br>
[2]  Nader Trabelsi.(2019) Are There Any Volatility Spill-Over Effects among Cryptocurrencies and Widely Traded Asset Classes? Journal of Rish and Financial Management, 11, 66-83.<br>
[3]  Norwegian University of Science and Technology, Multivariate DCC-GARCH Model-with various error distributions. Lecture notes.<br>
[4]  Paraskevi Katsiampaa.(2019) Shaen Corbet, Brian Lucey. Volatility spillover effects in leading cryptocurrencies: A BEKKMGARCH
analysis, Finance Research Letters,29, 68–74. <br>

