# linf

List instagram non followers

Login into your IG account on your PC, go to your profile and press F12 to open a console.

Now click on `followers`, paste this in the console and hit enter:

```js
setInterval(() => { 
	const aano = document.querySelector('.xyi19xy');
	if (aano) {
		aano.scrollTo(0, 1000000000000000000);
	}
}, 100);
```

Wait until it finishes loading and then paste this in the console and hit enter:

```js
const followers = [];
document.querySelectorAll('span._ap3a').forEach(n => {

	followers.push(n.innerText);

});
```

Click on `following`, wait for it to finish loading, then paste this and hit enter:

```js
document.querySelectorAll('span._ap3a').forEach(n => {

	const username = n.innerText;
	if (followers.indexOf(username) === -1) {
		console.log(username, ' IS NOT FOLLOWING YOU!');
	}

});
```

Ready! All those who unfollowed you will be listed in the console!
