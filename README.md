问题：在Vue实例的method方法中，this是指向的是当前Vue实例，但是使用ajax的回调函数中，this的指向会失败，然后使用=>箭头函数：

```vue
axios.get('/user', {
    params: {
      ID: 12345
    }
  })
  .then((response) => {
    console.log(response);
  })
  .catch((error) => {
    console.log(error);
  });
```

创建的水配料使用的模式是工厂和单例模式，从主界面进入制作方便面会进入indexServlet初始化对象