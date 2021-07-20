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
  The NNPA ratio was divided into 3 brackets Low(<1%), Medium(1%-2%) and high(>2%)
  
**Column name and there meaning**

![image](https://user-images.githubusercontent.com/76644910/126267393-6ff6a38c-0835-44b7-a6ca-afbd2c54b3de.png)



_________________________________________________________________________________________________________________________________________
  
 ## Univariate Analysis
  
![1](https://user-images.githubusercontent.com/76644910/124775541-54f10900-df5c-11eb-8cc3-fe96cd68717b.png)

 53.31% banks in our dataset are Public Sector banks and 46.69% are Private Sector Banks
_________________________________________________________________________________________________________________________________________

![2](https://user-images.githubusercontent.com/76644910/124775598-5f130780-df5c-11eb-907b-bd9bbb22e043.png)

 37.38% banks have high NNPA ratio, 24.61% banks have medium NNPA ratio, 38.01% banks low NNPA ratio
_________________________________________________________________________________________________________________________________________

![3](https://user-images.githubusercontent.com/76644910/124775633-6803d900-df5c-11eb-9bc6-d19c166a9ae4.png)


V6 (Ratio of deposits to total liabilities), V10 (Ratio of secured advances to total advances), V22 (Return on assets), V23 (Return on equity), capitalMarketSector_adv, realEstateSector_adv are heavily skewed data.

Target variable V36 (Net NPA ratio) is also right skewed

_________________________________________________________________________________________________________________________________________

![4](https://user-images.githubusercontent.com/76644910/124775667-6fc37d80-df5c-11eb-95c5-feecddf50388.png)


'V12'(Ratio of interest income to total assets),

'V13'(Ratio of net interest income to total assets (Net Interest Margin)),

'V14'(Ratio of non-interest income to total assets)

 Median of interest income is thrice the median of non-interest income.

_________________________________________________________________________________________________________________________________________

![5](https://user-images.githubusercontent.com/76644910/124775707-78b44f00-df5c-11eb-906c-9fb173bc93fb.png)


'V27'(Return on Advances),

'V28'(Return on investments),

Clearly return on advances has higher range compared to return on investment.

_________________________________________________________________________________________________________________________________________

![6](https://user-images.githubusercontent.com/76644910/124775741-7fdb5d00-df5c-11eb-8c55-6d2a9fe61251.png)


'V8'(Ratio of priority sector advances to total advances),

'V9'(Ratio of term loans to total advances),

'capitalMarketSector_adv'(Ratio of Capital Market Sector advances to total advances),

'realEstateSector_adv'(Ratio of Real Estate Sector advances to total advances)

Overall banks give more Real Estate Sector and least to Capital Market Sector.

_________________________________________________________________________________________________________________________________________


## Bivariate Analysis
#### Year wise box plot of NNPA ratio for Public Sector and Private Sector Banks
![1](https://user-images.githubusercontent.com/76644910/124775792-89fd5b80-df5c-11eb-9bfe-30168b79a84f.png)


Median and range of NNPA ratio for PUBLIC SECTOR BANK is increasing with year while for PRIVATE SECTOR BANKS range has increased but is almost same over the years.
PUBLIC SECTOR BANKS NNPA ratios are in in higher range compared to PRIVATE SECTOR BANKS.

_________________________________________________________________________________________________________________________________________
#### No. of banks falling under different NNPA ratio bracket for Public Sector banks and Private Sector Banks
![2](https://user-images.githubusercontent.com/76644910/124775820-91246980-df5c-11eb-9d8e-70afd314eb01.png)


PUBLIC SECTOR BANK GROUP has more banks with HIGH NNPA ratio while PRIVATE SECTOR group has more banks with LOW NNPA ratio.
_________________________________________________________________________________________________________________________________________
#### NNPA ratio bracket wise comparison of Public Sector and Private Sector Bank
![3](https://user-images.githubusercontent.com/76644910/124775866-98e40e00-df5c-11eb-8d1c-e16a16afdb3f.png)


Comparing banks with high NNPA ratio for both PUBLIC and PRIVATE SECTOR GROUP it can be seen median and range of NNPA ratio for banks in PUBLIC SECTOR BANK GROUP is much higher as compared to banks in PRIVATE SECTOR BANK GROUP.
_________________________________________________________________________________________________________________________________________
#### Public Sector Banks variation of NNPA ratio
![4](https://user-images.githubusercontent.com/76644910/124775897-a00b1c00-df5c-11eb-933b-ab980e622be8.png)


Over the year Public Sector Banks have increasing trend of NNPA ratio. From 2015 till 2018 increment is very sharp. 
After that NNPA ratio has decreased but still they all are in HIGH NNPA ratio bracket.
_________________________________________________________________________________________________________________________________________
#### Private Sector Banks variation of NNPA ratio
![5](https://user-images.githubusercontent.com/76644910/124775931-a8fbed80-df5c-11eb-8b37-d5288987a45e.png)


Unlike Public Sector Banks, Private Sector Banks NNPA ratio has no increasing trend. Also for most of the Private Sector Banks their NNPA ratio fall under MID or LOW NNPA ratio bracket.
_________________________________________________________________________________________________________________________________________
**Conclusion:**
Recovery of loan in Private Sector Banks in better as compared to Public Sector Banks
_________________________________________________________________________________________________________________________________________

## Multivariate Analysis
#### Bank group and NNPA ratio bracket wise variation of NNPA ratio with Term loan to total advances ratio
![1](https://user-images.githubusercontent.com/76644910/124775983-b4e7af80-df5c-11eb-97b7-7ce7d6fc35a5.png)


Term loan to total advance ratio has no trend with HIGH NNPA ratio for both PUBLIC and PRIVATE SECTOR BANK GROUP

In the MID range NNPA ratio it has slight increasing trend for PUBLIC SECTOR BANKS while slight decreasing for PRIVATE SECTOR BANKS.

In the LOW range NNPA ratio it has increasing trend for PUBLIC SECTOR BANKS while slight decreasing for PRIVATE SECTOR BANKS.

Over all if PUBLIC SECTOR BANKS lend more term loans then there NNPA will increase only in LOW range.

_________________________________________________________________________________________________________________________________________
#### Bank group and NNPA ratio bracket wise variation of NNPA ratio with Priority Sector advances to total advances ratio

![2](https://user-images.githubusercontent.com/76644910/124776030-bd3fea80-df5c-11eb-9319-7b6430e6037a.png)


NNPA ratio for banks with HIGH NNPA ratio in PUBLIC SECTOR BANK group increases quite significantly with increase in loan to priority sectors. 
This means for them more loan get default in priority sector.

NNPA ratio for banks with MID NNPA ratio in PUBLIC SECTOR BANK group decreases quite significantly with increase in loan to priority sectors. 
This means these banks are efficient in recovering loan/NPA from priority sector.

For PRIVATE SECTOR BANK group there is not much trend between NNPA ratio and loan to priority sector.

_________________________________________________________________________________________________________________________________________
#### Bank group and NNPA ratio bracket wise variation of NNPA ratio with Unsecured advances to total advances ratio

![3](https://user-images.githubusercontent.com/76644910/124776073-c761e900-df5c-11eb-9bb6-95ad31314d82.png)


For banks with HIGH NNPA ratio in both PRIVATE and PUBLIC SECTOR BANK group and LOW NNPA ratio in PRIVATE SECTOR BANK group
NNPA ratio decreases moderately with increase in unsecured loans.

This means for these banks loan recovery is good for unsecured loans. It also indicates bank put more effort and resources in recovering unsecured loan.

_________________________________________________________________________________________________________________________________________
#### Bank group and NNPA ratio bracket wise variation of NNPA ratio with Capital Market Sector advances to total advances ratio

![4](https://user-images.githubusercontent.com/76644910/124776121-cfba2400-df5c-11eb-8615-b4c3d1343088.png)


Banks with LOW NNPA ratio in PRIVATE SECTOR BANK GROUP has significant decrease in NNPA ratio with increase in loan to Capital market sector. 
It means for these banks loan recovery from this sector is good. For rest of the categories there is not much trend.

_________________________________________________________________________________________________________________________________________
#### Bank group and NNPA ratio bracket wise variation of NNPA ratio with Real Estate Sector advances to total advances ratio

![5](https://user-images.githubusercontent.com/76644910/124776162-d8125f00-df5c-11eb-930e-ddf8297456db.png)


BBanks with LOW NNPA ratio in PRIVATE SECTOR BANK GROUP has significant increase in NNPA ratio with increase in loan to Real Estate sector. 
It means for these banks there are more loan default cases from Real Estates.
_________________________________________________________________________________________________________________________________________
#### Bank group and NNPA ratio bracket wise variation of NNPA ratio with Repo Rate

![6](https://user-images.githubusercontent.com/76644910/124776190-de084000-df5c-11eb-8070-e2a9abef42ba.png)


Banks falling in HIGH NNPA ratio bracket in PUBLIC SECTOR BANK GROUP has significant decreasing trend in NNPA ratio 
with increase in repo rate while for banks falling in MID NNPA ratio bracket in the same group NNPA ratio increases with increase in repo rate.
_________________________________________________________________________________________________________________________________________
#### Bank group and NNPA ratio bracket wise variation of NNPA ratio with Consumer Price Index

![7](https://user-images.githubusercontent.com/76644910/124776223-e496b780-df5c-11eb-9e25-5e9753b904ba.png)


For every bank NNPA ratio has decreasing trend with increase in consumer price index especially for banks with HIGH NNPA ratio in PUBLIC SECTOR BANK group.

_________________________________________________________________________________________________________________________________________

## HYPOTHESIS TESTING

![image](https://user-images.githubusercontent.com/76644910/126267994-5bf25329-4f1f-4e5e-b0f3-e66711b07e06.png)

_________________________________________________________________________________________________________________________________________
_________________________________________________________________________________________________________________________________________

![image](https://user-images.githubusercontent.com/76644910/126268207-b41a334c-88fc-4994-a327-c00cc4a45242.png)

_________________________________________________________________________________________________________________________________________
_________________________________________________________________________________________________________________________________________

![image](https://user-images.githubusercontent.com/76644910/126268245-afe75c1d-320b-4dd4-b354-06576e5da9b4.png)

_________________________________________________________________________________________________________________________________________
_________________________________________________________________________________________________________________________________________

![image](https://user-images.githubusercontent.com/76644910/126268290-70c775ac-f382-48a5-8677-59b82c713582.png)

_________________________________________________________________________________________________________________________________________
_________________________________________________________________________________________________________________________________________

## MODEL BUILDING
Linear Regression was applied to understand association of NNPA ratio with different ratios of Schedule Commercial Banks such as
Unsecured advances to total advances ratio, Cash deposit ratio, consumer price index, etc.

We added lagged NNPA ratio column which contains previous year NNPA ratio and used it as predictor variable.

NNPA ratio bracket column and Bank Group column were categorical variable so we did one hot encoding for these variables.

We computed Adjusted_R2 which was obtained as 0.792 which means 79 % of the variation of target column expense can be well explained by one of the predictor variables.

We then use the stats model to find a summary of the linear regression model and the following are found.
Using Variance Inflation factor and stats model summary we removed those variable which were not significant or causing high multi-colinearity.

Final Output is presented below

__1. Regression Summary


![1](https://user-images.githubusercontent.com/76644910/124777258-b4034d80-df5d-11eb-96f7-2237054c6eaf.JPG)

_________________________________________________________________________________________________________________________________________
_________________________________________________________________________________________________________________________________________

__2. VIF summary

![2](https://user-images.githubusercontent.com/76644910/124777287-b9609800-df5d-11eb-8e81-6f3d263a87df.JPG)

_________________________________________________________________________________________________________________________________________
_________________________________________________________________________________________________________________________________________

__3. Residual Plot

![3](https://user-images.githubusercontent.com/76644910/124777500-e0b76500-df5d-11eb-924b-dfe28766b5dd.png)

_________________________________________________________________________________________________________________________________________
_________________________________________________________________________________________________________________________________________

__4. qq- plot

![4](https://user-images.githubusercontent.com/76644910/124777529-e6ad4600-df5d-11eb-85f9-94e26c22a88c.png)

_________________________________________________________________________________________________________________________________________
_________________________________________________________________________________________________________________________________________

__5. Final Regression Equation

![3](https://user-images.githubusercontent.com/76644910/124780764-7ce26b80-df60-11eb-8ba6-d1d7b2cd84b6.JPG)

_________________________________________________________________________________________________________________________________________
_________________________________________________________________________________________________________________________________________

__6. Feature Importance

![5](https://user-images.githubusercontent.com/76644910/124777642-fe84ca00-df5d-11eb-81fc-185df83e82d5.png)

_________________________________________________________________________________________________________________________________________
_________________________________________________________________________________________________________________________________________
