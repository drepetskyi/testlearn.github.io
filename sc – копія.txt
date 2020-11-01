$(document).ready(function(){

    let param=document.getElementsByClassName('platform');
    let tlo=document.getElementsByClassName('tlo');
    let close=document.getElementsByClassName('close');


    for (let i=0; i < param.length; i++){
        param[i].addEventListener('click', showParam);
        let tlo1 = tlo[i];
        let close1 = close[i];

    function showParam(){

        if( $(close1).is(':hidden')){
            $(tlo1).fadeIn(600);
            $(close1).fadeIn(600);
        }
        else {$(tlo1).fadeOut(600);
            $(close1).fadeOut(600);}

    };

    };
 
    for (let i=0; i < tlo.length; i++){
        close[i].addEventListener('click', showParam1);
        let tlo1 = tlo[i];
        let close1 = close[i];

    function showParam1(){
            $(tlo1).fadeOut(600);
            $(close1).fadeOut(600);
        }

    };
    
})