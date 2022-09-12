```plantuml
@startuml
digraph g {
graph [
rankdir = "LR"
];
node [
fontsize = "16"
shape = "ellipse"
];
edge [
];
"node0" [
label = "<f0> random.sol"
shape = "record"
];
"node1" [
label = "<f0> test"
shape = "record"
];
"node2" [
label = "<f0> metacoin.js"
shape = "record"
];
"node3" [
label = "<f0>test1.sol"
shape = "record"
];
"node4" [
label = "<f0> test2.js"
shape = "record"
];
"node5" [
label = "<f0> TestMetaCoin.sol"
shape = "record"
];
"node6" [
label = "<f0> sub_directory"
shape = "record"
];
"node7" [
label = "<f0> sub__sub_directory"
shape = "record"
];
"node8" [
label = "<f0> sub__sub_directory2"
shape = "record"
];
"node9" [
label = "<f0> symlink1 | <f1> Pointing to: sub_sub_directory"
shape = "record"
];
"node10" [
label = "<f0> symlink3 | <f1> Pointing to: random.sol"
shape = "record"
];
"node11" [
label = "<f0> symlink2 | <f1> Pointing to: sub_directory"
shape = "record"
];
"node12" [
label = "<f0> test3.sol"
shape = "record"
];
"node13" [
label = "<f0> test4.js"
shape = "record"
];
"node14" [
label = "<f0> test5.js"
shape = "record"
];
"node15" [
label = "<f0> test6.sol"
shape = "record"
];
"node16" [
label = "<f0> test7.sol"
shape = "record"
];
"node17" [
label = "<f0> sub_sub_directory2"
shape = "record"
];
"node18" [
label = "<f0> one_more_sub"
shape = "record"
];
"node19" [
label = "<f0> one_more_sub2"
shape = "record"
];
"node20" [
label = "<f0> test8.sol through test11.sol"
shape = "record"
];
"node21" [
label = "<f0> one_more_sub2"
shape = "record"
];
"node22" [
label = "<f0> test12.sol - test15.sol"
shape = "record"
];
"node23" [
label = "<f0> js_only_subdir"
shape = "record"
];
"node24" [
label = "<f0> solidity_only_subdir"
shape = "record"
];
"node25" [
label = "<f0> test19.js - test20.js"
shape = "record"
];
"node26" [
label = "<f0> test16.sol - test18.sol"
shape = "record"
];
"node0":f0 -> "node1":f0 [
id = 0
];
"node1":f0 -> "node2":f0 [
id = 2
];
"node1":f0 -> "node3":f0 [
id = 2
];
"node1":f1 -> "node4":f0 [
id = 3
];
"node1":f1 -> "node5":f0 [
id = 3
];
"node1":f1 -> "node6":f0 [
id = 3
];
"node6":f1 -> "node7":f0 [
id = 3
];
"node6":f1 -> "node8":f0 [
id = 3
];
"node6":f1 -> "node9":f0 [
id = 3
];
"node6":f1 -> "node10":f0 [
id = 3
];
"node7":f1 -> "node11":f0 [
id = 3
];
"node7":f1 -> "node12":f0 [
id = 3
];
"node7":f1 -> "node13":f0 [
id = 3
];
"node8":f1 -> "node14":f0 [
id = 3
];
"node8":f1 -> "node15":f0 [
id = 3
];
"node8":f1 -> "node16":f0 [
id = 3
];
"node8":f1 -> "node17":f0 [
id = 3
];
"node17":f1 -> "node18":f0 [
id = 3
];
"node17":f1 -> "node19":f0 [
id = 3
];
"node18":f1 -> "node20":f0 [
id = 3
];
"node19":f1 -> "node21":f0 [
id = 3
];
"node19":f1 -> "node22":f0 [
id = 3
];
"node21":f1 -> "node23":f0 [
id = 3
];
"node21":f1 -> "node24":f0 [
id = 3
];
"node23":f1 -> "node25":f0 [
id = 3
];
"node24":f1 -> "node26":f0 [
id = 3
];
}
@enduml
```