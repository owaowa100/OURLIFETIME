<div class="wrapper">
<div class="header"> You are watching this for: </div>
    <div class="counter-container">
        <div class="min-container">
            <div class="digit-container">
                <div class="digit-upper min2upper"></div>
                <div class="digit-lower min2lower"></div>
            </div>
            <div class="digit-container">
                <div class="digit-upper min1upper"></div>
                <div class="digit-lower min1lower"></div>
            </div>
        </div>

        <div class="min-text-container">
            <span class="unit"> Min </span>
        </div>

        <div class="sec-container">
            <div class="digit-container">
                <div class="digit-upper sec2upper"></div>
                <div class="digit-lower sec2lower"></div>
            </div>
            <div class="digit-container">
                <div class="digit-upper sec1upper"></div>
                <div class="digit-lower sec1lower"></div>
            </div>
        </div>

    <div class="sec-text-container">
       <span class="unit"> Sec </span>
    </div>
</div>
* {
    margin: 0;
    padding: 0;
    font-family: sans-serif;
}

html {
    height: 100%;
}

body {
    width: 100%;
    height: 100%;
    padding: 0;
    margin: 0;
    overflow: hidden;
    background: #bb71f3;
    background: -moz-linear-gradient(-45deg,#09203f 0%,#537895 100%);
    background: -webkit-linear-gradient(-45deg,#09203f 0%,#537895 100%);
    background: linear-gradient(135deg,#09203f 0%,#537895 100%);
    filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#bb71f3',endColorstr='#3d4d91',GradientType=1);
    font-family: helvetica neue,futura,trebuchet ms,Arial;
    -webkit-user-select: none;
    user-select: none;
    -webkit-tap-highlight-color: transparent;
    color: white;
}

.counter-container {
    position: absolute;
    height: 50%;
    width: 85%;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}

.min-container, .sec-container {
    width: 35%;
    float: left;
    height: 100%
}

.min-text-container, .sec-text-container {
    width: 15%;
    float: left;
    height: 100%;
    line-height: 50%;
    font-size: 500%;
    line-height: 264px;
    font-weight: bolder;
    text-align: center;
}

.digit-container {
    float: left;
    width: 40%;
    margin-left: 8%;
    height: 100%;
}

.digit-upper{
    height: 49%;
    width: 98%;
    animation-iteration-count: infinite;
}

.digit-lower{
    height: 49%;
    width: 98%;
    animation-iteration-count: infinite;
}

.header {
    font-size: 32px;
    padding-top: 12px;
    text-align: center;
}

.sec1upper, .sec1lower{animation-duration: 10s;}

.sec1upper {animation-name: animate-upper-sec1}
.sec1lower {animation-name: animate-lower-sec1}

.sec2upper, .sec2lower{animation-duration: 60s;}

.sec2upper {animation-name: animate-upper-sec2}
.sec2lower {animation-name: animate-lower-sec2}

.min1upper, .min1lower {animation-duration: 600s}

.min1upper {animation-name: animate-upper-min1}
.min1lower {animation-name: animate-lower-min1}

.min2upper, .min2lower {animation-duration: 6000s}

.min2upper {animation-name: animate-upper-min2}
.min2lower {animation-name: animate-lower-min2}

@keyframes animate-upper-sec1 {
    0% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid transparent}
    1% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid transparent; border-bottom: 12px solid transparent}

    10% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid transparent; border-bottom: 12px solid transparent}
    11% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}

    20% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}
    21% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}

    30% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}
    31% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid transparent; border-bottom: 12px solid white}

    40% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid transparent; border-bottom: 12px solid white}
    41% {border-left: 12px solid white; border-right: 12px solid transparent; border-top: 12px solid white; border-bottom: 12px solid white}

    50% {border-left: 12px solid white; border-right: 12px solid transparent; border-top: 12px solid white; border-bottom: 12px solid white}
    51% {border-left: 12px solid white; border-right: 12px solid transparent; border-top: 12px solid white; border-bottom: 12px solid white}

    60% {border-left: 12px solid white; border-right: 12px solid transparent; border-top: 12px solid white; border-bottom: 12px solid white}
    61% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid transparent}

    70% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid transparent}
    71% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}

    80% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}
    81% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}

    90% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}
    91% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid transparent}

    100% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid transparent}
}

@keyframes animate-lower-sec1 {
    0% {border-left: 12px solid white; border-right: 12px solid white; border-bottom: 12px solid white}
    1% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid transparent}

    10% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid transparent}
    11% {border-left: 12px solid white; border-right: 12px solid transparent;  border-bottom: 12px solid white}

    20% {border-left: 12px solid white; border-right: 12px solid transparent;  border-bottom: 12px solid white}
    21% {border-left: 12px solid transparent; border-right: 12px solid white;  border-bottom: 12px solid white}

    30% {border-left: 12px solid transparent; border-right: 12px solid white;  border-bottom: 12px solid white}
    31% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid transparent}

    40% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid transparent}
    41% {border-left: 12px solid transparent; border-right: 12px solid white;  border-bottom: 12px solid white}

    50% {border-left: 12px solid transparent; border-right: 12px solid white;  border-bottom: 12px solid white}
    51% {border-left: 12px solid white; border-right: 12px solid white;  border-bottom: 12px solid white}

    60% {border-left: 12px solid white; border-right: 12px solid white;  border-bottom: 12px solid white}
    61% {border-left: 12px solid transparent; border-right: 12px solid white;  border-bottom: 12px solid transparent}

    70% {border-left: 12px solid transparent; border-right: 12px solid white;  border-bottom: 12px solid transparent}
    71% {border-left: 12px solid white; border-right: 12px solid white;  border-bottom: 12px solid white}

    80% {border-left: 12px solid white; border-right: 12px solid white;  border-bottom: 12px solid white}
    81% {border-left: 12px solid transparent; border-right: 12px solid white;  border-bottom: 12px solid white}

    90% {border-left: 12px solid transparent; border-right: 12px solid white;  border-bottom: 12px solid white}
    91% {border-left: 12px solid white; border-right: 12px solid white; border-bottom: 12px solid white}

    100% {border-left: 12px solid white; border-right: 12px solid white; border-bottom: 12px solid white}
}

@keyframes animate-upper-sec2 {
    0% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid transparent}

    14.66% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid transparent}
    15.66% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid transparent; border-bottom: 12px solid transparent}

    31.33% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid transparent; border-bottom: 12px solid transparent}
    32.33% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}

    47.98% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}
    48.98% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}

    64.64% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}
    65.64% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid transparent; border-bottom: 12px solid white}

    81.3% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid transparent; border-bottom: 12px solid white}
    82.3% {border-left: 12px solid white; border-right: 12px solid transparent; border-top: 12px solid white; border-bottom: 12px solid white}

    97.5% {border-left: 12px solid white; border-right: 12px solid transparent; border-top: 12px solid white; border-bottom: 12px solid white}
    98.5% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid transparent}
    100% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid transparent}
}

@keyframes animate-lower-sec2 {
    0% {border-left: 12px solid white; border-right: 12px solid white; border-bottom: 12px solid white}

    14.66% {border-left: 12px solid white; border-right: 12px solid white; border-bottom: 12px solid white}
    15.66% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid transparent}

    31.33% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid transparent}
    32.33% {border-left: 12px solid white; border-right: 12px solid transparent;  border-bottom: 12px solid white}

    47.98% {border-left: 12px solid white; border-right: 12px solid transparent;  border-bottom: 12px solid white}
    48.98% {border-left: 12px solid transparent; border-right: 12px solid white;  border-bottom: 12px solid white}

    64.64% {border-left: 12px solid transparent; border-right: 12px solid white;  border-bottom: 12px solid white}
    65.64% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid transparent}

    81.3% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid transparent}
    82.3% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid white}

    97.5% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid white}
    98.5% {border-left: 12px solid white; border-right: 12px solid white; border-bottom: 12px solid white}
    100% {border-left: 12px solid white; border-right: 12px solid white; border-bottom: 12px solid white}
}

@keyframes animate-upper-min1 {
    0% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid transparent}

    9.9% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid transparent}
    10% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid transparent; border-bottom: 12px solid transparent}

    19.9% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid transparent; border-bottom: 12px solid transparent}
    20% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}

    29.9% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}
    30% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}

    39.9% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}
    40% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid transparent; border-bottom: 12px solid white}

    49.9% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid transparent; border-bottom: 12px solid white}
    50% {border-left: 12px solid white; border-right: 12px solid transparent; border-top: 12px solid white; border-bottom: 12px solid white}

    59.9% {border-left: 12px solid white; border-right: 12px solid transparent; border-top: 12px solid white; border-bottom: 12px solid white}
    60% {border-left: 12px solid white; border-right: 12px solid transparent; border-top: 12px solid white; border-bottom: 12px solid white}

    69.9% {border-left: 12px solid white; border-right: 12px solid transparent; border-top: 12px solid white; border-bottom: 12px solid white}
    70% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid transparent}

    79.9% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid transparent}
    80% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}

    89.9% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}
    90% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}

    99.9% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}
    100% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid transparent}
}

@keyframes animate-lower-min1 {
    0% {border-left: 12px solid white; border-right: 12px solid white; border-bottom: 12px solid white}

    9.9% {border-left: 12px solid white; border-right: 12px solid white; border-bottom: 12px solid white}
    10% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid transparent}

    19.9% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid transparent}
    20% {border-left: 12px solid white; border-right: 12px solid transparent;  border-bottom: 12px solid white}

    29.9% {border-left: 12px solid white; border-right: 12px solid transparent;  border-bottom: 12px solid white}
    30% {border-left: 12px solid transparent; border-right: 12px solid white;  border-bottom: 12px solid white}

    39.9% {border-left: 12px solid transparent; border-right: 12px solid white;  border-bottom: 12px solid white}
    40% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid transparent}

    49.9% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid transparent}
    50% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid white}

    59.9% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid white}
    60% {border-left: 12px solid white; border-right: 12px solid white; border-bottom: 12px solid white}

    69.9% {border-left: 12px solid white; border-right: 12px solid white; border-bottom: 12px solid white}
    70% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid transparent}

    79.9% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid transparent}
    80% {border-left: 12px solid white; border-right: 12px solid white; border-bottom: 12px solid white}

    89.9% {border-left: 12px solid white; border-right: 12px solid white; border-bottom: 12px solid white}
    90% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid white}

    99.9% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid white}
    100% {border-left: 12px solid white; border-right: 12px solid white; border-bottom: 12px solid white}
}
/*******************************************************************************************************/
@keyframes animate-upper-min2 {
    0% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid transparent}

    9.9% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid transparent}
    10% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid transparent; border-bottom: 12px solid transparent}

    19.9% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid transparent; border-bottom: 12px solid transparent}
    20% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}

    29.9% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}
    30% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}

    39.9% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}
    40% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid transparent; border-bottom: 12px solid white}

    49.9% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid transparent; border-bottom: 12px solid white}
    50% {border-left: 12px solid white; border-right: 12px solid transparent; border-top: 12px solid white; border-bottom: 12px solid white}

    59.9% {border-left: 12px solid white; border-right: 12px solid transparent; border-top: 12px solid white; border-bottom: 12px solid white}
    60% {border-left: 12px solid white; border-right: 12px solid transparent; border-top: 12px solid white; border-bottom: 12px solid white}

    69.9% {border-left: 12px solid white; border-right: 12px solid transparent; border-top: 12px solid white; border-bottom: 12px solid white}
    70% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid transparent}

    79.9% {border-left: 12px solid transparent; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid transparent}
    80% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}

    89.9% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}
    90% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}

    99.9% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid white}
    100% {border-left: 12px solid white; border-right: 12px solid white; border-top: 12px solid white; border-bottom: 12px solid transparent}
}

@keyframes animate-lower-min2 {
    0% {border-left: 12px solid white; border-right: 12px solid white; border-bottom: 12px solid white}

    9.9% {border-left: 12px solid white; border-right: 12px solid white; border-bottom: 12px solid white}
    10% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid transparent}

    19.9% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid transparent}
    20% {border-left: 12px solid white; border-right: 12px solid transparent;  border-bottom: 12px solid white}

    29.9% {border-left: 12px solid white; border-right: 12px solid transparent;  border-bottom: 12px solid white}
    30% {border-left: 12px solid transparent; border-right: 12px solid white;  border-bottom: 12px solid white}

    39.9% {border-left: 12px solid transparent; border-right: 12px solid white;  border-bottom: 12px solid white}
    40% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid transparent}

    49.9% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid transparent}
    50% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid white}

    59.9% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid white}
    60% {border-left: 12px solid white; border-right: 12px solid white; border-bottom: 12px solid white}

    69.9% {border-left: 12px solid white; border-right: 12px solid white; border-bottom: 12px solid white}
    70% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid transparent}

    79.9% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid transparent}
    80% {border-left: 12px solid white; border-right: 12px solid white; border-bottom: 12px solid white}

    89.9% {border-left: 12px solid white; border-right: 12px solid white; border-bottom: 12px solid white}
    90% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid white}

    99.9% {border-left: 12px solid transparent; border-right: 12px solid white; border-bottom: 12px solid white}
    100% {border-left: 12px solid white; border-right: 12px solid white; border-bottom: 12px solid white}
}
