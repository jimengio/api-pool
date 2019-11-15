## API Pool (WIP)

> Small library to reuse same requests in the same time from React Hooks

### Usage

TODO

```ts
// reuse same promise in 60s
apiPool.config({
  timeout: 60,
});

// create resource with a key(in array)
apiPool.getRequest(["materials", materialId], (options) => {
  return getMaterial(materialId);
});

// mark resource as outdated and deprecate promise
apiPool.outdateResource(["materials", materialId]);
```

### Workflow

https://github.com/jimengio/ts-workflow

### License

MIT
