# Rundown

## Things that would would nice

- Display Markdown with "run" button for code blocks.
- Decorator logic
	- promp
	- store var
		- use var in template
	- skip
	- jump
	- if

Parser

Run on markdown as “best guess” (run anything in code snippets? Possibly look for sections with headings like install or something

Option to ”decorate” specifically for rundown.

Nice to haves:
- Prompt decorator?
    - <!— prompt “We suggest installing this extra library as well, would you like to?” —>
- User Input/variable storage?
    - <!— prompt “are you on mac?” store-as=‘isMac’—>
    - Maybe more than y/n? Like string inputs? Could be handy for things like… install to specific dirs, or scripts that require a key or something… 
- Conditional logic
    - <!— if “isMac” —>
- Variable replacement in scripts?

```sh

```

```js

```

```rb

```

---------

---
name: My Project
---

# Example Project

My project does cool things.

## Setup

Run the following:

<!--rd-- prompt "Directory to clean?" store="dir" -->

```
cd {{dir}}
rm -rf *
```

<!--- prompt "are you on mac?" goto="#mac" --->

### Mac

<!--- if "!on mac?" skip --->

### Linux

<!--- sh
rm -rf *
--->

## Contributing

### How To

### Something


---

- https://oclif.io/docs/introduction
- http://yargs.js.org
- https://github.com/A1rPun/marked-cli/blob/master/terminal.js
- https://marked.js.org/using_pro#use
- https://github.com/vadimdemedes/ink
- https://github.com/cameronhunter/ink-markdown
- https://github.com/lukasbach/ink-form
- https://github.com/sindresorhus/ink-gradient
