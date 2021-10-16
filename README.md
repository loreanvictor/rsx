# rsx
idea: how would first-hand support for reactive programming in JS look like?

## Proposed Rules

<table>
<tr>
  <th>RSX Code</th>
  <th>JS Equivalent</th>
</tr>
<tr>
<td>

```jsx
const x@ = 2
```
  
</td>
<td>

```jsx
const x = new BehaviorSubject(2)
```
  
</td>
</tr>
<tr>
<td>

```jsx
const a = @b + @c * 2
```

</td>

<td>

```jsx
const a = computed(() => $(b) + $(c) * 2)

```

</td>
  
</tr>
</table>
