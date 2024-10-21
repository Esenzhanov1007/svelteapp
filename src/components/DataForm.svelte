<script>
    import Input from '../components/Input.svelte';
    import Checkbox from '../components/Checkbox.svelte';
    import Button from '../components/Button.svelte';
    import Title from './Title.svelte';
    import FormTitle from './FormTitle.svelte';

    let name = "";
    let company = "";
    let email = "";
    let phone = "";
    let subject = "";
    let message = "";
    let termsAccepted = false;
  </script>
  
  <Title />
  
  <form class="form">
    <FormTitle />
    <Input placeholder="Name*" bind:value={name} required={true} />
    <Input placeholder="Company*" bind:value={company} required={true} />
    <Input placeholder="E-mail*" bind:value={email} required={true} />
    <Input placeholder="Phone" bind:value={phone} />
    <Input placeholder="Subject*" bind:value={subject} required={true} />
    <Input placeholder="Message*" bind:value={message} required={true} />
    
    <Checkbox label="I accept Terms and Privacy Policy" bind:checked={termsAccepted} />
  
    <Button label="Send" />
  </form>
  
  <style>
    .form {
      text-align: center;
      width: 100%;
      max-width: 390px;
      height: 100%;
      max-height: 810px;
      margin: 0 auto 50px;
      background-color: #171929;
      padding: 2rem;
      border-radius: 27px;
    }
  </style>
  