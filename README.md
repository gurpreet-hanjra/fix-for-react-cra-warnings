# fix-for-react-cra-warnings
Fixes and causes for common warning React application

```javascript
const ids = [];
this.state.accounts.map(account => {
  ids.push({ id: Number(account.accountId) });
});
```
```javascript
const ids = this.state.accounts.map(account => {
  return { id: Number(account.accountId) };
});

```
