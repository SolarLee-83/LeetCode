### 2680.Maximum-OR

显然最贪心的策略是，我们将最高位的bit 1推地越远越好，最终的答案一定最大。所以直观上，我们应该把k次机会都给最大的元素，才能更高效地提升最高位的1。

但是从例子中可以发现，如果有多个元素都含有相同最高位的1，不见得推最大元素是最优解。那么没关系，我们每个元素都试一下抬高k位的效果，取最大值即可。时间复杂度就是o(N).