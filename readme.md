# OpenCC.NET GUI

![](opencc-net-gui.png)

## 介紹

OpenCC.NET GUI 是基於 OpenCC (Open Chinese Convert, 開放中文轉換)，使用 [OpenCC.NET](https://github.com/CosineG/OpenCC.NET) 實現的中文轉換工具，支持中文簡繁體之間詞彙級別的轉換，同時還支持地域間異體字以及詞彙的轉換。

## 功能

- 支持文本和批量文件的簡繁轉換。
- 文件格式：支持純文本、Word (`.docx`)、Excel (`.xlsx`) 和 PowerPoint (`.pptx`)。暫不支持 PDF 格式。
- 轉換選項：
  - 可自定義原文、目標格式（簡/繁）。
  - 支持 OpenCC、臺灣、香港異體字標準。
  - 支持大陸、臺灣地區詞彙轉換。
  - 可選「最大匹配」或「結巴分詞」模式。


## 開始

### 獲取

可以直接在倉庫頁面右側獲取最新Release版本，或下載源碼後自行編譯。若無法運行，請確保安裝了 [.NET 8 運行時](https://dotnet.microsoft.com/zh-cn/download/dotnet/thank-you/runtime-desktop-8.0.22-windows-x64-installer)。

### 使用

軟件提供了文本編輯轉換和文件批量轉換兩種功能。

#### 文本編輯轉換

此模式下直接在文本框中輸入你所需要轉換的語句，在右側選擇轉換選項後，點擊轉換按鈕即可得到結果。

![](screenshot-1.png)

#### 文件批量轉換

此模式下可以批量導入文件進行轉換。當前支持純文本和 `.docx`, `.pptx`, `.xlsx` 格式，未知格式將默認按照純文本進行轉換，暫不支持 PDF。

![](screenshot-2.png)

## 引用

### OpenCC.NET

[OpenCC.NET](https://github.com/CosineG/OpenCC.NET)實現文本轉換。

### OpenCC

[OpenCC](https://github.com/BYVoid/OpenCC)為OpenCC.NET提供詞庫。

### jieba.NET

[jieba.NET](https://github.com/anderscui/jieba.NET)為OpenCC.NET提供分詞。

### ModernWpf

[ModernWpf](https://github.com/Kinnara/ModernWpf)提供UI控件。

### Ookii.Dialogs.Wpf

[Ookii.Dialogs.Wpf](https://github.com/ookii-dialogs/ookii-dialogs-wpf)提供選擇文件夾窗口（沒錯，WPF沒有自帶選擇文件夾窗口）。
