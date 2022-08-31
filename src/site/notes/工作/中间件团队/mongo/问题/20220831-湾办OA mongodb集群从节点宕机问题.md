---
{"dg-publish":true,"permalink":"///mongo//20220831-oa-mongodb/","tags":"gardenEntry","dgHomeLink":true,"dgPassFrontmatter":false}
---


71从节点于12:21宕机，原因为主节点oplog容量太小，在数据并发量高的时候，从节点拉取oplog速度赶不上，会导致宕机。后续优化方案：扩容，并保证主从节点磁盘大小一致