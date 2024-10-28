## Deploy Next.js on Plesk

#### 1. Install and build nextjs on Plesk.
#### 2. Ppdate file `node_modules/.bin/next`.

before:
```js
program.command('dev', {
    isDefault: true
})

program.command('start')
```

after:
```js
program.command('dev')

program.command('start', {
    isDefault: true
})
```

#### 3. On Plesk, add `Application startup file` to `node_modules/.bin/next`.