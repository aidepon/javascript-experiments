var flipCoin = function(){if(Math.random() > 0.5){return true;} else {return false;}} 
var text = " drop drop drop drop drop "; 
var myIntervalTimer = setInterval(function(){text += " ";if(text.length > 50){text = " drop drop drop drop drop ";}if(flipCoin()){console.log('%c'+text, 'background: yellow; color: black; font-size: '+Math.round(Math.random()*50)+'px;');} else {console.log('%c'+text, 'background: black; color: white; font-size: '+Math.round(Math.random()*50)+'px;');}}, 15); 
setTimeout(function(){clearInterval(myIntervalTimer);}, 1000 * 20);
