Find regexes that match the following. (e.g. find a single regex that matches
both `antelope` and `antelopes`.)**/(antelopes?)/g**

* Single regex that matches either of these: **/(antelopes?\srocks?\sout)/g**

    antelope rocks out
    antelopes rock out

* Regex that matches either of:**/(goat|moat)/g**

    goat
    moat

  but not:

    boat

* Regex that matches dates in YYYY-MM-DD format. (Year can be 1-4 digits, and
  month and day can each be 1-2 digits). This does not need to verify the date
  is correct (e.g 3333-33-33 can match). **/[0-9]{1,4}-[0-9]{1,2}-[0-9]{1,2}/g**

  2000-10-12
  1999-1-20
  1999-01-20
  812-2-10

* Come up with regexes for the two above sequences. The one to set the cursor position should accept any digits for the row and column. The bold sequence need only accept 1 (and is a trivial regex). (ESC is a single character which can be represented with \e in the regex.)
    **/(\e\[)[0-9]\d+;[0-9]\d+[a-z]/gi**
    **/(\e\[1m)/g**