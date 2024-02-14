<script lang="ts">
	import '../app.postcss';

	// Highlight JS
	import hljs from 'highlight.js/lib/core';
	import 'highlight.js/styles/github-dark.css';
	import { storeHighlightJs } from '@skeletonlabs/skeleton';
	import xml from 'highlight.js/lib/languages/xml'; // for HTML
	import css from 'highlight.js/lib/languages/css';
	import javascript from 'highlight.js/lib/languages/javascript';
	import typescript from 'highlight.js/lib/languages/typescript';

	hljs.registerLanguage('xml', xml); // for HTML
	hljs.registerLanguage('css', css);
	hljs.registerLanguage('javascript', javascript);
	hljs.registerLanguage('typescript', typescript);
	storeHighlightJs.set(hljs);

	// Floating UI for Popups
	import { computePosition, autoUpdate, flip, shift, offset, arrow } from '@floating-ui/dom';
	import { storePopup } from '@skeletonlabs/skeleton';
	import { AppShell }	from '@skeletonlabs/skeleton';
	storePopup.set({ computePosition, autoUpdate, flip, shift, offset, arrow });
    export let pg = 'EcE';
</script>
<svelte:head>
    <title>{pg}</title>
</svelte:head>


<AppShell>
   
            <svelte:fragment slot="header">
                <header class="custom-header">
                    <div class="logo-container">
                        <a href="/">
                            <img src='src/lib/images/logo1.png' alt="EcE" />
                        </a>
                    </div>
                    <nav class="navigation-links">
                        <a class="text-link" href="/about">About Us</a>
                        <a class="text-link" href="/help">Find Help</a>
                        <a class="text-link" href="/give">Donate</a>
                        <a class="text-link" href="/contact">Contact Us</a>
                    </nav>
                </header>
       
		<slot />
    </svelte:fragment>
</AppShell>

<style>
    .custom-header {
        display: flex;
        justify-content: space-between; /* This will place the nav and logo at opposite ends */
        padding: 1rem 2rem;
        background-color: transparent; /* This ensures that the header is clear */
    }

    .logo-container {
        margin-right: auto; /* This will push the logo container to the right */
    }

    .navigation-links {
        display: flex;
        gap: 1rem; /* Space out the navigation links */
    }
    .text-link {
        color: #fff; /* Or any color that matches your design */
        text-decoration: none;
        font-weight: bold;
        transition: color 0.3s ease;
    }

    .text-link:hover {
        color: #aaa; /* Or any hover effect color you prefer */
    }
    </style>
