# udacity_python_prog_foundations
projects in the Udacify Programming Foundations in Python 

#project idea

#1) automate daily web browsing, auto check several web pages and bring to one place / one run of program instead of multiple book mark checks.
# an opportunity to research and practice python.

 #   -   get me the latest value of x- stocks

    #-   show me 5 most recent reuters wire headings
    #-   show me the top heading on reddit
    # -  show me something funnty eg youtube sketch
    # - show me soemthign cretive eg a poem by yeats! (search for or go to one site in particular etc)
    #-   show me a photo from NG or Reddit.earth 
    #-   maybe check if FB update

 #    ---display all output in  web browser? a directory etc? a 

import webbrowser 

stock_page = webbrowser.open(" https://www.google.com/finance?q=t&ei=vQwNV7DvKdXCU4CBv9AB")
print stock_page #when program was run output = true     
T_stock =  stock_page.find("ref_33312_l") # no good as stock)_page is a boolean, does not contaian the text.

#in chrome highlight the stock price, right click and inspect element. note it is in "price-panel" div. span id appears to # #contain a #number for the stock VZ=   "ref_664887_1" T= "ref_33312_1" for T
#<span id=ref_33312_l>38.69</span>  

so above does not work as the variable stock_page is a Boolean so you cant serach it for text. Need a new aapproach
