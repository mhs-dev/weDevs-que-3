# weDevs-que-3

```
function wearPPE() {
    return new Promise((resolve) => {
        setTimeout(() => resolve('Wearing PPE'), 2000);
    })
}

function fightCorona() {
    return new Promise((resolve) => {
        setTimeout(() => resolve('Fighting Corona'), 1000);
    })
}

function execute() {
    wearPPE().then(result => console.log(result));
    setTimeout(() => fightCorona().then(result => console.log(result)), 1500);
}

execute();
```
