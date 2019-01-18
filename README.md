## quill-video-resize-module

### install

```
yarn add quill-video-resize-module
```

basic usage
```js
<script>
import { quillEditor, Quill } from 'vue-quill-editor'
import VideoResize from 'quill-video-resize-module'
Quill.register('modules/VideoResize', VideoResize)

export default {
	options: {
		modules: {
			VideoResize: {
				modules: [ 'Resize', 'DisplaySize', 'Toolbar' ],
				tagName: 'iframe', // iframe | video
        	}
		}
	}
}
</script>
<style>
.quill-editor iframe,
.quill-editor video {
    pointer-events: none;
}
</style>
```
