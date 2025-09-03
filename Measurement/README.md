# C# 幾何測量系統 (Geometric Measurement System)

## 📐 功能概述 / Feature Overview

這是一個使用C#開發的幾何測量系統，能夠計算並報告各種幾何圖形的距離和面積。

This is a geometric measurement system developed in C# that can calculate and report distances and areas of various geometric shapes.

## 📊 支援的圖形 / Supported Shapes

系統支援以下幾何圖形的測量：

The system supports measurement of the following geometric shapes:

- **線段 (Line)** - 計算長度 / Calculate length
- **三角形 (Triangle)** - 計算周長和面積 / Calculate perimeter and area
- **矩形 (Rectangle)** - 計算周長和面積 / Calculate perimeter and area
- **五邊形 (Pentagon)** - 計算周長和面積 / Calculate perimeter and area
- **多邊形 (Polygon)** - 計算一般多邊形的周長和面積 / Calculate perimeter and area of general polygons
- **橢圓 (Ellipse)** - 計算周長和面積 / Calculate perimeter and area

## 🖼️ 程式展示 / Program Demo

![Demo](demo.png)

*程式運行界面展示 / Program interface demonstration*

![Screenshot](2023-12-03_21_001.png)

*實際測量結果截圖 / Actual measurement results screenshot*

## 🎯 線性代數應用 / Linear Algebra Applications

此專案中應用的線性代數概念包括：

Linear algebra concepts applied in this project include:

- **向量運算** - 計算點之間的距離和方向 / Vector operations for distance and direction calculations
- **矩陣變換** - 幾何圖形的座標變換 / Matrix transformations for geometric coordinate transformations
- **行列式** - 計算三角形和多邊形面積 / Determinants for calculating triangle and polygon areas
- **內積和外積** - 角度和面積計算 / Dot and cross products for angle and area calculations

## 🚀 使用方法 / Usage

### 執行環境要求 / System Requirements

- .NET Framework 或 .NET Core
- Visual Studio 或其他C#開發環境

### 編譯與執行 / Compilation and Execution

1. 開啟專案目錄中的解決方案檔案
2. 使用Visual Studio編譯專案
3. 執行生成的可執行檔案
4. 按照介面提示輸入幾何圖形的參數
5. 查看計算結果

```bash
# 如果使用命令列編譯
dotnet build
dotnet run
```

## 📁 專案結構 / Project Structure

```
exLAHomework4/
├── Program.cs          # 主程式入口
├── Shape.cs           # 幾何圖形基類
├── Triangle.cs        # 三角形類別
├── Rectangle.cs       # 矩形類別
├── Pentagon.cs        # 五邊形類別
├── Polygon.cs         # 多邊形類別
├── Ellipse.cs         # 橢圓類別
└── MathHelper.cs      # 數學輔助函數
```

## 📈 計算精度 / Calculation Precision

- 使用雙精度浮點數進行計算
- 支援小數點後多位精度
- 包含錯誤處理機制
