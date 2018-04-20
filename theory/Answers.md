* Single regex that matches either of these: **/(antelopes?)/g**

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