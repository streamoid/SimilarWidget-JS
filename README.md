**SimilarWidget-JS**
===============

Using ***SimilarWidget-JS*** sdk fashion websites can add a widget into their product detail page which will show all products visually similar to the product in display
 
  **Integration**
  
 1) Adding script in **head** tag


    (function(i,s,o,g,r,t,k,a,m){
     i['PiqitObject']=r;i['PiqitGa']=t;i['PiqitToken'] = k;i[r]=i[r]||function() {
     (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
     m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
     })(window, document, 'script', 'LOADER URL', 'PQT', 'GOOGLEANALYTICS-ID', 'CLIENT TOKEN');

  **Important Note** : If you are already using some other Streamoid's JS sdk in your website, you need not add the above script in **head** tag twice

 2) Add the below line of code(div) in your html source wherever you want to see the similar widget. Client website has to  programatically assign the values for PRODUCT ID, PRODUCT IMAGE URL on loading the product detail page

    <div class="streamoid_sdk" data-service="similar" data-token="CLIENT TOKEN" data-function="initialize" data-product="PRODUCT ID" data-fallback="PRODUCT IMAGE URL"></div>

    
Please contact streamoid.support@streamoid.com to get LOADER URL,CLIENT TOKEN, GA TRACKER-ID
