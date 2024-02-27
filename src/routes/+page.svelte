<script>
  import ReactiveDeclarations from "../components/ReactiveDeclarations.svelte";
import ReactiveAssignment from "../components/Reactive_Assignment.svelte";
  import ReactiveStatments from "../components/Reactive_Statments.svelte";

</script>
<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
<a href="/helloworld">Hello World</a> <br />
<a href='/dynamic_attribute'>Dynamic Attributes</a><br/>
<a href='styling'> Styling</a><br/>
<a href='nested_components'>Nested Component</a><br/>
<a href='html_tags'>HTML TAGS</a> <br/>

<div>
    <p><strong>Reactive Assignment</strong></p>
    <ReactiveAssignment/> <br/>

    <p><strong>Reactive Declarations</strong></p>
    <ReactiveDeclarations/>

    <p><strong>Reactive Statments</strong></p>
    <ReactiveStatments/>
</div>
