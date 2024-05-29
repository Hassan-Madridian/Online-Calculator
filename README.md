#java script

<title>Online Calculator</title> <style> table { margin: auto; border-collapse: collapse; } input[type=text] { width: 100%; text-align: right; font-size: 2em; } button { width: 100%; height: 50px; font-size: 1.5em; } </style>
1	2	3	+
4	5	6	-
7	8	9	*
0	.	=	/
C
<script>
    function main(key) {
        var screen = document.getElementById("screen");
        screen.value = screen.value + key;
    }

    function calculate() {
        var screen = document.getElementById("screen");
        try {
            screen.value = eval(screen.value);
        } catch (e) {
            screen.value = "Error";
        }
    }

    function clearScreen() {
        document.getElementById("screen").value = "";
    }
</script>
