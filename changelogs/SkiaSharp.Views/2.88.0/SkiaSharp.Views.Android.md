# API diff: SkiaSharp.Views.Android.dll

## SkiaSharp.Views.Android.dll

> Assembly Version Changed: 2.88.0.0 vs 2.80.0.0

### Namespace SkiaSharp.Views.Android

#### Type Changed: SkiaSharp.Views.Android.Resource

#### Type Changed: SkiaSharp.Views.Android.Resource.Attribute

Added field:

```csharp
public static int ignorePixelScaling;
```


#### New Type: SkiaSharp.Views.Android.Resource.Styleable

```csharp
public class Styleable {
	// fields
	public static int[] SKCanvasView;
	public static int SKCanvasView_ignorePixelScaling;
}
```


#### Type Changed: SkiaSharp.Views.Android.SKPaintGLSurfaceEventArgs

Obsoleted constructors:

```diff
 [Obsolete ()]
 public SKPaintGLSurfaceEventArgs (SkiaSharp.SKSurface surface, SkiaSharp.GRBackendRenderTarget renderTarget, SkiaSharp.GRSurfaceOrigin origin, SkiaSharp.SKColorType colorType, SkiaSharp.GRGlFramebufferInfo glInfo);
```

Added constructors:

```csharp
public SKPaintGLSurfaceEventArgs (SkiaSharp.SKSurface surface, SkiaSharp.GRBackendRenderTarget renderTarget, SkiaSharp.GRSurfaceOrigin origin, SkiaSharp.SKImageInfo info);
public SKPaintGLSurfaceEventArgs (SkiaSharp.SKSurface surface, SkiaSharp.GRBackendRenderTarget renderTarget, SkiaSharp.GRSurfaceOrigin origin, SkiaSharp.SKImageInfo info, SkiaSharp.SKImageInfo rawInfo);
```

Added properties:

```csharp
public SkiaSharp.SKImageInfo Info { get; }
public SkiaSharp.SKImageInfo RawInfo { get; }
```


#### Type Changed: SkiaSharp.Views.Android.SKPaintSurfaceEventArgs

Added constructor:

```csharp
public SKPaintSurfaceEventArgs (SkiaSharp.SKSurface surface, SkiaSharp.SKImageInfo info, SkiaSharp.SKImageInfo rawInfo);
```

Added property:

```csharp
public SkiaSharp.SKImageInfo RawInfo { get; }
```



