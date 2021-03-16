# 輸入優化

在有些比較惡劣的題目中，出題者會故意用測資卡你的輸出輸入時間，在即使兩個 code 的複雜度都一樣，只要優化輸出卻可以 AC 的情況
，本篇將介紹數個方法可以優化輸出輸入的時間。

## cin/cout

在 code 開頭加上以下 macro

```cpp
#define USE_CPPIO() ios_base::sync_with_stdio(0); cin.tie(0)
```

並在 `main()` 的一開始加上 `USE_CPPIO();`

```cpp
int main()
{
    USE_CPPIO();
    
    /* ... */
}
```

!!! danger
    接著你的 code 輸出就只能使用 `cin/cout` 注意不能跟 `printf/scanf` 混用。


另外記得換行使用 `\n' 代替 `endl` 

## Reference

<https://chino.taipei/note-2016-0311C-%E7%9A%84%E8%BC%B8%E5%87%BA%E5%85%A5cin-cout%E5%92%8Cscanf-printf%E8%AA%B0%E6%AF%94%E8%BC%83%E5%BF%AB%EF%BC%9F/>

<https://hackmd.io/@wiwiho/CPN-io-optimization>
