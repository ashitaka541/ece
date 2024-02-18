<script>
	export let pg = 'EcE';
  </script>
  
  <svelte:head>
	<title>{pg}</title>
  </svelte:head>
  
  <style>
	.container {
	  position: relative; /* Needed for absolute positioning of child elements */
	  height: 100vh;
	  width: 100%; /* Ensure the container spans the full width */
	}
  
	.card {
	  position: absolute; /* Position the card absolutely within the container */
	  top: 4em; /* Adjust the distance from the top */
	  left: 45em; /* Adjust the distance from the right */
	  width: auto; /* Adjust based on content size */
	  padding: 1em; /* Adjust padding around card content */
	  display: inline-flex; /* Make card size adjust to content */
	  flex-direction: column; /* Align children vertically */
	}
  
	.card-header {
	  font-weight: bold;
	  text-align: center;
	  font-size: 2em; /* Makes the header bold and larger */
	  margin-bottom: 0.5em; /* Reduces space below header */
	}
	
	p {
	  text-align: center; /* Centers the text */
	  font-size: 0.9em; /* Smaller font size */
	  margin-top: 0; /* Removes top margin */
	  margin-bottom: 1em; /* Standardizes bottom margin */
	}
  
	ul {
	  padding-left: 20px; /* Adjusts padding for list */
	  margin-top: 0; /* Adjusts spacing to fit content */
	}
  
	.btn {
	  margin-top: 0.5em; /* Adjusts button position to better fit card */
	}
  
	/* Add responsive styles as needed */
	@media (max-width: 768px) {
	  /* Adjust the positioning on smaller screens */
	  .card {
		top: auto;
		right: auto;
		bottom: 1em; /* Position at the bottom for mobile */
		left: 1em; /* Align to the left for mobile */
	  }
	}
  </style>
  
  <div class="container">
	<div class="card card-hover bg-gradient-to-br variant-gradient-secondary-teritary">
	  <header class="card-header">Welcome to EcE</header>
	  <section class="p-4">
		<p>Where innovation meets social justice</p>
		<div class="flex justify-center space-x-2">
		  <a
			class="btn btn-sm bg-gradient-to-br variant-gradient-primary-secondary"
			href="/about"
			target="_blank"
			rel="noreferrer"
		  >
			Click Me!!
		  </a>
		</div>
		<ul>
		  <li><code class="code">Skilify</code> ~ Level up your skills anytime anywhere.</li>
		  <li><code class="code">The Hub</code> ~ A Vital Villages Collaboration ~ Resource Center </li>
		  <li><code class="code">Chat</code> ~ Chat with a custom AI</li>
		  <li><code class="code">Resume Builder</code> ~ Build A Resume.</li>
		</ul>
	  </section>
	</div>
  </div>
  