# Trading-Algorithms-I-Accruals
Accruals trading strategy is based on a simple premise that the cash component proviides surety of the transaction that has happened or it's going to happen in near future but whereas the non-cash component or accruals doesn't give us that surety because the transactions may happen over longer periods of time and there is no guarantee that the due will be completely paid. But the companies sometimes uses these "cook the books" technique to bloat up the numbers and make it look enticing to the investors but in reality that is unsure transaction lined up in future with no surety. So, the more the accrual, the chances of default would be more, hence we ought to short the stock and long the stocks with lesser accruals 

## Dataset
-6000 firms registered on the BSE from 2011-2019.

-S&P BSE 500 index from 2011-2019.

## Approach
-Calculated the accrual component for every firm in the data-set by the following formula:

    Accrual = ((del_CA-del_Cash)-(del_CL-del_Short-termborrowing)-depreciation)/Avg total asset for previous period
    
-Calculated the returns for the firms in the data set on yearly,quarterly and semi-annual basis
    
-Sorted the firms in deciles on the basis of amount of accruals they hold, went long on top decile(minimum accruals) and shorted the bottom decile(maximum accruals)
