# jQuery Valida 2.0.7

Valida is a jQuery plugin which provides an easy, fast and lightweight way to make form validations on client-side.

It's source-code (minified) has about *8Kb*.

##Details

Validating a form on client-side, using Javascript, can be (at least for me is) a very boring and slower task! 

So, looking for a way to make it easyer and faster, I wrote this small, light, but very flexible plugin to do 
the hard and boring job, provindg a very smart way to validate web forms!

Since your are using *Valida*, you can expect:

> - Each TEXTAREA, on your form, which has a maxlength property set, will receive a description label
(right below it) that displays the maxlength and how many chars were already typed!

> - Each INPUT text field, on your form, which has a filter property set, will be analysed when the user 
is typing to inform him/her that the value is valid or invalid!

> - During the validation process, each field on your form which has the "required" property set and has 
no value or has the "filter" property set and the value doesn't match the given filter, will receive a 
label  (right below it) with a error/invalid message.

> - You also can run some stuff before/after the validation via callback methods and customize the messages 
and the layout of messages displayed!

> - There are 18 filters available to be used.

##How to use it ?

  Import the "valida.js" on the HEAD of your page:

  {{{
  <script type="text/javascript" src="valida.js" ></script>
  }}}

  Set what kind of fields are required and has filters:

  {{{
  <input type="text" ... required="true" /> <!-- required or -->
  <input type="text" ... filter="email" /> <!-- filter */ or -->
  <input type="text" ... required="true" filter="email" /> <!-- both -->
  }}}

  Then, you just need call it:

  {{{
  <script type="text/javascript" src="valida.js" >
      jQuery(document).ready(function(){
         $('your-form').valida();
      });
  </script>
  }}}

  Done!

*What will happen ?*

So, when you submit your form (as you usually may do), the Valida will get in action and make the analisys of your form, putting messages (error/warnings) when it is necessary and stopping the form submit for  mistakes corrections. Beyond some another nice stuff.

See how it works in detail: [http://code.google.com/p/jquery-valida/wiki/Documentation read more].

----

Well, that's it! Easy, don't you think?

If you have any suggestion, critics or just wanna say hello, feel free to mail me or leave a comments here.

Happy coding! =)
