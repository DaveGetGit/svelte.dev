<script>
  import TextAreaInput from "./../components/Bindings/TextAreaInput.svelte";
  import ReactiveDeclarations from "../components/Reactivity/ReactiveDeclarations.svelte";
  import ReactiveAssignment from "../components/Reactivity/Reactive_Assignment.svelte";
  import ReactiveStatments from "../components/Reactivity/Reactive_Statments.svelte";
  import DeclaringProps from "../components/Props/DeclaringProps.svelte";
  import DefaultValues from "../components/Props/Default_Values.svelte";
  import SpreadProps from "../components/Props/SpreadProps.svelte";
  import IfBLocks from "../components/Logic/If_BLocks.svelte";
  import ElseBlocks from "../components/Logic/Else_Blocks.svelte";
  import ElseIfBlocks from "../components/Logic/Else-If_Blocks.svelte";
  import EachBlock from "../components/Logic/Each-Block.svelte";
  import KeyedEachBlock from "../components/Logic/Keyed-Each-Block.svelte";
  import AwaitBlocks from "../components/Logic/Await-Blocks.svelte";
  import DomEvents from "../components/Events/DOM-Events.svelte";
  import InlineHandlers from "../components/Events/Inline-Handlers.svelte";
  import EventModifiers from "../components/Events/Event-Modifiers.svelte";
  import ComponentEvents from "../components/Events/Component-Events.svelte";
  import EventForwarding from "../components/Events/Event-Forwarding.svelte";
  import DomEventForwarding from "../components/Events/DOM-Event-Forwarding.svelte";
  import TextInputs from "../components/Bindings/TextInputs.svelte";
  import NumericInputs from "../components/Bindings/NumericInputs.svelte";
  import CheckboxInputs from "../components/Bindings/CheckboxInputs.svelte";
  import GroupInputs from "../components/Bindings/GroupInputs.svelte";
  import FileInputs from "../components/Bindings/FileInputs.svelte";
  import SelectBindings from "../components/Bindings/SelectBindings.svelte";
  import SelectMultiple from "../components/Bindings/SelectMultiple.svelte";
  import EachBlockBindings from "../components/Bindings/EachBlockBindings.svelte";
  import MediaElements from "../components/Bindings/MediaElements.svelte";
  import Dimensions from "../components/Bindings/Dimensions.svelte";
  import BindThisCanvas from "../components/Bindings/Bind_this_canvas.svelte";
  import ComponentBindings from "../components/Bindings/ComponentBindings.svelte";
</script>

<h1>Welcome to SvelteKit</h1>
<p>
  Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation
</p>
<a href="/helloworld">Hello World</a> <br />
<a href="/dynamic_attribute">Dynamic Attributes</a><br />
<a href="styling"> Styling</a><br />
<a href="nested_components">Nested Component</a><br />
<a href="html_tags">HTML TAGS</a> <br />

<div>
  <p><strong>Reactive Assignment</strong></p>
  <ReactiveAssignment /> <br />

  <p><strong>Reactive Declarations</strong></p>
  <ReactiveDeclarations />

  <p><strong>Reactive Statments</strong></p>
  <ReactiveStatments />
</div>

<div>
  <p><strong>Props Declaration</strong></p>
  <DeclaringProps />

  <p><strong>Default Values</strong></p>
  <DefaultValues />

  <p><strong>Spread Props</strong></p>
  <SpreadProps />
</div>

<div>
  <p><strong>IF Blocks</strong></p>
  <IfBLocks />

  <p><strong>Else Blocks</strong></p>
  <ElseBlocks />

  <p><strong>Else If Blocks</strong></p>
  <ElseIfBlocks />

  <p><strong>Each Block</strong></p>
  <EachBlock />

  <p><strong>Keyed Each Block</strong></p>
  <KeyedEachBlock />

  <p><strong>Await Block</strong></p>
  <AwaitBlocks />
</div>

<div>
  <p><strong>DOM Events</strong></p>
  <DomEvents />

  <p><strong>Inline Handlers</strong></p>
  <InlineHandlers />

  <p><strong>Event Modofiers</strong></p>
  <EventModifiers />

  <p><strong>Component Events</strong></p>
  <ComponentEvents />

  <p><strong>Event Forwarding</strong></p>
  <EventForwarding />

  <p><strong>DOM Event Forwarding</strong></p>
  <DomEventForwarding />
</div>

<div>
  <p><strong>Text Inputs</strong></p>
  <TextInputs />

  <p><strong>Numeric Inputs</strong></p>
  <NumericInputs />

  <p><strong>CheckBox</strong></p>
  <CheckboxInputs />

  <p><strong>Group Inputs</strong></p>
  <GroupInputs />

  <p><strong>TextArea Inputs</strong></p>
  <TextAreaInput />

  <p><strong>File Inputs</strong></p>
  <FileInputs />

  <p><strong>Select Bindings</strong></p>
  <SelectBindings />

  <p><strong>Select Multiple</strong></p>
  <SelectMultiple />

  <p><strong>Each Block Bindings</strong></p>
  <EachBlockBindings />

  <p><strong>Media Elements</strong></p>
  <MediaElements />

  <p><strong>Dimensions</strong></p>
  <Dimensions />

  <p><strong>Bind:this Canvas</strong></p>
  <BindThisCanvas />

  <p><strong>Component Bindings</strong></p>
  <ComponentBindings />
</div>
