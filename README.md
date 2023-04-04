# checkpoint-algorithm
VAR
    ch:STRING;
    nbW,nbV,i:INTEGER;
BEGIN
    write("Please enter your message");
    read(ch);
    nbW,nbV:=0;
    max:=ch.length;
     
WHILE (ch[max]=".") DO
    
    FOR i FROM 0 TO max-1 STEP step  DO
        IF (ch[i] in ("a","e","i","o","u")) or (ch[i] in ("A","E","I","O","U")) THEN
            nbV:=nbV+1;
        END_IF    
    END_FOR
    FOR i FROM 1 TO max STEP step  DO
        IF (ch[i])="" THEN
            nbw:=nbw+1;
        END_IF    
    END_FOR


END_WHILE
    write('the number of words is', nbW);
    write('the number of vowels is', nbV);
END.
