# DOM XSS — Search Box (Juice Shop)

**Challenge:** Trigger a DOM-based XSS by inserting a malicious `iframe` payload in the search box.

**Short description:** The application reflects untrusted input into the DOM without proper sanitization, allowing execution of JavaScript supplied via an `iframe` `src` attribute. 
The payload used here is:

```html
<iframe src="javascript:alert(`xss`)">
