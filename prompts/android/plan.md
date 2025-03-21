# Android 项目学习计划

## 项目技术栈

- **编程语言**：Kotlin - 现代 JVM 语言，支持函数式编程和协程
- **UI 框架**：Jetpack Compose - Android 声明式 UI 框架
- **构建工具**：Gradle - 灵活的项目自动化构建工具

## 学习步骤

### **1. 界面层（UI Layer）**

#### (1) 入口定位

• **`AndroidManifest.xml`**  
  定位所有 Activity（项目入口）、权限声明、主题配置。  
  示例：`<activity android:name=".MainActivity">` 标记主界面。
• **`res/layout/` 目录**  
  查看 XML 布局文件，快速预览界面结构，关注 `RecyclerView`、`ViewPager` 等复杂组件。

#### (2) 核心界面组件

• **Activity/Fragment 类**  
  类名通常与功能相关（如 `LoginActivity.kt`），重点关注 `onCreate()` 生命周期和 `setContentView()` 绑定的布局。
• **自定义 View**  
  在 `com.example.app.view` 或 `widget` 包中查找继承 `View`、`ViewGroup` 的类，如 `CustomButton.kt`。
• **Jetpack Compose**（如使用）  
  查找 `@Composable` 函数，导航逻辑可能集中在 `NavHostController`。

#### (3) 工具辅助

• 使用 Android Studio 的 **Layout Inspector** 实时关联界面元素与代码。

#### 提出问题：

TODO

---

### **2. 业务层（Business Layer）**

#### (1) 状态管理

• **ViewModel 类**  
  位于 `viewmodel` 或 `presentation` 包，如 `UserViewModel.kt`，观察 `LiveData` 或 `StateFlow` 暴露的数据。
• **状态保存逻辑**  
  检查 `onSaveInstanceState()` 或 `SavedStateHandle` 的使用。

#### (2) 页面导航

• **导航图文件**  
  `res/navigation/nav_graph.xml` 定义页面跳转关系，配合 `NavController` 实现路由。
• **深层链接（DeepLink）**  
  在 `AndroidManifest.xml` 或导航图中搜索 `<deepLink>` 标签。

#### (3) 依赖注入

• **Hilt/Dagger 模块**  
  查找 `@Module` 注解类（如 `AppModule.kt`），分析依赖注入关系。

---

#### 提出问题：

TODO

### **3. 数据层（Data Layer）**

#### (1) 网络请求

• **Retrofit 接口**  
  在 `api` 或 `network` 包中查找带 `@GET`/`@POST` 注解的接口（如 `ApiService.kt`）。
• **网络拦截器**  
  检查 `OkHttpClient` 配置中的 `Interceptor`（如日志、认证逻辑）。

#### (2) 本地存储

• **Room 组件**  
  `@Entity` 定义数据表，`@Dao` 接口在 `database` 包中，`RoomDatabase` 子类管理数据库实例。
• **SharedPreferences**  
  搜索 `getSharedPreferences()` 调用或封装类（如 `SettingsManager.kt`）。

#### (3) 数据流整合

• **Repository 模式**  
  在 `repository` 包中查看数据聚合类，通常结合 `Flow` 或 `RxJava` 实现多数据源协调。

---

### **4. 补充切入点**

• **Gradle 文件**  
  `build.gradle` 查看依赖库（如 `Retrofit 2.9.0`）、模块化配置。
• **资源管理**  
  `res/values/` 下的 `strings.xml`、`colors.xml` 管理静态资源。
• **第三方服务**  
  定位 Firebase、地图 SDK 等初始化代码（如 `MainApplication.kt`）。

#### 提出问题：

TODO