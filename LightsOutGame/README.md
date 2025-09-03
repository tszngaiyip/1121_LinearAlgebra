# C# 點燈遊戲 (Lights Out Game)

## 🎮 遊戲介紹 / Game Introduction

點燈遊戲（Lights Out）是一個經典的數學謎題遊戲。玩家需要將所有的燈泡都點亮（或全部熄滅），每次點擊一個燈泡時，該燈泡及其相鄰的燈泡都會改變狀態。

Lights Out is a classic mathematical puzzle game. Players need to turn on all lights (or turn off all lights). When clicking a light, both the light itself and its adjacent lights will change state.

## 🎯 遊戲目標 / Game Objective

- **目標：** 將所有燈泡變為相同狀態（全亮或全暗）
- **規則：** 點擊任何燈泡會改變該燈泡及其上下左右相鄰燈泡的狀態
- **挑戰：** 用最少的步數達成目標

**Objective:** Make all lights the same state (all on or all off)  
**Rules:** Clicking any light changes its state and the state of its adjacent lights (up, down, left, right)  
**Challenge:** Achieve the goal with minimum steps

## 🖼️ 遊戲截圖 / Game Screenshot

![Demo](demo.png)

*遊戲運行界面 / Game interface*

## 🔢 線性代數原理 / Linear Algebra Principles

點燈遊戲本質上是一個線性代數問題：

The Lights Out game is essentially a linear algebra problem:

### 數學模型 / Mathematical Model

- **狀態向量：** 用二進制向量表示每個燈泡的狀態（0=熄滅，1=點亮）
- **變換矩陣：** 每次點擊操作可以用矩陣乘法表示
- **解的存在性：** 通過矩陣的行列式和核空間分析遊戲的可解性

**State Vector:** Binary vector representing each light's state (0=off, 1=on)  
**Transformation Matrix:** Each click operation can be represented by matrix multiplication  
**Solution Existence:** Analyze game solvability through matrix determinant and null space

### 數學公式 / Mathematical Formula

```
初始狀態 + Σ(點擊操作矩陣) ≡ 目標狀態 (mod 2)
Initial State + Σ(Click Operation Matrix) ≡ Target State (mod 2)
```

## 🛠️ 技術實現 / Technical Implementation

### 核心功能 / Core Features

- **圖形界面：** 使用WinForms或WPF實現互動式遊戲界面
- **遊戲邏輯：** 實現燈泡狀態的切換邏輯
- **求解算法：** 使用高斯消元法求解最優解
- **步數統計：** 記錄玩家的操作步數

**Graphics Interface:** Interactive game interface using WinForms or WPF  
**Game Logic:** Implementation of light state toggling logic  
**Solving Algorithm:** Using Gaussian elimination to find optimal solutions  
**Step Counter:** Track player's number of moves

### 系統要求 / System Requirements

- .NET Framework 4.5 或更高版本
- Windows 操作系統
- Visual Studio 2017 或更高版本

## 🚀 使用說明 / Usage Instructions

### 編譯執行 / Compilation and Execution

1. 開啟 `s1111452_hw1.sln` 解決方案檔案
2. 在Visual Studio中編譯專案
3. 執行生成的程式
4. 按照遊戲規則進行操作

### 遊戲操作 / Game Controls

- **滑鼠點擊：** 點擊任意燈泡以切換狀態
- **重新開始：** 點擊重置按鈕開始新遊戲
- **提示功能：** 查看最優解的提示

## 📊 演算法複雜度 / Algorithm Complexity

- **時間複雜度：** O(n³) - 高斯消元法求解
- **空間複雜度：** O(n²) - 儲存變換矩陣
- **最優解：** 保證找到最少步數的解（如果存在）

**Time Complexity:** O(n³) - Gaussian elimination  
**Space Complexity:** O(n²) - Store transformation matrix  
**Optimal Solution:** Guaranteed to find minimum-step solution (if exists)