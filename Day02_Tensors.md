ABOUT TENSORS :-
The shape tells the whole story. When you see (32, 3, 224, 224) in code, read it right to left — 224×224 spatial grid, 3 colour channels, 32 of them in a batch.

When asked "what's a tensor?" — say: "A generalization of scalars, vectors, and matrices to arbitrary dimensions. Shape tells you exactly what each axis means."
When asked about batch dimension — say: "We add it at axis 0 so we can process multiple samples in parallel on the GPU. PyTorch's convention is always (batch, ...)."
When asked about 5D — say: "Typical for video models. Shape (N, T, C, H, W) — batch, time, channels, height, width. You'd see this in 3D Conv networks like C3D or SlowFast."
