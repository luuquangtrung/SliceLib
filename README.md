# SliceLib
SliceLib is a library of test instances for network slice embedding problem


Format of each instance:

```
0 # identifier of network trace ('0': synthetic, '1': real)
2 # nb of slices

1 1 0 2		# [SLICE 1] slice id - slice_weight - slice_arrival_time - num_sfcs

1 3 2  		# [SFC 1 OF SLICE 1] sfc_id - num_vnodes - num_vlinks
1 10 10 10 10	# vnode_id - attribute_1 - attribute_2 - attribute_3 - attribute_4
2 10 10 10 10
3 10 10 10 10
1 1 2 10 10     # vlink_id - ingress - egress - attribute_1 - attribute_2
2 2 3 10 10

2 3 2           # [SFC 2 OF SLICE 1] ...
1 10 10 10 10	
2 10 10 10 10
3 10 10 10 10
1 1 2 10 10		
2 2 3 10 10


2 1 0 1		# [SLICE 2] ...

1 3 2  		# [SFC 1 OF SLICE 2] ...
1 10 10 10 10	
2 10 10 10 10
3 10 10 10 10
1 1 2 10 10		
2 2 3 10 10

4 4        # [PHYSICAL NETWORK] num_nodes num_links

1 10 10 10 10	# node_id - attribute_1 - attribute_2 - attribute_3	- attribute_4	
2 10 10 10 10
3 10 10 10 10
4 10 10 10 10

1 1 2 10 10     # link_id - ingress - egress - attribute_1 - attribute_2
2 2 3 10 10
3 3 4 10 10
4 1 1 10 10

```

#### Authors
* [Quang-Trung Luu](https://luuquangtrung.github.io/)
* TBD

(c) 2023 School of Electrical and Electronic Engineering, Hanoi University of Science and Technology (SEEE, HUST)
