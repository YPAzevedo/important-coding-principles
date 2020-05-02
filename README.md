# Important coding principles 👾

## 1.DRY

`DRY` is an abbreviation for `Don't Repeat Yourself` .

`WRONG`: It doesn't mean to not repeat code.

`CORRECT`: Don't repeat business logic. Meaning to not repeat code that has an specific objective.

A good way to look at it is, if you are coding the same behavior more the 3 times then perhaps you should move that to abstract that code.

## 2.KISS

`KISS` is an abbreviation for `Keep It Simple and Stupid` .

It means to keep you code easy to ready and understand for someone that never seen it before, keeping you parameter, const, variables with readable names.

`WRONG`:

```tsx
function showUsersInformation(data) {
	return data.map(u => {
		name: u.name,
		age: u.age
	}
}
```

`CORRECT`:

```tsx
function getUsersNameAndAge(users) {
	return users.map(user => {
		name: user.name,
		age: user.age
	}
}
```

## 3.YAGNI

`YAGNI` is an abbreviation for `You Ain't Gonna Need It` .

It means to not implement tools and features just for the sake of implementing it, over complicating your application before you actually need to implement those tools or features.
