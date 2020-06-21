# ypa
一个`c++`数据生成和对拍库

## IO

`IO::IO("ypa_test.in");`向`ypa_test.in`中输入数据

`IO::IO("ypa_test_%d_%d_%d.in",192,60,817);`向`ypa_test_192_60_817.in`中输入数据

## Vector 
`vector<int> re=Vector<int>({23,33,333},{192,60,817});`生成一个有`3`个元素,分别 $\in [23,192],\in [33,60],\in [333,817]$ 的向量

`Vector::Print(re);`输出这个向量并换行

`Vector::Print(re,' ');`输出这个向量并在其后输出`' '`,不换行

## Tree
`vector<pair<int,int> > re=Tree::Tree(50000);`生成一棵有`50000`个节点的树

`for(auto i:re)Pair::Print(i);`输出这棵树

## Cactus

`vector<pair<int,int> >re=Cactus::Cactus(50000,500000,0.8);`


`fprintf(IO::In,"%d %d\n",50000,re.size());`

`for(auto i:re)Pair::Print(i);`

`fclose(IO::In);`

`Function::Function("std_check.exe","ypa_test.in","ypa_test.out");`