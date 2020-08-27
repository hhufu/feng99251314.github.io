---

title: vue使用watch监听拿到props的传值

date:

tags: Vue

---

第一种情况：
<!--more-->
```javascript
<script>
    export default {
        data() {
            return {
                floorData0: {},
                floorData1: {},
                floorData2: {},
            }
        },
        props:['floorData'],
        watch:{
            floorData:val => {
                console.log(this.floorData);
                this.floorData0 = this.floordata[0];
                this.floorData1 = this.floordata[1];
                this.floorData2 = this.floordata[2];
            }
        }
    }
</script>
```
在floorData传值成功的前提下，有时候会出现直接在 watch 里面通过 this.floorData 是无法拿到的，总是显示 undefined。然后需要通过 newVal和oldVal这么处理，才能拿到 floorData 的值：

第二种
```javascript
        props: {
			farmlandList: {
				type: Array,
				default: []
			},
			rentFarmlandList: {
				type: Array,
				default: []
			}
		},
		data() {
			return {
				isOpen2: 0,
				// 图片数组
				imageList: [],
				// 田块List
				farmlands: this.farmlandList,
				// 租出田块list
				rentFarmlands: this.rentFarmlandList,
				// 显示图片
				show: false
				
			}
		},
		watch: {
			farmlandList(val) {
				this.farmlands = val
			},
            
            rentFarmlandList(val) {
            	this.rentFarmlands = val
            }
		},
```
