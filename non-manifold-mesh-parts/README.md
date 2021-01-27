# Non-manifold mesh parts

## Goal

When working with polygonal meshes it is convenient and more efficient to work with so called [manifold](https://en.wikipedia.org/wiki/Manifold) meshes. So our goal for this task is to detect topologically non-manifold mesh parts. This means that we only need to consider mesh connectivity for vertices, edges and faces and can ignore mesh geometry.

## Non-manifold topology

Here are the examples of non-manifold topology that we need to detect in the input mesh:

![Non-manifold topology](./non-manifold-topology.png)

## Input mesh

For this task input mesh will be triangular mesh, i.e. all its faces will be triangles. The mesh should be loaded from the [OFF file](https://en.wikipedia.org/wiki/OFF_(file_format)), it is a simple text file. No need to support optional parts like comments or colors. Example files with meshes can be found in [example-meshes](./example-meshes) directory.

