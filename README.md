An epidemiological week, commonly referred to as an epi week or a CDC week, is simply a standardized method of counting 
weeks to allow for the comparison of data year after year.

### Definition
The first epi week of the year ends, by definition, on the first Saturday of January, as long as it falls at least four
days into the month. Each epi week begins on a Sunday and ends on a Saturday.

### Usage
``` javascript
import epi from 'epidemiological-week'

epi.calculate('2006-12-31')  //{year: 2007, week: 1}
epi.calculate('2007-01-07')  //{year: 2007, week: 2}
epi.calculate('2016-01-01')  //{year: 2015, week: 52}
epi.calculate('2016-01-03')  //{year: 2016, week: 1}
epi.calculate('2016-11-13')  //{year: 2016, week: 46}

epi.calculate('12-31-2006', 'MM-DD-YYYY')  //{year: 2007, week: 1}
epi.calculate('31-12-2006', 'DD-MM-YYYY')  //{year: 2007, week: 1}

//Special dates
//These dates can not be found on epi calendar, so for now just give it -1
epi.calculate('2008-12-28')  //{year: -1, week: -1}
epi.calculate('2014-12-28')  //{year: -1, week: -1}
epi.calculate('2009-01-02')  //{year: -1, week: -1}
epi.calculate('2015-01-03')  //{year: -1, week: -1} 
```

>You can find the definition and calendars on [this website](http://www.cmmcp.org/epiweek.htm)   
>The result of the function is exactly the same as what those calendars show



