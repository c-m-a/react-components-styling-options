# React Components Styling Options

1. inline-style.
In side of the HTML, has the "highest specificity" which means if you write any CSS code that modify the current style element is not going to work. 

- Pros
* If you want to modify something quick you just to write on the HTML.
* You know that nothing can't affect the style of that element.

- Cons
* No portable.
* No maintainable.
* No accesible for everybody your style is inside of the code a designer can't access to modify CSS properties.
* No taking advantage of the cascade nature of CSS.
* You can't use pseudo selectors or pseudo elements.

eg.

```html
<div
	style={{
		with: '90%',
		maxWidth: '40rem',
		margin: '2rem auto',
		border: '1px solid #ccc',
		padding: '1rem'
	}}
>
```

2. Styled Component.

You have to install to this package by using:

```bash
npm i styled-components
```

Import library

import styled from 'styled-components';

You have to start with a capital letter to use it as a component.

const StyledDiv = styled.div`
	with: 90%;
	max-width: 40rem;
	margin: 2rem auto;
	border: 1px solid #ccc;
	padding: 1rem;
`;


function App() {
	return (
		<StyledDiv>
			Hi there!
		</StyledDiv>
	);
}


3. Normal CSS.

4. CSS Modules.

