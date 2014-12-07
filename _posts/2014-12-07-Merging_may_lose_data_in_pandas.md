---
layout: post
title: Merging may lose data in Pandas
---

When I use Pandas, I've ran into some cases that it lost the data after merging two DataFrames.

This is because that the two DataFrames may have different dtypes on the "same" column. As by default, the dtypes are inferred by the first portion of the data. So we may come into cases that the "same" column got inferred as numbers(the special cases) and string(object type in Pandas terminology) types in two different DataFrames.

(Example would be provided later.)

To fix this, we can specify the dtype when we read in the data:

	df = pandas.read_csv(csv_file, dtype={column1: np.object, column2: np.float64})

