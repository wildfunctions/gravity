<!DOCTYPE html>
<html>
    <head>
        <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
        <title></title>
    </head>
    <body>
        <canvas id="canvas" width="500" height="500"></canvas>
        <div id="stats"></div>
    </body>
</html>

<script type="text/javascript">
    var canvas = document.getElementById('canvas');
    var context = canvas.getContext('2d');
    var centerX = canvas.width / 2;
    var centerY = canvas.height / 2;
    
    //var a = 149.60 * 1000000; //earth's semi-major axis
    var a = 60; //semi-major axis
    //var e = 0.0167; //earth's eccentricity
    var e = 0.6; //eccentricity
    var n = 10; //number of orbits desired
    var stepSize = 100;
    var t_init = 0;
    var t = t_init;
    var t_max = n*Math.sqrt(a*a*a); //since (period)^2 ~ a^3 from Kepler's 3rd Law
    var dt = t_max/(n*stepSize);
    
    var GM = 39.4784176;
    var g = GM/a;

    var v = new Array(0, Math.sqrt((g*(1-e))/(1+e)), 0);
    var pos = new Array(a*(1+e), 0, 0);
    
    var run = function() {
        if(t <= t_max) {
            t += dt;
            for(var i = 0; i < 3; i++) {
                pos[i] += v[i]*dt/2;
            }
        
            r = Math.sqrt(pos[0]*pos[0] + pos[1]*pos[1]);
            r3 = r*r*r;
        
            var acc = new Array(0, 0, 0);
            for(var i = 0; i < 3; i++) {
                acc[i] = (-GM/r3) * pos[i];
            }
        
            for(var i = 0; i < 3; i++) {
                v[i] += acc[i]*dt;
                pos[i] += v[i]*(dt/2);
            }
            
            var statsDiv = document.getElementById("stats");
            statsDiv.innerHTML = "Orbits: " + Math.round(t*100/Math.sqrt(a*a*a))/100 + " Velcity: " + Math.round(Math.sqrt(v[0]*v[0] + v[1]*v[1])*100)/100;
            
            context.fillStyle   = '#151515';
            context.fillRect  (0,  0, 500, 500);
            
            drawObject(0, 0, 'yellow', '#FFA500', 10); //sun
            drawObject(pos[0], pos[1], '#00FFFF', '#003300', 2); //earth
        }
    }
    
    var drawObject = function(x, y, coreColor, strokeColor, radius) {
        x = centerX + x;
        y = centerY + y;
        context.beginPath();
        context.arc(x, y, radius, 0, 2 * Math.PI, false);
        context.fillStyle = coreColor;
        context.fill();
        context.lineWidth = 1;
        context.strokeStyle = strokeColor;
        context.stroke();
    }
    
    setInterval(run, 1000/50);
</script>