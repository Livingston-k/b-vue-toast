# b-vue-toast For Vue2

This was bulit with bootstrap 4

### How to install with npm

```
npm install --save Livingston-k/b-vue-toast#main
```

### How to install with yarn

```
yarn add Livingston-k/b-vue-toast#main
```


### How to use it?

1- Import..

```
import VueBootstrapToasts from "vue-bootstrap-toasts";
Vue.use(VueBootstrapToasts);
```

2 - Add the component in your html, somewhere at the top..

```
<Toasts></Toasts>
```

Or if u want to override default values

```
<Toasts
	:show-progress="true"
	:rtl="true"
	:max-messages="7"
	:time-out="5000" // 5 secs
	:closeable="true"
></Toasts>
```

3 - Call these methods where ever you want inside vue..

```
this.$toast.success('your message');
this.$toast.error('your message');
this.$toast.warning('your message');
this.$toast.info('your message');
```

Or Pass an options per toast

```
this.$toast.success("your message", {
	showProgress: true,
	rtl: true,
	timeOut: 0, // infinity
	closeable: false
});
```
