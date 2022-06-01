welcome 
import wixAnimations from 'wix-animations';


$w.onReady(function () {

    activateBackgroundAnimation();
 

});

function activateBackgroundAnimation() {

    let backgroundImage = $w('#backgroundImg');
    let timeline = wixAnimations.timeline({
            repeat: -1,
            "yoyo": true
        })
        .add(backgroundImage, {
            scale: 1.8,
            rotate: 45,
            x: 100,
            duration: 15000
        });

    timeline.play();
}
