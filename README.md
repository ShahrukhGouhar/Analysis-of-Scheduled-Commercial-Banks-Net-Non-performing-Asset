# Analysis-of-Scheduled-Commercial-Banks-Net-Non-performing-Asset
Analysis of Scheduled Commercial Banks Net Non performing Asset based on Selected Ratios

**Definition of 'Non Performing Assets'**

**Definition:** A non performing asset (NPA) is a loan or advance for which the principal or interest payment remained overdue for a period of 90 days.

**Description:** Banks are required to classify NPAs further into Substandard, Doubtful and Loss assets.

  1.  Substandard assets: Assets which has remained NPA for a period less than or equal to 12 months.

  2.  Doubtful assets: An asset would be classified as doubtful if it has remained in the substandard category for a period of 12 months.

  3.  Loss assets: As per RBI, “Loss asset is considered uncollectible and of such little value that its continuance as a bankable asset is not warranted, although there may be          some salvage or recovery value.”

**MOTIVATION:** 
Non-performing assets are a reflection of the bank’s overall efficiency while performing its business of converting deposits into loans and recovering these loans. Non-recovery or partial recovery of loans has an impact on the bank’s balance sheet and income statement items in the form of reduction in interest earned on loan assets, increase in provision on NPAs, increase in capital requirement and lower profits. Hence, rising NPAs are a concern for a bank and determinants of NPAs should be identified prior to loans turning into NPAs.

**OBJECTIVE:** To find Association of NNPA ratio with different ratios such as operational capability, solvency and profitability of Schedule Commercial Banks.

**Data Source:**

  https://dbie.rbi.org.in/DBIE/dbie.rbi?site=publications

  https://fred.stlouisfed.org/series/INDCPIALLQINMEI
             
  https://www.bankbazaar.com/finance-tools/emi-calculator/current-rbi-bank-interest-rates.html
  
  Data Set contain 37 columns and 1422 rows containing data of Public Sector, Private Sector, Foreign Bank Group, Small Finance Bank and Paytm Banks data from the year 2005 to     2020
  Analysis was focused on the data ranging from year 2007 to 2020 of Public Sector and  Private Sector bank group. Additionaly we added bank group, cpi and repo rate data.
  The NNPA ratio was divided into 3 brackets Low(<1%), Midium(1%-2%) and high(>2%)
_________________________________________________________________________________________________________________________________________
  
 ## Univariate Analysis
  
![1](https://user-images.githubusercontent.com/76644910/124307118-fa833180-db84-11eb-864a-589fa21a727d.png)

 53.31% banks in our dataset are Public Sector banks and 46.69% are Private Sector Banks
_________________________________________________________________________________________________________________________________________

![2](https://user-images.githubusercontent.com/76644910/124307252-2d2d2a00-db85-11eb-80e9-97eddd7100e2.png)

 37.38% nbanks have high NNPA ratio, 24.61% banks have midium NNPA ratio, 38.01% banks low NNPA ratio
_________________________________________________________________________________________________________________________________________

 ![3](https://user-images.githubusercontent.com/76644910/124307317-4b932580-db85-11eb-9dce-fc75e9084284.png)

 V6(Ratio of deposits to total liabilities),V10(Ratio of secured advances to total advances), 
 V22(Return on assets),V23(Return on equity), capitalMarketSector_adv, realEstateSector_adv are heavily skewd data.
 
 Target variable V36(Net NPA ratio) is also right skewed
_________________________________________________________________________________________________________________________________________

 ![4](https://user-images.githubusercontent.com/76644910/124307475-809f7800-db85-11eb-8d30-960e98865255.png)

'V12'(Ratio of interest income to total assets),

'V13'(Ratio of net interest income to total assets (Net Interest Margin)),

'V14'(Ratio of non-interest income to total assets)

 Median of interest income is thrice the median of non interest income
_________________________________________________________________________________________________________________________________________

 ![5](https://user-images.githubusercontent.com/76644910/124307605-b0e71680-db85-11eb-8dd3-a378bf01e1c6.png)

'V27'(Return on Advances),

'V28'(Return on investments),

 Clearly return on advances has higher range compared to return on investment
_________________________________________________________________________________________________________________________________________

![6](https://user-images.githubusercontent.com/76644910/124342925-4f569480-dbe5-11eb-8f1d-589e5966dc20.png)

'V8'(Ratio of priority sector advances to total advances),

'V9'(Ratio of term loans to total advances),

'capitalMarketSector_adv'(Ratio of Capital Market Sector advances to total advances),

'realEstateSector_adv'(Ratio of Real Estate Sector advances to total advances).

 Overall banks give more Real Estate Sector and least to Capital Market Sector
_________________________________________________________________________________________________________________________________________


## Bivariate Analysis
#### Year wise box plot of NNPA ratio for Public Sector and Private Sector Banks
![1](https://user-images.githubusercontent.com/76644910/124308011-3ec30180-db86-11eb-882e-8925874a0256.png)

Median and range of NNPA ratio for PUBLIC SECTOR BANK is increasing with year while for PRIVATE SECTOR BANKS range has increased but is almost same over the years.
PUBLIC SECTOR BANKS NNPA ratio are in in higher range compared to PRIVATE SECTOR BANKS

_________________________________________________________________________________________________________________________________________
#### No. of banks falling under different NNPA ratio bracket for Public Sector banks and Private Sector Banks
![2](https://user-images.githubusercontent.com/76644910/124308088-5dc19380-db86-11eb-8a62-8cdc1db4a0ff.png)

PUBLIC SECTOR BANK GROUP has more banks with HIGH NNPA ratio while PRIVATE SECTOR group has more bank with LOW NNPA ratio
_________________________________________________________________________________________________________________________________________
#### NNPA ratio bracket wise comparison of Public Sector and Private Sector Bank
![3](https://user-images.githubusercontent.com/76644910/124308149-75008100-db86-11eb-9da2-4ccf76bc3679.png)

Comparing banks with high NNPA ratio for both PUBLIC and PRIVATE SECTOR GROUP it can be seen median and range of NNPA ratio for banks in PUBLIC SECTOR BANK GROUP is much higher as compared to banks in PRIVATE SECTOR BANK GROUP
_________________________________________________________________________________________________________________________________________
#### Public Sector Banks variation of NNPA ratio
![4](https://user-images.githubusercontent.com/76644910/124342108-1fa48e00-dbdf-11eb-9e28-ff7a41dc5353.png)

Over the year Public Sector Banks have increasing trend of NNPA ratio. From 2015 till 2018 increament is very sharp. After that NNPA ratio has decreased but still they all are in HIGH NNPA ratio bracket
_________________________________________________________________________________________________________________________________________
#### Private Sector Banks variation of NNPA ratio
![5](https://user-images.githubusercontent.com/76644910/124342339-d05f5d00-dbe0-11eb-9ff1-e5fed3cfb30c.png)

Unlike Public Sector Banks, Private Sector Banks NNPA ratio has no increasing trend. Also for most of the Private Sector Banks their NNPA ratio fall under MID or LOW NNPA ratio bracket.
_________________________________________________________________________________________________________________________________________
**Conclusion:**
Recovery of loan in Private Sector Banks in better as compared to Public Sector Banks
_________________________________________________________________________________________________________________________________________

## Multivariate Analysis
#### Bank group and NNPA ratio bracket wise variation of NNPA ratio with Term loan to total advances ratio
![1](https://user-images.githubusercontent.com/76644910/124343229-99d91080-dbe7-11eb-8bd3-e36ff7872b19.png)

Term loan to total advance ratio has no trend with HIGH NNPA ratio for both PUBLIC and PRIVATE SECTOR BANK GROUP

In the MID range NNPA ratio it has slight increasing trend for PUBLIC SECTOR BANKS while slight decreasing for PRIVATE SECTOR BANKS.

In the LOW range NNPA ratio it has increasing trend for PUBLIC SECTOR BANKS while slight decreasing for PRIVATE SECTOR BANKS.

Over all if PUBLIC SECTOR BANKS lend more trem loans then there NNPA will increase only in LOW range
_________________________________________________________________________________________________________________________________________
#### Bank group and NNPA ratio bracket wise variation of NNPA ratio with Priority Sector advances to total advances ratio

![2](https://user-images.githubusercontent.com/76644910/124343451-2fc16b00-dbe9-11eb-84d4-7d696f3ac798.png)


NNPA ratio for banks with HIGH NNPA ratio in PUBLIC SECTOR BANK group increases quite significantly with increase in loan to priority sectors. This means for them more loan get default in priority sector.

NNPA ratio for banks with MID NNPA ratio in PUBLIC SECTOR BANK group decreases quite significantly with increase in loan to priority sectors. This means these banks are efficient in recovering loan/NPA from priority sector.

For PRIVATE SECTOR BANK group there is not much trend between NNPA ratio and loan to priority sector.
_________________________________________________________________________________________________________________________________________
#### Bank group and NNPA ratio bracket wise variation of NNPA ratio with Unsecured advances to total advances ratio

![3](https://user-images.githubusercontent.com/76644910/124343598-69df3c80-dbea-11eb-88cc-bfd61802f713.png)

NNPA ratio for banks with HIGH NNPA ratio in both PRIVATE and PUBLIC SECTOR BANK group and LOW NNPA ratio in PRIVATE SECTOR BANK group decreases moderately with increase in unsecured loans.

This means for these banks loan recovery is good for unsecured loans. It also indicates bank put more effort and resources in recovering unsecured loan.
_________________________________________________________________________________________________________________________________________
#### Bank group and NNPA ratio bracket wise variation of NNPA ratio with Capital Market Sector advances to total advances ratio

![4](https://user-images.githubusercontent.com/76644910/124343710-5aacbe80-dbeb-11eb-91f5-43f4704a218e.png)

Banks with LOW NNPA ratio in PRIVATE SECTOR BANK GROUP has significant decrease in NNPA ratio with increase in loan to Capital market sector. 
It means for these banks loan recovery from this sector is good. For rest of the categories there is not much trend.

_________________________________________________________________________________________________________________________________________
#### Bank group and NNPA ratio bracket wise variation of NNPA ratio with Real Estate Sector advances to total advances ratio

![5](https://user-images.githubusercontent.com/76644910/124343848-4c12d700-dbec-11eb-94d2-d1d8d5364b8e.png)

Banks with LOW NNPA ratio in PRIVATE SECTOR BANK GROUP has significant increase in NNPA ratio with increase in loan to Real Estate sector. 
It means for these banks there are more loan default cases from Real Estate.
_________________________________________________________________________________________________________________________________________
#### Bank group and NNPA ratio bracket wise variation of NNPA ratio with Repo Rate

![6](https://user-images.githubusercontent.com/76644910/124343953-2a661f80-dbed-11eb-94de-2e30408d558b.png)

Banks falling in HIGH NNPA ratio bracket in PUBLIC SECTOR BANK GROUP has significant decreasing trend in NNPA ratio with increase in repo rate while for banks falling in MID NNPA ratio bracket in the same group NNPA ratio increases with increase in repo rate
_________________________________________________________________________________________________________________________________________
#### Bank group and NNPA ratio bracket wise variation of NNPA ratio with Consumer Price Index

![7](https://user-images.githubusercontent.com/76644910/124344172-79f91b00-dbee-11eb-9dfd-109a4e4b47a6.png)

For every bank NNPA ratio has decreasing trend with increase in consumer price index specially for banks with HIGH NNPA ratio in PUBLIC SECTOR BANK group.

_________________________________________________________________________________________________________________________________________

## HYPOTHESIS TESTING

![1](https://user-images.githubusercontent.com/76644910/124344688-6a2f0600-dbf1-11eb-8576-5fe9f96cd973.JPG)

![2](https://user-images.githubusercontent.com/76644910/124344691-6c916000-dbf1-11eb-9e5c-716c9512dd55.JPG)

![3](https://user-images.githubusercontent.com/76644910/124344694-71eeaa80-dbf1-11eb-81af-61dee8e30f95.JPG)

![4](https://user-images.githubusercontent.com/76644910/124344679-64392500-dbf1-11eb-9f12-eb1ce35405c8.JPG)

_________________________________________________________________________________________________________________________________________
_________________________________________________________________________________________________________________________________________
![1](https://user-images.githubusercontent.com/76644910/124344792-2a1c5300-dbf2-11eb-8309-20f5141400d5.JPG)

![2](https://user-images.githubusercontent.com/76644910/124344796-2d174380-dbf2-11eb-8d7b-69f341de3c39.JPG)

![3](https://user-images.githubusercontent.com/76644910/124344798-30123400-dbf2-11eb-937c-d08c7caac4d3.JPG)

_________________________________________________________________________________________________________________________________________
_________________________________________________________________________________________________________________________________________

![1](https://user-images.githubusercontent.com/76644910/124344909-0b6a8c00-dbf3-11eb-89db-11c2174f71d0.JPG)

![2](https://user-images.githubusercontent.com/76644910/124344911-0dcce600-dbf3-11eb-8ff2-5b6ea11d9e15.JPG)

![3](https://user-images.githubusercontent.com/76644910/124344913-10c7d680-dbf3-11eb-9172-a1f1ce1e9f10.JPG)

_________________________________________________________________________________________________________________________________________
_________________________________________________________________________________________________________________________________________

![1](https://user-images.githubusercontent.com/76644910/124344987-8fbd0f00-dbf3-11eb-975d-818fc8df7cd7.JPG)

![2](https://user-images.githubusercontent.com/76644910/124344992-9481c300-dbf3-11eb-859b-a3b336556706.JPG)

_________________________________________________________________________________________________________________________________________
_________________________________________________________________________________________________________________________________________

## MODEL BUILDING
Lineaer Regression was applied to understand association of NNPA ratio with different ratios of Schedule Commercial Banks such as
unsecured advances to total advances ratio, Cash deposit ratio, consumer price index, etc
We added lagged NNPA ratio column which contains previous year NNPA ratio and used it as predictor variable.

NNPA ratio bracket column and Bank Group column were categorical variable so we did one hot encoding for these variables.

We computed Adjusted_R2 which was obtained as 0.792 which means 79 % of the variation of target column expense can be well explained by one of the predictor variables.

We then use the stats model to find a summary of the linear regression model and the following are found.
Using Variance Inflation factor and stats model summary we removed those variable which were not significant or causing high multi collinearity.

Final Output is presented below

__1. Regression Summary

![1](https://user-images.githubusercontent.com/76644910/124347065-f6482a00-dbff-11eb-9aeb-56f380d59855.JPG)

_________________________________________________________________________________________________________________________________________
_________________________________________________________________________________________________________________________________________

__2. VIF summary

![2](https://user-images.githubusercontent.com/76644910/124347084-2394d800-dc00-11eb-8d5a-149176e1db6f.JPG)

_________________________________________________________________________________________________________________________________________
_________________________________________________________________________________________________________________________________________

__3. Residual Plot

![3](https://user-images.githubusercontent.com/76644910/124347108-50e18600-dc00-11eb-8063-941c974c8106.png)
_________________________________________________________________________________________________________________________________________
_________________________________________________________________________________________________________________________________________

__4. qq- plot

![4](https://user-images.githubusercontent.com/76644910/124347114-5d65de80-dc00-11eb-9953-f9beb9702936.png)
_________________________________________________________________________________________________________________________________________
_________________________________________________________________________________________________________________________________________

__5. Final Regression Equation

![3](https://user-images.githubusercontent.com/76644910/124347675-791eb400-dc03-11eb-8c0b-31a85e0cb3d4.JPG)

