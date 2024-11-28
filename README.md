# discord-experiment

To access the experimental feature, first log in to your Discord account. Then, open the inspect element tool by pressing Ctrl + Shift + I on Google Chrome (or Command + Option + I on Mac).
## Browser Tutorial
Open inspect element on any browser, click on the `'Console'` tab under the inspect element window, then copy the code below, and paste it in the console. However, prior to pasting, make sure you have the `'Allow Paste'` enabled because, in case you have been not allowed to paste the code in.
## Mac

## Code

`webpackChunkdiscord_app.push([["wp_isdev_patch"], {}, r => cache=Object.values(r.c)]);
var UserStore = cache.find(m => m?.exports?.default?.getCurrentUser).exports.default;
var actions = Object.values(UserStore._dispatcher._actionHandlers._dependencyGraph.nodes);
var user = UserStore.getCurrentUser();
actions.find(n => n.name === "ExperimentStore").actionHandler.CONNECTION_OPEN({
	type: "CONNECTION_OPEN", user: {flags: user.flags |= 1}, experiments: [],
});
actions.find(n => n.name === "DeveloperExperimentStore").actionHandler.CONNECTION_OPEN();
webpackChunkdiscord_app.pop(); user.flags &= ~1; "done";`
