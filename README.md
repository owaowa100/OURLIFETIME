<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/easytimer@1.1.1/src/easytimer.min.js"></script>

<html>

<head>
   
    <title>Timer</title>
</head>

<body>   
   <div id="secondTenthsExample">
   <span class="hours">0</span><span>:</span><span class="values">243:20::00</span>

</div>
   <!-- You can change from what time it will start counting up, just put in specific time to replace 00. If you want to start from 5 mins up, just put 05 (ex) minutes: 05 -->
    <script src="easytimer.js"></script>
    <script>
        var timer = new Timer();
        timer.start({precision: 'secondTenths', startValues: {secondTenths: 00, seconds: 00, minutes: 00, hours: 00, days: 243}}, );
        timer.addEventListener('secondTenthsUpdated', function (e) {
        $('#secondTenthsExample .hours').html(timer.getTotalTimeValues().hours);
        $('#secondTenthsExample .values').html(timer.getTimeValues().toString(['minutes', 'seconds', 'secondTenths']));
});            
    </script>
</body>
</html>
