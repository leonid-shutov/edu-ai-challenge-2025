## Experienced Developer Perspective

**Observations:**

- The logic is straightforward and readable.
- The use of `var` is outdated and can introduce scoping issues.
- The ternary operator used for setting `active` is unnecessary.

**Recommendations:**

- Replace `var` with `let` or `const` for better scoping and modern best practices.
- Simplify the boolean assignment: `data[i].status === 'active'` returns a boolean already.
- Use `Array.prototype.map()` for a cleaner and more expressive transformation of the array.

**Suggested Refactor:**

```javascript
function processUserData(data: any[]) {
  const users = data.map((item) => ({
    id: item.id,
    name: item.name,
    email: item.email,
    active: item.status === "active",
  }));
  console.log(`Processed ${users.length} users`);
  return users;
}
```
