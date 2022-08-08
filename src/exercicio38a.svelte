<script>
	import {time} from "./exercicio38b";

	const formatter = new Intl.DateTimeFormat("en", {
		hour12: true,
		hour: "numeric",
		minute: "2-digit",
		second: "2-digit"
	});
</script>

<h1>Hora certa: {formatter.format($time)}</h1>