#Ti.ToneGenerator

This Titanium module for Android generates tones.

##Usage:

```javascript

var TonGen = require("de.appwerft.tonegenerator");


var peep = TonGen.createTone({
    duration : 1000,
    frequence : 440.0,
    volume : 0.5
});

var button = Ti.UI.createButton({
    title : "Kammerton a"
});

button.addEventListener("click",function(){
    peep.play();
})

