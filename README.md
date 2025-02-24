# julia2

# Julia データ分析リポジトリ

このリポジトリには、データ操作、統計分析、および可視化を行うためのJuliaスクリプトとQuartoドキュメントが含まれています。主な焦点は、さまざまなJuliaパッケージを使用してデータ分析を行うことです。

## 内容

- `test.qmd`: Juliaを使用したさまざまなデータ分析手法を示すQuartoドキュメント。

## 使用されるパッケージ

このリポジトリで使用されるJuliaパッケージは以下の通りです：

- `Turing`
- `QuartoNotebookRunner`
- `RDatasets`
- `CategoricalArrays`
- `Chain`
- `CSV`
- `DataFrames`
- `DataFramesMeta`
- `TableOne`
- `Distributions`
- `GLM`
- `StatsBase`
- `StatsPlots`
- `MixedModels`
- `Survival`
- `CairoMakie`
- `Gadfly`

## test.qmd

`test.qmd` ファイルは、Juliaを使用したデータ操作、統計分析、および可視化のさまざまな例を含むQuartoドキュメントです。このドキュメントは以下のトピックをカバーしています：

1. **Basic Data Preparation**：
    - CSVファイルからのデータ読み込み。
    - 列の名前変更。
    - データの選択とフィルタリング。

2. **Data wrangling such as filter and select**：
    - データの構造を記述。
    - 条件に基づく行のフィルタリング。
    - 条件に基づく列の選択。

3. **Mutate and missing wrangling**：
    - 新しい列の追加。
    - 既存の列の変換。
    - 欠損値の処理。

4. **Grouping and aggregation**：
    - 1つ以上の列でデータをグループ化。
    - 各グループの要約統計量を計算。

5. **Basic statistical analysis and survival analysis**：
    - 記述表（Table 1）の作成。
    - 一般化線形モデル（GLM）の適合。
    - 混合モデルの適合。
    - 生存分析の実施。

6. **Visualization**：
    - カプラン・マイヤー曲線の作成。
    - 信頼区間付きの生存率の可視化。
    - リスクにさらされている数のプロット。

## 実行方法

`test.qmd` の例を実行するには、Juliaと必要なパッケージをインストールする必要があります。以下のコマンドをJulia REPLで実行してパッケージをインストールできます：

```julia
using Pkg

Pkg.add(
    "Turing")

Pkg.add([
    "QuartoNotebookRunner", "RDatasets", "CategoricalArrays", "Chain", 
    "CSV", "DataFrames", "DataFramesMeta", "TableOne", "Distributions", "GLM", 
    "StatsBase", "StatsPlots", "MixedModels", "Survival", "CairoMakie", "Gadfly"
])
```

1: add Turing
2: add QuartoNotebookRunner, RDatasets, CategoricalArrays, Chain, CSV , DataFrames, DataFramesMeta, TableOne, Distributions, GLM, StatsBase, StatsPlots,  MixedModels, Survival, CairoMakie, Gadfly

