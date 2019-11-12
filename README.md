## goal

easy to setup apis with config file;

easy to switch between mock and the real apis;


```js
const myAxios = nscAxios({
  'post:/api/projects': 'post:/api/projects/new',
  'put:/api/projects/:id': 'put:/api/projects/:id/update',
  'method:/api/endpoint': (axiosOptions) => {
    return {
      url: '',
      data: '',
      params: '',

    }
  }
})

myAxios.mock(true)
```



