<script>
    import {browser} from "$app/environment"
    let ids = ["name", "email", "grade", "llvm"]
    export let data;
    console.log(data.llvm)
    if (browser) {
        setInterval(() => {
            let butto = document.getElementById("submit")
            let total = true
            for (let i = 0; i < ids.length; i++) {
                let id = ids[i]
                let element = document.getElementById(id)
                if (element.value === "") {

                    butto.disabled = true
                    //butto.style.backgroundColor = "black"
                    total = false
                }
            }
            if (total) {
                butto.disabled = false
                butto.style.backgroundColor = "white"
            }
        }, 20)


    } //very bad for performance
    /** @type {import('./$types').ActionData} */
    export let form;
    if (form?.gcc) {
        if (browser) {
            window.location.href = "/"
            alert(form?.llvm)
            window.localStorage.setItem("email", form?.email)
        }

    }
</script>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Apply</title>
</head>
<body class="overflow-x-hidden overflow-y-auto w-screen h-screen bg-gradient-to-b from-black to-indigo-900">
    <div class="navbar bg-gray-900 fixed top-0 w-full z-20">
		<div class="navbar-start">
		  <div class="dropdown">
			<div tabindex="0" role="button" class="btn btn-ghost lg:hidden">
			  <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h8m-8 6h16" /></svg>
			</div>
			<ul tabindex="0" class="menu menu-sm dropdown-content mt-3 z-[1] p-2 shadow bg-base-100 rounded-box w-52">
				<li><a href="/#FAQ">FAQ</a></li>
				<li><a href="/#GS">Guest Speakers</a></li>
				<li><a href="/#SCHED">Schedule</a></li>
				<li><a href="/apply">Apply</a></li>
			</ul>
		  </div>
		  <a class="btn btn-ghost text-xl" href="/">ManeFrame</a>
		  <div class="w-10 rounded-full size-10">
			<img alt="ManeFrame" src="/img.png" />
		  </div>
		</div>
		<div class="navbar-center hidden lg:flex">
		  <ul class="menu menu-horizontal px-1">
			<li><a href="/#FAQ">FAQ</a></li>
			<li><a href="/#GS">Guest Speakers</a></li>
			<li><a href="/#SCHED">Schedule</a></li>
			<li><a href="/apply">Apply</a></li>
		  </ul>
		</div>
		<div class="navbar-end">
			<div class="w-10 rounded-full mr-2">
				<a href="https://discord.gg/JSRUHBAG" target="_blank">
					<img alt="DC" src="/icons8-discord-48.png" />
				</a>
			</div>
			<div class="w-10 rounded-full mr-2">
				<a href="https://instagram.com/maneframe2024" target="_blank">
					<img alt="IG" src="/icons8-instagram-48.png" />
				</a>
			</div>
			<div class="w-10 rounded-full mr-10">
				<a href="mailto:maneframe24@gmail.com" target="_blank">
					<img alt="SMTP" src="/icons8-email-48.png" />
				</a>
			</div>
		</div>
	  </div>
<div class="z-30 w-screen h-2/5 text-center content-center justify-center relative row-start-1">
    <h1 class="text-7xl font-bold text-center animate-pulse text-white m-20 z-0 mt-32">Apply</h1>
    <div class="flex content-center justify-center items-center">
        <div class="card w-96 glass shadow-xl mb-20">
            <div class="card-body">
                <h2 class="font-bold text-2xl text-white">Sign Up!</h2>
                <h1 class="font-bold text-md text-white">June 15th, 9:30 AM to 5:00 PM</h1>
                <h1 class="font-bold text-md text-white">MLK Library, San Jose State University</h1>
                <!------>
                <form method="POST">
                    <label class="form-control w-full max-w-xs">
                        <div class="label">
                            <span class="text-xs text-white">What's your full name?</span>
                        </div>
                        <input type="text" placeholder="Name" class="input input-bordered" name="name" id="name">
                    </label>
                    <br>
                    <br>
                    <label class="form-control w-full max-w-xs">
                        <div class="label">
                            <span class="text-xs text-white">What's your email?</span>
                        </div>
                        <input type="text" placeholder="We promise no spam!" class="input input-bordered" name="email" id="email">
                    </label>
                    <br>
                    <br>
                    <label class="form-control w-full max-w-xs">
                        <div class="label">
                            <span class="text-xs text-white">What grade are you in?</span>
                        </div>
                        <input type="text" placeholder="e.g. 10th, 11th" class="input input-bordered" name="grade" id="grade">
                    </label>
                    <br>
                    <br>
                    <label class="form-control w-full max-w-xs">
                        <div class="label">
                            <span class="text-xs text-white">Any Dietary Restrictions?</span>
                        </div>
                        <input type="text" placeholder="e.g. vegan" class="input input-bordered" name="diet" id="llvm">
                    </label>
                <br>
                <br>
                <div class="card-actions justify-center">
                    <button class="btn glass" id="submit">SUBMIT!</button>
                    <h1 class="text-sm text-white">This will redirect you back to the home page. Remember to check your email!</h1>
                </div>
                </form>
            </div>
        </div>
    </div>

</div>
</body>
</html>