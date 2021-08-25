# HSongSlideTabView
## 让TabView变的更酷!
### 1.展示效果
<br />
<div>
<img src="/DIsplayImage/noImgDisplay.gif" width = "250" height = "541" alt="" align=center />
<img src="/DIsplayImage/haveImgDisplay.gif" width = "250" height = "541" alt="" align=center />
<div />

### 2.使用
  
#### ①首先引入HSongSlideTabView
    import HSongSlideTabView
#### ②定义TabView样式
##### 无图标（如1中左图）
    struct ContentView: View {
        let manager: Manager = Manager(leftTitle: "你好", rightTitle: "欢迎")
        var body: some View {
            HSongSlideTabView(manager: manager) {
                AView()
                BView()
            }
        }
    }
 ##### 有图标（如1中右图）
    struct ContentView: View {
        let manager: Manager = Manager(leftImg: "dianpu", leftSelectedImg: "dianpu-sed",leftTitle: "你好", rightImg: "yinliao", rightSelectedImg: "yinliao-sed",rightTitle: "欢迎")
        var body: some View {
            HSongSlideTabView(manager: manager) {
                AView()
                BView()
            }
        }
    }
