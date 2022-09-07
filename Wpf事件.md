# 使用事件
* Nuget添加[Microsoft.Xaml.Behaviors.Wpf](https://github.com/Microsoft/XamlBehaviorsWpf)包
* xaml文件中添加***xmlns:i="http://schemas.microsoft.com/xaml/behaviors"***命名控件
* 使用事件
* 示例代码

```xaml
    <i:Interaction.Triggers>
        <i:EventTrigger EventName="Loaded">
            <i:InvokeCommandAction Command="{Binding LoadCompletedCommand}" />
        </i:EventTrigger>
    </i:Interaction.Triggers>
```

# 常用事件
|  事件                                                   |  描述                                                                                                                                |
|-------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|
|  Annotation.AnchorChanged                             |  新增、移除或修改 Anchor 元素时发生。                                                                                                            |
|  Annotation.AuthorChanged                             |  新增、移除或修改 Author 元素时发生。                                                                                                            |
|  Annotation.CargoChanged                              |  新增、移除或修改 Cargo 元素时发生。                                                                                                             |
|  AnnotationStore.AnchorChanged                        |  存放区中任何注释上的 Anchor 元素变化时发生。                                                                                                        |
|  AnnotationStore.AuthorChanged                        |  存放区中任何注释上的 Author 元素变化时发生。                                                                                                        |
|  AnnotationStore.CargoChanged                         |  存放区中任何附注上的 Cargo 元素变化时发生。                                                                                                         |
|  AnnotationStore.StoreContentChanged                  |  在存放区中新增或删除注释时发生。                                                                                                                  |
|  Application.Activated                                |  应用程序变成前景应用程序时发生。                                                                                                                  |
|  Application.Deactivated                              |  应用程序停止作为前景应用程序时发生。                                                                                                                |
|  Application.DispatcherUnhandledException             |  引发无法处理的例外时发生。                                                                                                                     |
|  Application.Exit                                     |  应用程序即将关闭之前发生。                                                                                                                     |
|  Application.FragmentNavigation                       |  应用程序内的一或多个 NavigationService 物件引发 FragmentNavigation 时发生。                                                                         |
|  Application.LoadCompleted                            |  应用程序内的一或多个 NavigationService 物件引发 LoadCompleted 时发生。                                                                              |
|  Application.Navigated                                |  应用程序内的一或多个 NavigationService 物件引发 Navigated 时发生。                                                                                  |
|  Application.Navigating                               |  应用程序内的一或多个 NavigationService 物件引发 Navigating 时发生。                                                                                 |
|  Application.NavigationProgress                       |  应用程序内的一或多个 NavigationService 物件引发 NavigationProgress 时发生。                                                                         |
|  Application.NavigationStopped                        |  应用程序内的一或多个 NavigationService 物件引发 NavigationStopped 时发生。                                                                          |
|  Application.SessionEnding                            |  使用者登出或关闭作业系统结束 Windows 工作阶段时发生。                                                                                                   |
|  Application.Startup                                  |  呼叫 Application 物件的 Run 方法时发生。                                                                                                     |
|  BitmapDecoder.DownloadCompleted                      |  BitmapDecoder 完成点阵图内容下载时发生。                                                                                                       |
|  BitmapDecoder.DownloadProgress                       |  BitmapDecoder 进行点阵图内容下载时发生。                                                                                                       |
|  BitmapSource.DownloadCompleted                       |  点阵图内容完成下载时发生。                                                                                                                     |
|  BitmapSource.DownloadProgress                        |  点阵图内容的下载进度变化时发生。                                                                                                                  |
|  ButtonBase.Click                                     |  按一下按钮时发生。                                                                                                                         |
|  Clock.CurrentGlobalSpeedInvalidated                  |  更新时钟速度时发生。                                                                                                                        |
|  Clock.CurrentStateInvalidated                        |  更新时钟的 CurrentState 属性时发生。                                                                                                         |
|  Clock.CurrentTimeInvalidated                         |  时钟的 CurrentTime 变成无效时发生。                                                                                                          |
|  CollectionView.CurrentChanged                        |  CurrentItem 变化 后发生。                                                                                                               |
|  CollectionView.CurrentChanging                       |  变化货币时发生。                                                                                                                          |
|  CollectionViewSource.Filter                          |  会提供筛选逻辑。                                                                                                                          |
|  ComboBox.DropDownClosed                              |  无法再看到下拉式方块的下拉部分时发生。                                                                                                               |
|  ComboBox.DropDownOpened                              |  开启下拉式方块的快显清单时发生。                                                                                                                  |
|  CommandBinding.CanExecute                            |  此 CommandBinding 的相关命令开始进行检查，以判断是否可以在命令目标上执行命令时发生。                                                                                |
|  CommandBinding.Executed                              |  执行与此 CommandBinding 相关的命令时发生。                                                                                                     |
|  CommandBinding.PreviewCanExecute                     |  此 CommandBinding 的相关命令开始进行检查，以判断是否可以在目前的命令目标上执行命令时发生。                                                                             |
|  CommandBinding.PreviewExecuted                       |  执行与此 CommandBinding 相关的命令时发生。                                                                                                     |
|  ContentElement.DragEnter                             |  当输入系统报告出将这个元素当做拖曳目标的基础拖曳事件时发生。                                                                                                    |
|  ContentElement.DragLeave                             |  当输入系统报告出将这个元素当做拖曳来源的基础拖曳事件时发生。                                                                                                    |
|  ContentElement.DragOver                              |  当输入系统报告出将这个元素当做可能放下目标的基础拖曳事件时发生。                                                                                                  |
|  ContentElement.Drop                                  |  当输入系统报告出将这个元素当做放下目标的基础放下事件时发生。                                                                                                    |
|  ContentElement.GiveFeedback                          |  与此事件相关的基础拖放事件输入系统报告产生时发生。                                                                                                         |
|  ContentElement.GotFocus                              |  当这个元素取得逻辑焦点时发生。                                                                                                                   |
|  ContentElement.GotKeyboardFocus                      |  当键盘将焦点放在此元素时发生。                                                                                                                   |
|  ContentElement.GotMouseCapture                       |  当这个元素撷取鼠标时发生。                                                                                                                     |
|  ContentElement.GotStylusCapture                      |  当这个元素撷取手写笔时发生。                                                                                                                    |
|  ContentElement.IsEnabledChanged                      |  当这个元素的 IsEnabled 属性值变化时发生。                                                                                                        |
|  ContentElement.IsKeyboardFocusedChanged              |  当这个元素的 IsKeyboardFocused 属性值变化时发生。                                                                                                |
|  ContentElement.IsKeyboardFocusWithinChanged          |  当这个元素的 IsKeyboardFocusWithinChanged 属性值变化时发生。                                                                                     |
|  ContentElement.IsMouseCapturedChanged                |  当这个元素的 IsMouseCaptured 属性值变化时发生。                                                                                                  |
|  ContentElement.IsMouseCaptureWithinChanged           |  这个元素的 IsMouseCaptureWithinProperty 栏位值变化时发生。                                                                                      |
|  ContentElement.IsMouseDirectlyOverChanged            |  当这个元素的 IsMouseDirectlyOver 属性值变化时发生。                                                                                              |
|  ContentElement.IsStylusCapturedChanged               |  当这个元素的 IsStylusCaptured 属性值变化时发生。                                                                                                 |
|  ContentElement.IsStylusCaptureWithinChanged          |  这个元素的 IsStylusCaptureWithin 属性值变化时发生。                                                                                             |
|  ContentElement.IsStylusDirectlyOverChanged           |  当这个元素的 IsStylusDirectlyOver 属性值变化时发生。                                                                                             |
|  ContentElement.KeyDown                               |  当键盘将焦点放在这个元素上的同时按下按键时发生。                                                                                                          |
|  ContentElement.KeyUp                                 |  当键盘将焦点放在这个元素上的同时放开按键时发生。                                                                                                          |
|  ContentElement.LostFocus                             |  当这个元素失去逻辑焦点时发生。                                                                                                                   |
|  ContentElement.LostKeyboardFocus                     |  当键盘不再将焦点放在此元素时发生。                                                                                                                 |
|  ContentElement.LostMouseCapture                      |  当这个元素失去鼠标撷取时发生。                                                                                                                   |
|  ContentElement.LostStylusCapture                     |  当这个元素失去手写笔撷取时发生。                                                                                                                  |
|  ContentElement.MouseDown                             |  鼠标指标在这个元素上的同时按下鼠标按钮时发生。如果 ContentElement 是 Button 控制项，表示 Windows Presentation Foundation 未登录这个事件。请改用 PreviewMouseDown 或 Click 事件。 |
|  ContentElement.MouseEnter                            |  当鼠标指标进入这个元素的界限时发生。                                                                                                                |
|  ContentElement.MouseLeave                            |  当鼠标指标离开这个元素的界限时发生。                                                                                                                |
|  ContentElement.MouseLeftButtonDown                   |  当鼠标指标在这个元素上的同时按下鼠标左键时发生。                                                                                                          |
|  ContentElement.MouseLeftButtonUp                     |  当鼠标指标在这个元素上的同时放开鼠标左键时发生。                                                                                                          |
|  ContentElement.MouseMove                             |  鼠标指标在这个元素上的同时移动鼠标指标时发生。                                                                                                           |
|  ContentElement.MouseRightButtonDown                  |  当鼠标指标在这个元素上的同时按下鼠标右键时发生。                                                                                                          |
|  ContentElement.MouseRightButtonUp                    |  当鼠标指标在这个元素上的同时放开鼠标右键时发生。                                                                                                          |
|  ContentElement.MouseUp                               |  在这个元素上放开任何鼠标按钮时发生。                                                                                                                |
|  ContentElement.MouseWheel                            |  使用者在鼠标指标于这个元素上的同时滚动鼠标滚轮时发生。                                                                                                       |
|  ContentElement.PreviewDragEnter                      |  当输入系统报告出将这个元素当做拖曳目标的基础拖曳事件时发生。                                                                                                    |
|  ContentElement.PreviewDragLeave                      |  当输入系统报告出将这个元素当做拖曳来源的基础拖曳事件时发生。                                                                                                    |
|  ContentElement.PreviewDragOver                       |  当输入系统报告出将这个元素当做可能放下目标的基础拖曳事件时发生。                                                                                                  |
|  ContentElement.PreviewDrop                           |  当输入系统报告出将这个元素当做放下目标的基础放下事件时发生。                                                                                                    |
|  ContentElement.PreviewGiveFeedback                   |  在启动拖放作业时发生。                                                                                                                       |
|  ContentElement.PreviewGotKeyboardFocus               |  当键盘将焦点放在此元素时发生。                                                                                                                   |
|  ContentElement.PreviewKeyDown                        |  当键盘将焦点放在这个元素上的同时按下按键时发生。                                                                                                          |
|  ContentElement.PreviewKeyUp                          |  当键盘将焦点放在这个元素上的同时放开按键时发生。                                                                                                          |
|  ContentElement.PreviewLostKeyboardFocus              |  当键盘不再将焦点放在此元素时发生。                                                                                                                 |
|  ContentElement.PreviewMouseDown                      |  鼠标指标在这个元素上的同时按下鼠标按钮时发生。                                                                                                           |
|  ContentElement.PreviewMouseLeftButtonDown            |  当鼠标指标在这个元素上的同时按下鼠标左键时发生。                                                                                                          |
|  ContentElement.PreviewMouseLeftButtonUp              |  当鼠标指标在这个元素上的同时放开鼠标左键时发生。                                                                                                          |
|  ContentElement.PreviewMouseMove                      |  当鼠标指标在这个元素上的同时移动鼠标指标时发生。                                                                                                          |
|  ContentElement.PreviewMouseRightButtonDown           |  当鼠标指标在这个元素上的同时按下鼠标右键时发生。                                                                                                          |
|  ContentElement.PreviewMouseRightButtonUp             |  当鼠标指标在这个元素上的同时放开鼠标右键时发生。                                                                                                          |
|  ContentElement.PreviewMouseUp                        |  当鼠标指标在这个元素上的同时放开鼠标按钮时发生。                                                                                                          |
|  ContentElement.PreviewMouseWheel                     |  使用者在鼠标指标于这个元素上的同时滚动鼠标滚轮时发生。                                                                                                       |
|  ContentElement.PreviewQueryContinueDrag              |  在拖放作业期间，当键盘或鼠标按钮状态变化时发生。                                                                                                          |
|  ContentElement.PreviewStylusButtonDown               |  当指标在这个元素上的同时按下手写笔按钮时发生。                                                                                                           |
|  ContentElement.PreviewStylusButtonUp                 |  当指标在这个元素上的同时放开手写笔按钮时发生。                                                                                                           |
|  ContentElement.PreviewStylusDown                     |  当手写笔在这个元素上的同时手写笔接触到数码板时发生。                                                                                                        |
|  ContentElement.PreviewStylusInAirMove                |  当手写笔移到元素上但实际上没有接触数码板时发生。                                                                                                          |
|  ContentElement.PreviewStylusInRange                  |  当手写笔相当靠近数码板而能检测到，且手写笔同时在这个元素上时发生。                                                                                                 |
|  ContentElement.PreviewStylusMove                     |  当手写笔在元素上的同时移动手写笔时发生。若要引发这个事件，必须在数码板检测到手写笔时移动手写笔，否则会改为引发 PreviewStylusInAirMove。                                                   |
|  ContentElement.PreviewStylusOutOfRange               |  当手写笔离数码板太远而无法检测到时发生。                                                                                                              |
|  ContentElement.PreviewStylusSystemGesture            |  使用者执行其中一个手写笔笔势时发生。                                                                                                                |
|  ContentElement.PreviewStylusUp                       |  当手写笔在这个元素上的同时，使用者将手写笔移开数码板时发生。                                                                                                    |
|  ContentElement.PreviewTextInput                      |  这个元素使用与装置无关的方法取得文字时发生。                                                                                                            |
|  ContentElement.QueryContinueDrag                     |  在拖放作业期间，当键盘或鼠标按钮状态变化时发生。                                                                                                          |
|  ContentElement.QueryCursor                           |  在要求显示游标时发生。每次鼠标指标移到新位置时就会在元素上引发这个事件，表示可能需要根据鼠标指标的新位置变化游标物件。                                                                       |
|  ContentElement.StylusButtonDown                      |  当指标在这个元素上的同时按下手写笔按钮时发生。                                                                                                           |
|  ContentElement.StylusButtonUp                        |  当指标在这个元素上的同时放开手写笔按钮时发生。                                                                                                           |
|  ContentElement.StylusDown                            |  当手写笔在这个元素上的同时手写笔接触到数码板时发生。                                                                                                        |
|  ContentElement.StylusEnter                           |  当手写笔进入这个元素的界限时发生。                                                                                                                 |
|  ContentElement.StylusInAirMove                       |  当手写笔移到元素上但实际上没有接触数码板时发生。                                                                                                          |
|  ContentElement.StylusInRange                         |  手写笔相当靠近数码板而能检测到，且手写笔同时在这个元素上时发生。                                                                                                  |
|  ContentElement.StylusLeave                           |  当手写笔离开元素的界限时发生。                                                                                                                   |
|  ContentElement.StylusMove                            |  当手写笔移到这个元素上时发生。若要引发这个事件，必须在手写笔在数码板上的同时移动手写笔，否则会改为引发 StylusInAirMove。                                                              |
|  ContentElement.StylusOutOfRange                      |  手写笔离数码板太远而无法检测到，且手写笔同时在这个元素上时发生。                                                                                                  |
|  ContentElement.StylusSystemGesture                   |  当使用者执行其中一个手写笔笔势时发生。                                                                                                               |
|  ContentElement.StylusUp                              |  当手写笔在这个元素上的同时，使用者将手写笔移开数码板时发生。                                                                                                    |
|  ContentElement.TextInput                             |  这个元素使用与装置无关的方法取得文字时发生。                                                                                                            |
|  ContextMenu.Closed                                   |  关闭快显功能表的特定例项时发生。                                                                                                                  |
|  ContextMenu.Opened                                   |  开启快显功能表的特定例项时发生。                                                                                                                  |
|  Control.MouseDoubleClick                             |  以鼠标按两下控制项时发生。                                                                                                                     |
|  Control.PreviewMouseDoubleClick                      |  使用者按两下或更多下鼠标按钮时发生。                                                                                                                |
|  DataSourceProvider.DataChanged                       |  Data 属性有新值时发生。                                                                                                                    |
|  DataTrigger.Invalidated                              |  &nbsp;                                                                                                                            |
|  Dispatcher.ShutdownFinished                          |  发送器关闭完成时发生。                                                                                                                       |
|  Dispatcher.ShutdownStarted                           |  发送器开始关闭时发生。                                                                                                                       |
|  Dispatcher.UnhandledException                        |  掷回执行绪例外，并在使用 Invoke 或 BeginInvoke 执行委派期间未拦截该例外时发生。                                                                                |
|  Dispatcher.UnhandledExceptionFilter                  |  掷回执行绪例外，并在使用 Invoke 或 BeginInvoke 于筛选阶段执行委派期间未拦截该例外时发生。                                                                           |
|  DispatcherHooks.DispatcherInactive                   |  发送器没有要处理的作业时发生。                                                                                                                   |
|  DispatcherHooks.OperationAborted                     |  中止作业时发生。                                                                                                                          |
|  DispatcherHooks.OperationCompleted                   |  完成作业时发生。                                                                                                                          |
|  DispatcherHooks.OperationPosted                      |  作业张贴到发送器时发生。                                                                                                                      |
|  DispatcherHooks.OperationPriorityChanged             |  作业的优先顺序变化时发生。                                                                                                                     |
|  DispatcherOperation.Aborted                          |  中止与此 DispatcherOperation 相关之发送器伫列上的委派时发生。                                                                                         |
|  DispatcherOperation.Completed                        |  完成与此 DispatcherOperation 相关之发送器伫列上的委派时发生。                                                                                         |
|  DispatcherTimer.Tick                                 |  已超过计时器间隔而且停用计时器时发生。                                                                                                               |
|  DocumentPage.PageDestroyed                           |  引述 DocumentPage 的视觉元素已损坏且无法用于显示时发生。                                                                                               |
|  DocumentPageView.PageConnected                       |  已连接 DocumentPage 的视觉元素时发生。                                                                                                        |
|  DocumentPageView.PageDisconnected                    |  已中断连接 DocumentPage 的视觉元素时发生。                                                                                                      |
|  DocumentPaginator.ComputePageCountCompleted          |  ComputePageCountAsync 作业完成时发生。                                                                                                    |
|  DocumentPaginator.GetPageCompleted                   |  GetPageAsync 完成时发生。                                                                                                               |
|  DocumentPaginator.PagesChanged                       |  变化文件内容时发生。                                                                                                                        |
|  DocumentReferenceCollection.CollectionChanged        |  新增或移除元素时发生。                                                                                                                       |
|  DocumentViewerBase.PageViewsChanged                  |  与这个检视器相关之 DocumentPageView 项目的集合 (由 PageViews 属性表示) 变化时发生。                                                                        |
|  DrawingAttributes.AttributeChanged                   |  DrawingAttributes 物件中的属性变化时发生。                                                                                                    |
|  DrawingAttributes.PropertyDataChanged                |  在 StrokeCollection 中新增或移除属性资料时发生。                                                                                                 |
|  DynamicDocumentPaginator.GetPageNumberCompleted      |  GetPageNumberAsync 完成时发生。                                                                                                         |
|  DynamicDocumentPaginator.PaginationCompleted         |  所有文件的内容都已标上页码时发生。                                                                                                                 |
|  DynamicDocumentPaginator.PaginationProgress          |  一或多个内容页面已标上页码时发生。                                                                                                                 |
|  Expander.Collapsed                                   |  关闭 Expander 控制项的内容视窗，而且只能看见标题时发生。                                                                                                 |
|  Expander.Expanded                                    |  开启 Expander 控制项的内容视窗以显示此标题和内容时发生。                                                                                                 |
|  FileDialog.FileOk                                    |  使用者按一下 OpenFileDialog 的 [开启] 按钮或 SaveFileDialog 的 [储存] 按钮，以选取档桉名称时发生。                                                             |
|  Frame.ContentRendered                                |  在显示框架内容之后发生。                                                                                                                      |
|  Frame.FragmentNavigation                             |  开始导览到 XAML 内容片段 (这在载入来源 XAML 页面之后发生) 时发生。                                                                                         |
|  Frame.LoadCompleted                                  |  已载入或剖析整个来源内容时发生。                                                                                                                  |
|  Frame.Navigated                                      |  找到来源内容并开始下载时发生。                                                                                                                   |
|  Frame.Navigating                                     |  导览即将开始之前发生。                                                                                                                       |  &nbsp; |
|  Frame.NavigationProgress                             |  下载期间会定期发生，以提供导览进度资讯。                                                                                                              |
|  Frame.NavigationStopped                              |  在导览期间呼叫 StopLoading 方法时发生。                                                                                                        |
|  FrameworkContentElement.ContextMenuClosing           |  即将关闭 FrameworkContentElement 上的快显功能表之前发生。                                                                                         |
|  FrameworkContentElement.ContextMenuOpening           |  已开启 FrameworkContentElement 上的快显功能表时发生。                                                                                           |
|  FrameworkContentElement.DataContextChanged           |  变化 FrameworkContentElement 的资料内容时发生。                                                                                              |
|  FrameworkContentElement.Initialized                  |  初始化 FrameworkContentElement 时发生。这与 IsInitialized 属性的值从 False (或未定义) 变化为 True 的情况一致。                                               |
|  FrameworkContentElement.Loaded                       |  已配置、显示 FrameworkContentElement 并准备进行互动时发生。                                                                                        |
|  FrameworkContentElement.SourceUpdated                |  参与 FrameworkContentElement 上之繫结的相关资料来源变化时发生。                                                                                      |
|  FrameworkContentElement.TargetUpdated                |  参与 FrameworkContentElement 上之繫结的相关目标属性变化时发生。                                                                                      |
|  FrameworkContentElement.ToolTipClosing               |  即将关闭 FrameworkContentElement 上的工具提示之前发生。                                                                                          |
|  FrameworkContentElement.ToolTipOpening               |  已开启元素上的工具提示时发生。                                                                                                                   |
|  FrameworkContentElement.Unloaded                     |  从所载入元素的元素树状目录中移除 FrameworkContentElement 时发生。                                                                                     |
|  FrameworkElement.ContextMenuClosing                  |  即将关闭 FrameworkElement 上的快显功能表之前发生。                                                                                                |
|  FrameworkElement.ContextMenuOpening                  |  已开启 FrameworkElement 上的快显功能表时发生。                                                                                                  |
|  FrameworkElement.DataContextChanged                  |  变化 FrameworkElement 的资料内容时发生。                                                                                                     |
|  FrameworkElement.Initialized                         |  初始化 FrameworkElement 时发生。这与 IsInitialized 属性的值从 False (或未定义) 变化为 True 的情况一致。                                                      |
|  FrameworkElement.Loaded                              |  已配置、显示 FrameworkElement 并准备进行互动时发生。                                                                                               |
|  FrameworkElement.RequestBringIntoView                |  在这个元素上呼叫 BringIntoView 时发生。                                                                                                       |
|  FrameworkElement.SizeChanged                         |  ActualHeight 或 ActualWidth 属性变化 FrameworkElement 上的值时发生。                                                                          |
|  FrameworkElement.SourceUpdated                       |  参与 FrameworkElement 上之繫结的相关资料来源变化时发生。                                                                                             |
|  FrameworkElement.TargetUpdated                       |  参与 FrameworkElement 上之繫结的相关目标属性变化时发生。                                                                                             |
|  FrameworkElement.ToolTipClosing                      |  即将关闭 FrameworkElement 上的工具提示之前发生。                                                                                                 |
|  FrameworkElement.ToolTipOpening                      |  已开启 FrameworkElement 上的工具提示时发生。                                                                                                   |
|  FrameworkElement.Unloaded                            |  从所载入元素的元素树状目录中移除 FrameworkElement 时发生。                                                                                            |
|  Freezable.Changed                                    |  修改这个 Freezable 物件或内含物件时发生。                                                                                                        |
|  GridViewColumnCollection.ColumnCollectionChanged     |  &nbsp;                                                                                                                            |
|  HwndHost.MessageHook                                 |  对主控视窗所接收之每则无法处理的讯息发生。                                                                                                             |
|  HwndSource.AutoResized                               |  版面配置使得 HwndSource 自动调整大小时发生。                                                                                                      |
|  HwndSource.Disposed                                  |  处置 HwndSource 物件时发生。                                                                                                              |
|  HwndSource.SizeToContentChanged                      |  HwndSource 物件的 SizeToContent 属性值变化时发生。                                                                                            |
|  Hyperlink.Click                                      |  按一下鼠标左键时发生。                                                                                                                       |
|  Hyperlink.RequestNavigate                            |  要求导览事件时发生。                                                                                                                        |
|  ICollectionView.CurrentChanged                       |  实作 ICollectionView 介面时，在变化目前的项目之后引发这个事件。                                                                                          |
|  ICollectionView.CurrentChanging                      |  实作 ICollectionView 介面时，在变化目前的项目之前引发这个事件。事件处理常式可以取消此事件。                                                                            |
|  ICommand.CanExecuteChanged                           |  执行命令的能力变化时发生。                                                                                                                     |
|  IInputElement.GotKeyboardFocus                       |  当键盘将焦点放在此元素时发生。                                                                                                                   |
|  IInputElement.GotMouseCapture                        |  元素撷取鼠标时发生。                                                                                                                        |
|  IInputElement.GotStylusCapture                       |  元素撷取手写笔时发生。                                                                                                                       |
|  IInputElement.KeyDown                                |  键盘将焦点放在这个元素上的同时按下按键时发生。                                                                                                           |
|  IInputElement.KeyUp                                  |  键盘将焦点放在这个元素上的同时放开按键时发生。                                                                                                           |
|  IInputElement.LostKeyboardFocus                      |  键盘不再将焦点放在此元素时发生。                                                                                                                  |
|  IInputElement.LostMouseCapture                       |  元素失去鼠标撷取时发生。                                                                                                                      |
|  IInputElement.LostStylusCapture                      |  元素失去手写笔撷取时发生。                                                                                                                     |
|  IInputElement.MouseEnter                             |  鼠标指标进入元素的界限时发生。                                                                                                                   |
|  IInputElement.MouseLeave                             |  鼠标指标离开元素的界限时发生。                                                                                                                   |
|  IInputElement.MouseLeftButtonDown                    |  鼠标指标在元素上的同时按下鼠标左键时发生。                                                                                                             |
|  IInputElement.MouseLeftButtonUp                      |  鼠标指标在元素上的同时放开鼠标左键时发生。                                                                                                             |
|  IInputElement.MouseMove                              |  鼠标指标在元素上的同时移动鼠标指标时发生。                                                                                                             |
|  IInputElement.MouseRightButtonDown                   |  鼠标指标在元素上的同时按下鼠标右键时发生。                                                                                                             |
|  IInputElement.MouseRightButtonUp                     |  鼠标指标在元素上的同时放开鼠标右键时发生。                                                                                                             |
|  IInputElement.MouseWheel                             |  鼠标指标在元素上的同时移动鼠标滚轮时发生。                                                                                                             |
|  IInputElement.PreviewGotKeyboardFocus                |  键盘将焦点放在此元素时发生。                                                                                                                    |
|  IInputElement.PreviewKeyDown                         |  键盘将焦点放在这个元素上的同时按下按键时发生。                                                                                                           |
|  IInputElement.PreviewKeyUp                           |  键盘将焦点放在这个元素上的同时放开按键时发生。                                                                                                           |
|  IInputElement.PreviewLostKeyboardFocus               |  键盘不再将焦点放在此元素时发生。                                                                                                                  |
|  IInputElement.PreviewMouseLeftButtonDown             |  鼠标指标在元素上的同时按下鼠标左键时发生。                                                                                                             |
|  IInputElement.PreviewMouseLeftButtonUp               |  鼠标指标在元素上的同时放开鼠标左键时发生。                                                                                                             |
|  IInputElement.PreviewMouseMove                       |  鼠标指标在元素上的同时移动鼠标指标时发生。                                                                                                             |
|  IInputElement.PreviewMouseRightButtonDown            |  鼠标指标在元素上的同时按下鼠标右键时发生。                                                                                                             |
|  IInputElement.PreviewMouseRightButtonUp              |  鼠标指标在元素上的同时放开鼠标右键时发生。                                                                                                             |
|  IInputElement.PreviewMouseWheel                      |  鼠标指标在元素上的同时移动鼠标滚轮时发生。                                                                                                             |
|  IInputElement.PreviewStylusButtonDown                |  手写笔在元素上的同时按下手写笔按钮时发生。                                                                                                             |
|  IInputElement.PreviewStylusButtonUp                  |  手写笔在元素上的同时放开手写笔按钮时发生。                                                                                                             |
|  IInputElement.PreviewStylusDown                      |  手写笔在元素上的同时接触数码板时发生。                                                                                                               |
|  IInputElement.PreviewStylusInAirMove                 |  手写笔移到元素上但没有接触数码板时发生。                                                                                                              |
|  IInputElement.PreviewStylusInRange                   |  手写笔很靠近数码板而可以检测到时发生。                                                                                                               |
|  IInputElement.PreviewStylusMove                      |  手写笔在元素上的同时移动手写笔时发生。                                                                                                               |
|  IInputElement.PreviewStylusOutOfRange                |  当手写笔离数码板太远而无法检测到时发生。                                                                                                              |
|  IInputElement.PreviewStylusSystemGesture             |  检测到其中一个手写笔笔势 (例如「轻敲」或「拖曳」) 时发生。                                                                                                   |
|  IInputElement.PreviewStylusUp                        |  手写笔在元素上的同时移开数码板时发生。                                                                                                               |
|  IInputElement.PreviewTextInput                       |  元素使用与装置无关的方法取得文字时发生。                                                                                                              |
|  IInputElement.StylusButtonDown                       |  手写笔在元素上的同时按下手写笔按钮时发生。                                                                                                             |
|  IInputElement.StylusButtonUp                         |  手写笔在元素上的同时放开手写笔按钮时发生。                                                                                                             |
|  IInputElement.StylusDown                             |  手写笔在元素上的同时接触数码板时发生。                                                                                                               |
|  IInputElement.StylusEnter                            |  手写笔游标进入元素的界限时发生。                                                                                                                  |
|  IInputElement.StylusInAirMove                        |  手写笔移到元素上但没有接触数码板时发生。                                                                                                              |
|  IInputElement.StylusInRange                          |  手写笔很靠近数码板而可以检测到时发生。                                                                                                               |
|  IInputElement.StylusLeave                            |  手写笔游标离开元素的界限时发生。                                                                                                                  |
|  IInputElement.StylusMove                             |  手写笔游标移到元素上时发生。                                                                                                                    |
|  IInputElement.StylusOutOfRange                       |  当手写笔离数码板太远而无法检测到时发生。                                                                                                              |
|  IInputElement.StylusSystemGesture                    |  检测到其中一个手写笔笔势 (例如「轻敲」或「拖曳」) 时发生。                                                                                                   |
|  IInputElement.StylusUp                               |  手写笔在元素上的同时移开数码板时发生。                                                                                                               |
|  IInputElement.TextInput                              |  元素使用与装置无关的方法取得文字时发生。                                                                                                              |
|  IncrementalLassoHitTester.SelectionChanged           |  套索路径选取或取消选取笔墨笔触时发生。                                                                                                               |
|  IncrementalStrokeHitTester.StrokeHit                 |  IncrementalStrokeHitTester 与笔墨笔触交集时发生。                                                                                            |
|  InkCanvas.ActiveEditingModeChanged                   |  目前的编辑模式变化时发生。                                                                                                                     |
|  InkCanvas.DefaultDrawingAttributesReplaced           |  取代 DefaultDrawingAttributes 属性时发生。                                                                                                |
|  InkCanvas.EditingModeChanged                         |  当 InkCanvas 物件的 EditingMode 属性已变化时发生。                                                                                             |
|  InkCanvas.EditingModeInvertedChanged                 |  InkCanvas 物件的 EditingModeInverted 属性已变化时发生。                                                                                       |
|  InkCanvas.Gesture                                    |  InkCanvas 检测到笔势时发生。                                                                                                               |
|  InkCanvas.SelectionChanged                           |  InkCanvas 上的选取变化时发生。                                                                                                              |
|  InkCanvas.SelectionChanging                          |  选取新的笔墨笔触或元素集合时发生。                                                                                                                 |
|  InkCanvas.SelectionMoved                             |  使用者移动笔触或元素的选取时发生。                                                                                                                 |
|  InkCanvas.SelectionMoving                            |  开始移动选取的笔触和元素时发生。                                                                                                                  |
|  InkCanvas.SelectionResized                           |  使用者调整笔触或元素的选取大小时发生。                                                                                                               |
|  InkCanvas.SelectionResizing                          |  开始调整选取的笔触和元素大小时发生。                                                                                                                |
|  InkCanvas.StrokeCollected                            |  使用者绘製的笔触加入 Strokes 属性时发生。                                                                                                         |
|  InkCanvas.StrokeErased                               |  使用者清除笔触时发生。                                                                                                                       |
|  InkCanvas.StrokeErasing                              |  使用者即将清除笔触之前发生。                                                                                                                    |
|  InkCanvas.StrokesReplaced                            |  取代 Strokes 属性时发生。                                                                                                                 |
|  INotifyCollectionChanged.CollectionChanged           |  透过新增或移除项目而变化集合时发生。                                                                                                                |
|  InputLanguageManager.InputLanguageChanged            |  完成输入语言的变化时发生。                                                                                                                     |
|  InputLanguageManager.InputLanguageChanging           |  初始化输入语言的变化时发生。                                                                                                                    |
|  InputManager.HitTestInvalidatedAsync                 |  点击测试的结果可能已变化时发生。                                                                                                                  |
|  InputManager.PostNotifyInput                         |  PreNotifyInput 处理常式处理好原始输入，且已引发对应的 Windows Presentation Foundation 事件之后发生。                                                        |
|  InputManager.PostProcessInput                        |  PreNotifyInput 处理常式处理好原始输入之后发生。                                                                                                   |
|  InputManager.PreNotifyInput                          |  如果没有取消原始输入，在 PreProcessInput 处理常式处理好原始输入后发生。                                                                                      |
|  InputManager.PreProcessInput                         |  InputManager 开始处理原始输入项目时发生。                                                                                                       |
|  InputMethod.StateChanged                             |  输入方法状态 (由 ImeState 属性表示) 变化时发生。                                                                                                   |
|  ItemContainerGenerator.ItemsChanged                  |  由 ItemContainerGenerator 引发，通知版面配置已变化项目集合。                                                                                        |
|  ItemContainerGenerator.StatusChanged                 |  由 ItemContainerGenerator 引发，通知控制项状态已变化。                                                                                           |
|  ListBoxItem.Selected                                 |  选取 ListBoxItem 时发生。                                                                                                               |
|  ListBoxItem.Unselected                               |  取消 ListBoxItem 选取时发生。                                                                                                             |
|  MediaElement.BufferingEnded                          |  结束媒体缓冲处理时发生。                                                                                                                      |
|  MediaElement.BufferingStarted                        |  已开始媒体缓冲处理时发生。                                                                                                                     |
|  MediaElement.MediaEnded                              |  已结束媒体时发生。                                                                                                                         |
|  MediaElement.MediaFailed                             |  遇到媒体错误时发生。                                                                                                                        |
|  MediaElement.MediaOpened                             |  完成媒体载入时发生。                                                                                                                        |
|  MediaPlayer.BufferingEnded                           |  完成媒体缓冲处理时发生。                                                                                                                      |
|  MediaPlayer.BufferingStarted                         |  已开启媒体缓冲处理时发生。                                                                                                                     |
|  MediaPlayer.MediaEnded                               |  媒体已完成播放时发生。                                                                                                                       |
|  MediaPlayer.MediaFailed                              |  遇到媒体错误时发生。                                                                                                                        |
|  MediaPlayer.MediaOpened                              |  开启媒体时发生。                                                                                                                          |
|  MenuItem.Checked                                     |  核取功能表项目时发生。                                                                                                                       |
|  MenuItem.Click                                       |  使用针对功能表项目定义的快速键或便捷键点选或选取功能表项目时发生。                                                                                                 |
|  MenuItem.SubmenuClosed                               |  IsSubmenuOpen 属性的状态变化为 false 时发生。                                                                                                 |
|  MenuItem.SubmenuOpened                               |  IsSubmenuOpen 属性的状态变化为 True 时发生。                                                                                                  |
|  MenuItem.Unchecked                                   |  清除功能表项目的核取方块时发生。                                                                                                                  |
|  MultiDataTrigger.Invalidated                         |  &nbsp;                                                                                                                            |
|  MultiTrigger.Invalidated                             |  &nbsp;                                                                                                                            |
|  NavigationService.FragmentNavigation                 |  开始导览到 XAML 内容片段 (这在载入来源 XAML 页面之后发生) 时发生。                                                                                         |
|  NavigationService.LoadCompleted                      |  已载入或剖析整个来源内容时发生。                                                                                                                  |
|  NavigationService.Navigated                          |  找到来源内容并开始下载时发生。                                                                                                                   |
|  NavigationService.Navigating                         |  导览即将开始之前发生。                                                                                                                       |
|  NavigationService.NavigationProgress                 |  下载期间会定期发生，以提供导览进度资讯。                                                                                                              |
|  NavigationService.NavigationStopped                  |  呼叫 NavigationService 物件的 StopLoading 方法时发生。                                                                                       |
|  NavigationWindow.FragmentNavigation                  |  开始导览到 XAML 内容片段 (这在载入来源 XAML 页面之后发生) 时发生。                                                                                         |
|  NavigationWindow.LoadCompleted                       |  已载入或剖析整个来源内容时发生。                                                                                                                  |
|  NavigationWindow.Navigated                           |  找到来源内容并开始下载时发生。                                                                                                                   |
|  NavigationWindow.Navigating                          |  导览即将开始之前发生。                                                                                                                       |
|  NavigationWindow.NavigationProgress                  |  下载期间会定期发生，以提供导览进度资讯。                                                                                                              |
|  NavigationWindow.NavigationStopped                   |  在导览期间呼叫 StopLoading 方法时发生。                                                                                                        |
|  ObservableCollection`1.CollectionChanged             |  &nbsp;                                                                                                                            |
|  PackageDigitalSignatureManager.InvalidSignatureEvent |  VerifySignatures 发现无效的签章时发生。                                                                                                      |
|  PageContent.GetPageRootCompleted                     |  GetPageRootAsync 已完成时发生。                                                                                                          |
|  PageFunction`1.Return                                |  &nbsp;                                                                                                                            |
|  PasswordBox.PasswordChanged                          |  Password 属性的值变化时发生。                                                                                                               |
|  Popup.Closed                                         |  IsOpen 属性变化为 False 时发生。                                                                                                           |
|  Popup.Opened                                         |  IsOpen 属性变化为 True 时发生。                                                                                                            |
|  PresentationSource.ContentRendered                   |  已显示内容并准备用于使用者互动时发生。                                                                                                               |
|  PrintDialogBase.PrinterChanged                       |  &nbsp;                                                                                                                            |
|  PrintDialogBase.PrintTicketChanged                   |  &nbsp;                                                                                                                            |
|  PrintDialogBase.PrintTicketChanging                  |  &nbsp;                                                                                                                            |
|  PrintDialogBase.PropertyChanged                      |  &nbsp;                                                                                                                            |
|  RangeBase.ValueChanged                               |  范围值变化时发生。                                                                                                                         |
|  RoutedCommand.CanExecuteChanged                      |  在目前的命令目标上执行命令的能力变化时发生。                                                                                                            |
|  ScrollBar.Scroll                                     |  使用者使用鼠标移动 Thumb 控制项，且透过捲轴捲动内容时会发生一次或数次。                                                                                           |
|  ScrollViewer.ScrollChanged                           |  检测到捲动位置、范围或检视区大小的变化时发生。                                                                                                           |
|  Selector.SelectionChanged                            |  选取器的选取范围变化时发生。                                                                                                                    |
|  SerializerWriter.WritingCompleted                    |  在衍生类别中覆写时，会在完成写入作业时发生。                                                                                                            |
|  SerializerWriter.WritingPrintTicketRequired          |  在衍生类别中覆写时，会在使用 Write 或 WriteAsync 方法即将把 PrintTicket 加入资料流之前发生。                                                                    |
|  SerializerWriter.WritingProgressChanged              |  在衍生类别中覆写时，会在 SerializerWriter 更新进度时发生。                                                                                            |
|  Stroke.DrawingAttributesChanged                      |  与 Stroke 物件相关的 DrawingAttributes 变化时发生。                                                                                           |
|  Stroke.DrawingAttributesReplaced                     |  取代 Stroke 物件的绘图属性时发生。                                                                                                             |
|  Stroke.Invalidated                                   |  Stroke 的外观变化时发生。                                                                                                                  |
|  Stroke.PropertyDataChanged                           |  Stroke 物件上的自订属性变化时发生。                                                                                                             |
|  Stroke.StylusPointsChanged                           |  StylusPoints 属性变化时发生。                                                                                                             |
|  Stroke.StylusPointsReplaced                          |  StylusPoints 属性指派了新的 StylusPointCollection 时发生。                                                                                   |
|  StrokeCollection.PropertyDataChanged                 |  在 StrokeCollection 中新增或移除自订属性时发生。                                                                                                 |
|  StrokeCollection.StrokesChanged                      |  集合中的 Stroke 变化时发生。                                                                                                                |
|  StylusPointCollection.Changed                        |  StylusPointCollection 变化时发生。                                                                                                      |
|  TextBoxBase.SelectionChanged                         |  已变化文字选取时发生。                                                                                                                       |
|  TextBoxBase.TextChanged                              |  文字元素中的内容变化时发生。                                                                                                                    |
|  TextRange.Changed                                    |  调整范围位置以涵盖新的内容范围时发生。                                                                                                               |
|  Thumb.DragCompleted                                  |  Thumb 控制项失去鼠标撷取时发生。                                                                                                               |
|  Thumb.DragDelta                                      |  Thumb 控制项具有逻辑焦点和鼠标撷取，且鼠标变化位置时会发生一次或数次。                                                                                            |
|  Thumb.DragStarted                                    |  Thumb 控制项接收逻辑焦点和鼠标撷取时发生。                                                                                                          |
|  Timeline.CurrentGlobalSpeedInvalidated               |  时间轴之时钟的时间进度速率变化时发生。                                                                                                               |
|  Timeline.CurrentStateInvalidated                     |  时间轴之时钟的 CurrentState 属性更新时发生。                                                                                                     |
|  Timeline.CurrentTimeInvalidated                      |  时间轴之时钟的 CurrentTime 属性更新时发生。                                                                                                      |
|  ToggleButton.Checked                                 |  核取切换按钮时发生。                                                                                                                        |
|  ToggleButton.Indeterminate                           |  切换按钮的状态不是开启也不是关闭时发生。                                                                                                              |
|  ToggleButton.Unchecked                               |  取消核取切换按钮时发生。                                                                                                                      |
|  ToolTip.Closed                                       |  关闭工具提示而且不再显示时发生。                                                                                                                  |
|  ToolTip.Opened                                       |  工具提示消失时发生。                                                                                                                        |
|  TreeView.SelectedItemChanged                         |  选取的项目变化时发生。                                                                                                                       |
|  TreeViewItem.Collapsed                               |  IsExpanded 属性从 True 变为 False 时发生。                                                                                                 |
|  TreeViewItem.Expanded                                |  IsExpanded 属性从 False 变为 True 时发生。                                                                                                 |
|  TreeViewItem.Selected                                |  TreeViewItem 的 IsSelected 属性从 False 变为 True 时发生。                                                                                  |
|  TreeViewItem.Unselected                              |  TreeViewItem 的 IsSelected 属性从 True 变为 False 时发生。                                                                                  |
|  Trigger.Invalidated                                  |
|  UIElement.DragEnter                                  |  当输入系统报告出将这个元素当做拖曳目标的基础拖曳事件时发生。                                                                                                    |
|  UIElement.DragLeave                                  |  当输入系统报告出将这个元素当做拖曳来源的基础拖曳事件时发生。                                                                                                    |
|  UIElement.DragOver                                   |  当输入系统报告出将这个元素当做可能放下目标的基础拖曳事件时发生。                                                                                                  |
|  UIElement.Drop                                       |  当输入系统报告出将这个元素当做放下目标的基础放下事件时发生。                                                                                                    |
|  UIElement.GiveFeedback                               |  与此事件相关的基础拖放事件输入系统报告产生时发生。                                                                                                         |
|  UIElement.GotFocus                                   |  当这个元素取得逻辑焦点时发生。                                                                                                                   |
|  UIElement.GotKeyboardFocus                           |  当键盘将焦点放在此元素时发生。                                                                                                                   |
|  UIElement.GotMouseCapture                            |  当这个元素撷取鼠标时发生。                                                                                                                     |
|  UIElement.GotStylusCapture                           |  当这个元素撷取手写笔时发生。                                                                                                                    |
|  UIElement.IsEnabledChanged                           |  当这个元素的 IsEnabled 属性值变化时发生。                                                                                                        |
|  UIElement.IsHitTestVisibleChanged                    |  这个元素的 IsHitTestVisible 相依属性值变化时发生。                                                                                                |
|  UIElement.IsKeyboardFocusedChanged                   |  当这个元素的 IsKeyboardFocused 属性值变化时发生。                                                                                                |
|  UIElement.IsKeyboardFocusWithinChanged               |  当这个元素的 IsKeyboardFocusWithinChanged 属性值变化时发生。                                                                                     |
|  UIElement.IsMouseCapturedChanged                     |  当这个元素的 IsMouseCaptured 属性值变化时发生。                                                                                                  |
|  UIElement.IsMouseDirectlyOverChanged                 |  当这个元素的 IsMouseDirectlyOver 属性值变化时发生。                                                                                              |
|  UIElement.IsStylusCapturedChanged                    |  当这个元素的 IsStylusCaptured 属性值变化时发生。                                                                                                 |
|  UIElement.IsStylusDirectlyOverChanged                |  当这个元素的 IsStylusDirectlyOver 属性值变化时发生。                                                                                             |
|  UIElement.IsVisibleChanged                           |  这个元素的 IsVisible 属性值变化时发生。                                                                                                         |
|  UIElement.KeyDown                                    |  当键盘将焦点放在这个元素上的同时按下按键时发生。                                                                                                          |
|  UIElement.KeyUp                                      |  当键盘将焦点放在这个元素上的同时放开按键时发生。                                                                                                          |
|  UIElement.LayoutUpdated                              |  与现行发送器相关之各种视觉元素的版面配置变化时发生。                                                                                                        |
|  UIElement.LostFocus                                  |  当这个元素失去逻辑焦点时发生。                                                                                                                   |
|  UIElement.LostKeyboardFocus                          |  当键盘不再将焦点放在此元素时发生。                                                                                                                 |
|  UIElement.LostMouseCapture                           |  当这个元素失去鼠标撷取时发生。                                                                                                                   |
|  UIElement.LostStylusCapture                          |  当这个元素失去手写笔撷取时发生。                                                                                                                  |
|  UIElement.MouseDown                                  |  指标移过这个元素的同时按下鼠标按钮时发生。如果 UIElement 是 Button 控制项，表示 Windows Presentation Foundation 未登录这个事件。请改用 PreviewMouseDown 或 Click 事件。        |
|  UIElement.MouseEnter                                 |  当鼠标指标进入这个元素的界限时发生。                                                                                                                |
|  UIElement.MouseLeave                                 |  当鼠标指标离开这个元素的界限时发生。                                                                                                                |
|  UIElement.MouseLeftButtonDown                        |  当鼠标指标在这个元素上的同时按下鼠标左键时发生。                                                                                                          |
|  UIElement.MouseLeftButtonUp                          |  当鼠标指标在这个元素上的同时放开鼠标左键时发生。                                                                                                          |
|  UIElement.MouseMove                                  |  鼠标指标移过这个元素的同时移动鼠标指标时发生。                                                                                                           |
|  UIElement.MouseRightButtonDown                       |  当鼠标指标在这个元素上的同时按下鼠标右键时发生。                                                                                                          |
|  UIElement.MouseRightButtonUp                         |  当鼠标指标在这个元素上的同时放开鼠标右键时发生。                                                                                                          |
|  UIElement.MouseUp                                    |  在这个元素上放开任何鼠标按钮时发生。                                                                                                                |
|  UIElement.MouseWheel                                 |  使用者在鼠标指标于这个元素上的同时滚动鼠标滚轮时发生。                                                                                                       |
|  UIElement.PreviewDragEnter                           |  当输入系统报告出将这个元素当做拖曳目标的基础拖曳事件时发生。                                                                                                    |
|  UIElement.PreviewDragLeave                           |  当输入系统报告出将这个元素当做拖曳来源的基础拖曳事件时发生。                                                                                                    |
|  UIElement.PreviewDragOver                            |  当输入系统报告出将这个元素当做可能放下目标的基础拖曳事件时发生。                                                                                                  |
|  UIElement.PreviewDrop                                |  当输入系统报告出将这个元素当做放下目标的基础放下事件时发生。                                                                                                    |
|  UIElement.PreviewGiveFeedback                        |  在启动拖放作业时发生。                                                                                                                       |
|  UIElement.PreviewGotKeyboardFocus                    |  当键盘将焦点放在此元素时发生。                                                                                                                   |
|  UIElement.PreviewKeyDown                             |  当键盘将焦点放在这个元素上的同时按下按键时发生。                                                                                                          |
|  UIElement.PreviewKeyUp                               |  当键盘将焦点放在这个元素上的同时放开按键时发生。                                                                                                          |
|  UIElement.PreviewLostKeyboardFocus                   |  当键盘不再将焦点放在此元素时发生。                                                                                                                 |
|  UIElement.PreviewMouseDown                           |  指标移过这个元素的同时按下鼠标按钮时发生。                                                                                                             |
|  UIElement.PreviewMouseLeftButtonDown                 |  当鼠标指标在这个元素上的同时按下鼠标左键时发生。                                                                                                          |
|  UIElement.PreviewMouseLeftButtonUp                   |  当鼠标指标在这个元素上的同时放开鼠标左键时发生。                                                                                                          |
|  UIElement.PreviewMouseMove                           |  当鼠标指标在这个元素上的同时移动鼠标指标时发生。                                                                                                          |
|  UIElement.PreviewMouseRightButtonDown                |  当鼠标指标在这个元素上的同时按下鼠标右键时发生。                                                                                                          |
|  UIElement.PreviewMouseRightButtonUp                  |  当鼠标指标在这个元素上的同时放开鼠标右键时发生。                                                                                                          |
|  UIElement.PreviewMouseUp                             |  当鼠标指标在这个元素上的同时放开鼠标按钮时发生。                                                                                                          |
|  UIElement.PreviewMouseWheel                          |  使用者在鼠标指标于这个元素上的同时滚动鼠标滚轮时发生。                                                                                                       |
|  UIElement.PreviewQueryContinueDrag                   |  在拖放作业期间，当键盘或鼠标按钮状态变化时发生。                                                                                                          |
|  UIElement.PreviewStylusButtonDown                    |  当指标在这个元素上的同时按下手写笔按钮时发生。                                                                                                           |
|  UIElement.PreviewStylusButtonUp                      |  当指标在这个元素上的同时放开手写笔按钮时发生。                                                                                                           |
|  UIElement.PreviewStylusDown                          |  当手写笔在这个元素上的同时手写笔接触到数码板时发生。                                                                                                        |
|  UIElement.PreviewStylusInAirMove                     |  当手写笔移到元素上但实际上没有接触数码板时发生。                                                                                                          |
|  UIElement.PreviewStylusInRange                       |  当手写笔相当靠近数码板而能检测到，且手写笔同时在这个元素上时发生。                                                                                                 |
|  UIElement.PreviewStylusMove                          |  当手写笔在元素上的同时移动手写笔时发生。在数码板检测到手写笔时必须移动手写笔以引发这个事件，否则会改为引发 PreviewStylusInAirMove。                                                     |
|  UIElement.PreviewStylusOutOfRange                    |  当手写笔离数码板太远而无法检测到时发生。                                                                                                              |
|  UIElement.PreviewStylusSystemGesture                 |  当使用者执行其中一个手写笔笔势时发生。                                                                                                               |
|  UIElement.PreviewStylusUp                            |  当手写笔在这个元素上的同时，使用者将手写笔移开数码板时发生。                                                                                                    |
|  UIElement.PreviewTextInput                           |  元素使用与装置无关的方法取得文字时发生。                                                                                                              |
|  UIElement.QueryContinueDrag                          |  在拖放作业期间，当键盘或鼠标按钮状态变化时发生。                                                                                                          |
|  UIElement.QueryCursor                                |  在要求显示游标时发生。每次鼠标指标移到新位置时就会在元素上引发这个事件，表示可能需要根据鼠标指标的新位置变化游标物件。                                                                       |
|  UIElement.StylusButtonDown                           |  当指标在这个元素上的同时按下手写笔按钮时发生。                                                                                                           |
|  UIElement.StylusButtonUp                             |  当指标在这个元素上的同时放开手写笔按钮时发生。                                                                                                           |
|  UIElement.StylusDown                                 |  当手写笔在这个元素上的同时手写笔接触到数码板时发生。                                                                                                        |
|  UIElement.StylusEnter                                |  当手写笔进入这个元素的界限时发生。                                                                                                                 |
|  UIElement.StylusInAirMove                            |  当手写笔移到元素上但实际上没有接触数码板时发生。                                                                                                          |
|  UIElement.StylusInRange                              |  当手写笔相当靠近数码板而能检测到，且手写笔同时在这个元素上时发生。                                                                                                 |
|  UIElement.StylusLeave                                |  当手写笔离开元素的界限时发生。                                                                                                                   |
|  UIElement.StylusMove                                 |  当手写笔移到这个元素上时发生。手写笔在数码板上时，必须移动手写笔以引发这个事件，否则会改为引发 StylusInAirMove。                                                                  |
|  UIElement.StylusOutOfRange                           |  手写笔离数码板太远而无法检测到，且手写笔同时在这个元素上时发生。                                                                                                  |
|  UIElement.StylusSystemGesture                        |  当使用者执行其中一个手写笔笔势时发生。                                                                                                               |
|  UIElement.StylusUp                                   |  手写笔在这个元素上的同时，使用者将手写笔移开数码板时发生。                                                                                                     |
|  UIElement.TextInput                                  |  元素使用与装置无关的方法取得文字时发生。                                                                                                              |
|  Window.Activated                                     |  视窗变成前景视窗时发生。                                                                                                                      |
|  Window.Closed                                        |  即将关闭视窗时发生。                                                                                                                        |
|  Window.Closing                                       |  呼叫Close 之后立即发生，并可用来处理取消关闭视窗。                                                                                                      |
|  Window.ContentRendered                               |  在显示视窗的内容之后发生。                                                                                                                     |
|  Window.Deactivated                                   |  视窗变成背景视窗时发生。                                                                                                                      |
|  Window.LocationChanged                               |  视窗的位置变化时发生。                                                                                                                       |
|  Window.SourceInitialized                             |  在建立视窗的 HwndSource 物件之后，视窗显示之前发生。                                                                                                  |
|  Window.StateChanged                                  |  视窗的 WindowState 属性变化时发生。                                                                                                          |
