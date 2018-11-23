# ICS-02-Summative--Paige-Leena-Raiqah
Grade 3 game information.
https://docs.google.com/document/d/1BDN1UOa2PsHfQe8BMaAoyDuvldLp8jTHMbWcbeMlMcI/edit

code prototype for game

var currentScene;

var drawScene1 = function() {
    currentScene = 1;
    background(180, 250, 247);
    noStroke();
    fill(67, 184, 0);
    ellipse(360,380,5007,259);
    fill(255, 234, 0);
    ellipse(21,35,100,100);
    fill(0, 0, 0);
    rect(131,122,150,60);
    fill(255, 255, 255);
    textSize(45);
    text("Start", 153,165);
    
   
};

var drawScene2 = function() {
    currentScene = 2;
      background(129, 243, 247);
noStroke();
var x= 146;
var y=105;
var x2=122;
var y2=149;
fill(44, 166, 13);
ellipse(207,348,498,210);
fill(255, 255, 255);
rect(111,74,232,293);
fill(0, 0, 0);
textSize(30);
text("Instructions",x,y);
textSize(11);
text("Avoid obsticles in each stage.",x2-5,y2);
text("Must do math problem if level not passed",x2-7,y2+31);
text("If level complete, collect points and move on.",x2-8,y2+73);
fill(0, 0, 0);
rect(176,284,87,40);
fill(250, 250, 250);
textSize(16);
text("Okay",x+53,y+203);
fill(255, 255, 0);
ellipse(26,43,109,109);

};

var drawScene3 = function() {
    
    background(153, 248, 255);
    noStroke();
    fill(0, 173, 12);
    rect(2,236,1390,1400);
    fill(255, 255, 0);
    ellipse(20,20,100,100);
    fill(209, 202, 202);
    rect(33,92,150,200);
    rect(237,92,150,200);

    
};

var drawScene4= function(){
    background(224, 196, 16);
    fill(124, 21, 219);
    ellipse(200,200,10,20);
   
};

var drawScene5= function(){
    background(255, 0, 0);
    fill(0, 0, 0);
    rect(200,100,100,100);
};

mouseClicked = function() {
    if (currentScene === 1) {
        drawScene2();
    } else if (currentScene === 2) {
        drawScene3();
    } else if (currentScene === 3) {
        drawScene4();
    } else if (currentScene === 4){
        drawScene5();
    } else if (currentScene === 5){
        drawScene1();
    }
     
};

drawScene1();
//drawScene2();
