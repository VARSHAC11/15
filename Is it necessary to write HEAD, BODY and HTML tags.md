Is it necessary to write HEAD, BODY and HTML tags?
no they are not necessary,even without these tags html works fine,but the structure of DOM tree differs
Eg:
<!DOCTYPE html>
<title>Test case</title>
<form action='#'>
   <input name="var1">
</form>
Expected DOM Tree:
HTML
    HEAD
        TITLE
    BODY
        FORM action="#"
            INPUT name="var1
            
Actual DOM Tree:
HTML
    HEAD
       TITLE
       FORM action="#"
           BODY
               INPUT name="var1"
    BODY
