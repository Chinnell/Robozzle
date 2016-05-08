# Robozzle
robozzle.com games made into JS code.

//game link on robozzle: http://robozzle.com/js/play.aspx?puzzle=27

var instructions= [];
var blueSteps = ["x"];
function pushB(){
	for (i=0; i<19; i++){
		
	blueSteps.push("b");
	}
}

pushB();


function stairs(blueStairs){
	console.log ("moveForward");
	instructions.push("moveForward");
	for(i=1; i<(blueStairs.length-1); i++){
		if (i % 2 == 1){
			console.log("turnLeft and moveForward");
			instructions.push("turn left");
			instructions.push("move forward");
		}
		else {
			console.log("turnRight and moveForward");
			instructions.push("turn right");
			instructions.push("move forward");
		
		}
}

	
}

stairs(blueSteps);
instructions.length;
