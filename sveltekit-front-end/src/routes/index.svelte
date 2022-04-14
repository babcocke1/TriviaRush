<script>
    import '../app.css';
    
    let play = "play";
    export const loadNextPage = () => {}
    
    let m = "ayooo";

    // socketio
    import { io } from "socket.io-client";
import { prevent_default } from "svelte/internal";

    // const socket = io("https://TriviaRush.ericbabcock.repl.co");

    let sendMessage = () => {
        // send a message to the server
        // socket.emit("message", m);
        console.log(m);
    }
    
</script>
<body>
	<div class="TitleImage">
		<img src="title.png" alt="Trivia Rush Logo">
	</div>
    <div class="container mx-auto">
        <div class="form-control  w-full max-w-xs mx-auto">
            <form class="label max-w-sm mx-auto" id="form1" on:submit|preventDefault>
                <input type="text" placeholder="What should we call you" 
                    class="input input-bordered "> 
                <button class="btn btn-ghost prompt border min-w-100" on:click={sendMessage} >{play}</button>
            </form >
        </div>
    </div>

    
</body>
<div class="bg">

</div>

<style>
	.TitleImage {
		width: 80%;
		margin-left: 10%;
	}
	img {
        margin: 0 auto;
		width:100%;
        max-width: 400px;
	}
    .prompt {
        color:#FFFFFF
    }
    .bg {
        position: absolute;
        height: 100%;
        width: 100%;
        top: 0;
        z-index: -1;
    	background: linear-gradient(81.32deg, #6D7CFF 34%, #F54968 66%);

    }


</style>
