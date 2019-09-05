# utl-Graph-with-known-intercept-and-slope
Graph with known intercept and slope 

    Graph with known intercept and slope                                                                       
                                                                                                               
    I did not know that.                                                                                       
                                                                                                               
    github                                                                                                     
    https://github.com/rogerjdeangelis/utl-Graph-with-known-intercept-and-slope                                
                                                                                                               
    Graphic                                                                                                    
    https://tinyurl.com/y595nps6                                                                               
    https://github.com/rogerjdeangelis/utl-Graph-with-known-intercept-and-slope/blob/master/line.pdf           
                                                                                                               
    SAS forum                                                                                                  
    https://tinyurl.com/y69qvhpj                                                                               
    https://communities.sas.com/t5/Graphics-Programming/Graph-with-known-intercept-and-slope/m-p/585737        
                                                                                                               
    PaigeMiller Profile                                                                                        
    https://communities.sas.com/t5/user/viewprofilepage/user-id/10892                                          
                                                                                                               
    *_                   _                                                                                     
    (_)_ __  _ __  _   _| |_                                                                                   
    | | '_ \| '_ \| | | | __|                                                                                  
    | | | | | |_) | |_| | |_                                                                                   
    |_|_| |_| .__/ \__,_|\__|                                                                                  
            |_|      _           ___                                                                           
     _   _   _____  / |    _    |___ \  __  __                                                                 
    | | | | |_____| | |  _| |_    __) | \ \/ /                                                                 
    | |_| | |_____| | | |_   _|  / __/   >  <                                                                  
     \__, |         |_|   |_|   |_____| /_/\_\                                                                 
     |___/                                                                                                     
    ;                                                                                                          
                                                                                                               
    *            _               _                                                                             
      ___  _   _| |_ _ __  _   _| |_                                                                           
     / _ \| | | | __| '_ \| | | | __|                                                                          
    | (_) | |_| | |_| |_) | |_| | |_                                                                           
     \___/ \__,_|\__| .__/ \__,_|\__|                                                                          
                    |_|                                                                                        
    ;                                                                                                          
                                                                                                               
                                                                                                               
    21 +                    /                                                                                  
    20 +                   /                                                                                   
    19 +                  /                                                                                    
    18 +   Y = 1 + 2x    /                                                                                     
    17 +                /                                                                                      
    16 +               /                                                                                       
    15 +              /                                                                                        
    14 +             /                                                                                         
    13 +            /                                                                                          
    12 +           /                                                                                           
    11 +          /                                                                                            
    10 +         /                                                                                             
     9 +        /                                                                                              
     8 +       /                                                                                               
     7 +      /                                                                                                
     6 +     /                                                                                                 
     5 +    /                                                                                                  
     4 +   /                                                                                                   
     3 +  /                                                                                                    
       |                                                                                                       
       -+---------+---------+--                                                                                
        0         5        10                                                                                  
                                                                                                               
                    X                                                                                          
                                                                                                               
    *                                                                                                          
     _ __  _ __ ___   ___ ___  ___ ___                                                                         
    | '_ \| '__/ _ \ / __/ _ \/ __/ __|                                                                        
    | |_) | | | (_) | (_|  __/\__ \__ \                                                                        
    | .__/|_|  \___/ \___\___||___/___/                                                                        
    |_|                                                                                                        
    ;                                                                                                          
                                                                                                               
                                                                                                               
    ods pdf file="d:/pdf/line.pdf";                                                                            
    proc sgplot data=sashelp.class;                                                                            
    scatter x=height y=weight/transparency=1;                                                                  
    lineparm x=0 y=1 slope=2;                                                                                  
    xaxis min=0 max=10 label='Timepoint';                                                                      
    yaxis min=0 max=21 label='Y';                                                                              
    run;quit;                                                                                                  
    ods pdf close;                                                                                             
                                                                                                               
    *               _ _         _       _                                                                      
      __ _ ___  ___(_|_)  _ __ | | ___ | |_                                                                    
     / _` / __|/ __| | | | '_ \| |/ _ \| __|                                                                   
    | (_| \__ \ (__| | | | |_) | | (_) | |_                                                                    
     \__,_|___/\___|_|_| | .__/|_|\___/ \__|                                                                   
                         |_|                                                                                   
    ;                                                                                                          
                                                                                                               
    data have;                                                                                                 
      do x=1 to 10 by .5;                                                                                      
         y=1+2*x;                                                                                              
         output;                                                                                               
      end;                                                                                                     
    run;quit;                                                                                                  
                                                                                                               
    options ls=64 ps=32;                                                                                       
    proc plot data=have(rename=y=y1234567890123456789012345678901);                                            
     plot y1234567890123456789012345678901*X="/";                                                              
    run;quit;                                                                                                  
    options ls=171;                                                                                            
                                                                                                               
