
<script>
// Countdown Timer
window.addEventListener('DOMContentLoaded', (event) => {
    const deadline = new Date('2023-10-01T14:00:00').getTime();
    
    setInterval(() => {
        const now = new Date().getTime();
        const distance = deadline - now;

        const days = Math.floor(distance / (1000 * 60 * 60 * 24));
        const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
        const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
        const seconds = Math.floor((distance % (1000 * 60)) / 1000);
        
        document.querySelector('#js-timer-days').innerText = days;
        document.querySelector('#js-timer-hours').innerText = hours;
        document.querySelector('#js-timer-minutes').innerText = minutes;
        document.querySelector('#js-timer-seconds').innerText = seconds;

    }, 1000);
});

</script>
