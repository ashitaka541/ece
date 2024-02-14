<script>
     
    let sections = {
    'Our Mission': "To harness the transformative power of technology and education to promote social justice and human dignity. We are dedicated to empowering individuals from all walks of life, especially those in marginalized communities, by providing access to resources, skills, and opportunities needed to live autonomous, fulfilling lives.",
    'Our Vision': "In a world where the right to life and dignity stands as the cornerstone of our shared humanity, we envision a future where every individual's freedom to live an autonomous life, free of coercion and abuse, is not just a dream but a reality. In this future, the intrinsic value of human life is celebrated, standing tall against the shadows cast by the relentless pursuit of wealth by a privileged few. Our vision is a world where technological advancements, particularly in automation and AI, are not mere tools for profit, but powerful forces harnessed for the greater good.",
    'Our Values': "Founded on empathy, evidence, and empowerment, our organization prioritizes a trauma-informed approach and evidence-based solutions. We empower clients through collaborative SMART goal setting for specific, measurable, and achievable outcomes. Our inclusive, low-barrier approach ensures wide-reaching service accessibility. We emphasize community collaboration and agile responsiveness, constantly adapting to evolving needs, driving progress toward a more equitable future. ",
    'Our Programs': 'Our suite of programs empowers individuals through Core Curriculum Development in job, social, technical, and life skills, delivered via a flexible hybrid model for accessibility. Our Resource Connection Hub, Digital Access Center, and Health and Hygiene Facilities offer essential support, while partnerships enhance personal care services. We integrate AI and Data Analysis for service refinement and employ SCRUM Lean Project Management for efficiency. Continuous Feedback and Improvement, coupled with Community Engagement and Empowerment, form our holistic approach for long-term stability and independence.',
  };
 
  export let pg = 'EcE ~ About';
</script>
<svelte:head>
    <title>{pg}</title>
</svelte:head>

<div class="grid-container">
<div class="block card card-hover bg-gradient-to-br variant-gradient-secondary-primary">
    <header class="card-header">Our Vision</header>
    <section class="p-4">{sections['Our Vision']}</section>
</div>
<div class="block card card-hover bg-gradient-to-br variant-gradient-primary-secondary">
  <header class="card-header">Our Mission</header>
  <section class="p-4">{sections['Our Mission']}</section>
</div>
<div class="block card card-hover bg-gradient-to-br variant-gradient-secondary-primary">
  <header class="card-header">Our Values</header>
  <section class="p-4">{sections['Our Values']}</section>
</div>
<div class="block card card-hover bg-gradient-to-br variant-gradient-primary-secondary">
  <header class="card-header">Our Programs</header>
  <section class="p-4">{sections['Our Programs']}</section>
</div>
</div>
<style>
    .grid-container {
      display: grid;
      grid-template-columns: repeat(2, 1fr); /* Creates a 2-column layout */
      gap: 2rem; /* This is the padding between the items */
      padding: 2rem; /* This is the padding around the entire grid */
    }
    .card-header {
  font-size: 2rem; /* Adjust the size as needed */
  font-weight: bold; /* Optional: if you want the headers to be bold */
  margin-bottom: 1rem; /* Optional: if you want space between the header and the content */
  /* Include other styling like color, text-transform as needed */
}
</style>
