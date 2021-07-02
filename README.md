# Analysis-of-Scheduled-Commercial-Banks-Net-Non-performing-Asset
Analysis of Scheduled Commercial Banks Net Non performing Asset based on Selected Ratios

Definition of 'Non Performing Assets'

Definition: A non performing asset (NPA) is a loan or advance for which the principal or interest payment remained overdue for a period of 90 days.

Description: Banks are required to classify NPAs further into Substandard, Doubtful and Loss assets.

  1.  Substandard assets: Assets which has remained NPA for a period less than or equal to 12 months.

  2.  Doubtful assets: An asset would be classified as doubtful if it has remained in the substandard category for a period of 12 months.

  3.  Loss assets: As per RBI, “Loss asset is considered uncollectible and of such little value that its continuance as a bankable asset is not warranted, although there may be          some salvage or recovery value.”

Motivation:

Data Source: 

  https://dbie.rbi.org.in/DBIE/dbie.rbi?site=publications

  https://fred.stlouisfed.org/series/INDCPIALLQINMEI
             
  https://www.bankbazaar.com/finance-tools/emi-calculator/current-rbi-bank-interest-rates.html
  
  Data Set contain 37 columns and 1422 rows containing data of Public Sector, Private Sector, Foreign Bank Group, Small Finance Bank and Paytm Banks data from the year 2005 to     2020
  Analysis was focused on the data ranging from year 2007 to 2020 of Public Sector and  Private Sector bank group. Additionaly we added bank group, cpi and repo rate data.
  The NNPA ratio was divided into 3 brackets Low(<1%), Midium(1%-2%) and high(>2%)
  
  ## Univariate Analysis
  
  ![1](https://user-images.githubusercontent.com/76644910/124307118-fa833180-db84-11eb-864a-589fa21a727d.png)

53.31% banks in our dataset are Public Sector banks and 46.69% are Private Sector Banks
\
\
\
![2](https://user-images.githubusercontent.com/76644910/124307252-2d2d2a00-db85-11eb-80e9-97eddd7100e2.png)

37.38% nbanks have high NNPA ratio, 24.61% banks have midium NNPA ratio, 38.01% banks low NNPA ratio
\
\
\
  ![3](https://user-images.githubusercontent.com/76644910/124307317-4b932580-db85-11eb-9dce-fc75e9084284.png)

V6,V10, V22,V23, capitalMarketSector_adv, realEstateSector_adv are heavily skewd data.
Target variable V36 is also right skewed
\
\
\
  ![4](https://user-images.githubusercontent.com/76644910/124307475-809f7800-db85-11eb-8d30-960e98865255.png)

'V12'(Ratio of interest income to total assets) ,
'V13'(Ratio of net interest income to total assets (Net Interest Margin)) ,
'V14'(Ratio of non-interest income to total assets)
Median of interest income is thrice the median of non interest income
\
\
\
  ![5](https://user-images.githubusercontent.com/76644910/124307605-b0e71680-db85-11eb-8dd3-a378bf01e1c6.png)

'V27'(Return on Advances) ,
'V28'(Return on investments) ,
Clearly return on advances has higher range compared to return on investment
\
\
\
  ![6](https://user-images.githubusercontent.com/76644910/124307856-0d4a3600-db86-11eb-94d8-e215c4df6006.png)

'V8'(Ratio of priority sector advances to total advances)
'V9'(Ratio of term loans to total advances) ,
'V10'(Ratio of secured advances to total advances)
Overall banks give more secured loans and least loan to priority sectors


## Bivariate Analysis
#### Year wise box plot of NNPA ratio for Public Sector and Private Sector Banks
  ![1](https://user-images.githubusercontent.com/76644910/124308011-3ec30180-db86-11eb-882e-8925874a0256.png)

Median and range of NNPA ratio for PUBLIC SECTOR BANK is increasing with year while for PRIVATE SECTOR BANKS range has increased but is almost same over the years.
PUBLIC SECTOR BANKS NNPA ratio are in in higher range compared to PRIVATE SECTOR BANKS


#### No. of banks falling under different NNPA ratio bracket for Public Sector banks and Private Sector Banks
  ![2](https://user-images.githubusercontent.com/76644910/124308088-5dc19380-db86-11eb-8a62-8cdc1db4a0ff.png)

PUBLIC SECTOR BANK GROUP has more banks with HIGH NNPA ratio while PRIVATE SECTOR group has more bank with LOW NNPA ratio


  ![3](https://user-images.githubusercontent.com/76644910/124308149-75008100-db86-11eb-9da2-4ccf76bc3679.png)
Comparing banks with high NNPA ratio for both PUBLIC and PRIVATE SECTOR GROUP it can be seen median and range of NNPA ratio for banks in PUBLIC SECTOR BANK GROUP is much higher as compared to banks in PRIVATE SECTOR BANK GROUP
\
\
\
