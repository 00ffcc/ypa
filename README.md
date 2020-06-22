# ypa
一个`c++`数据生成和对拍库

## IO

`IO::IO("ypa_test.in");`向`ypa_test.in`中输入数据

`IO::IO("ypa_test_%d_%d_%d.in",192,60,817);`向`ypa_test_192_60_817.in`中输入数据
## Rand
`int re=Rand::random<int>();`生成一个数

`int re=Rand::random(19260817);`生成一个 <img src="http://00ffcc.cf/images/MommyTalk159282195765445.png" width = "100" height = "25" alt="" align=center /> 的数

`int re=Rand::random(2333,19260817);`生成一个 <img src="http://00ffcc.cf/images/MommyTalk159282199645326.png" width = "150" height = "25" alt="" align=center /> 的数
## Pair
`pair<int,int> re=Pair::Pair(19,260817);`生成一个`std::pair<int,int>`,保证 <img src="http://00ffcc.cf/images/MommyTalk159282201943832.png" width = "200" height = "25" alt="" align=center /> 且 <img src="http://00ffcc.cf/images/MommyTalk159282203824389.png" width = "300" height = "25" alt="" align=center />

`Pair::Print(re)`输出这个`pair`并换行

`Pair::Print(re,' ');`输出这个`pair`并在其后输出`' '`,不换行
## Vector 
`vector<int> re=Vector<int>({23,33,333},{192,60,817});`生成一个有`3`个元素,分别 <img src="http://00ffcc.cf/images/MommyTalk159282206336941.png" width = "400" height = "25" alt="" align=center /> 的向量

`Vector::Print(re);`输出这个向量并换行

`Vector::Print(re,' ');`输出这个向量并在其后输出`' '`,不换行
## UFS
`UFS::UFS<10000> S;`创建并初始化一个大小为`10000`的并查集,从`0`开始标号

`S.IsSplit(x,y);`查询`x`,`y`是否处在两个不同的集合

`S.merge(x,y);`合并`x`,`y`所在集合
## Tree
`vector<pair<int,int> > re=Tree::Tree(50000);`生成一棵有`50000`个节点的树

`for(auto i:re)Pair::Print(i);`输出这棵树

## Atlas
`vector<pair<int,int> > re=Atlas::Atlas(50000,500000);`生成一张有`50000`个点,`500000`条边的联通图

`for(auto i:re)Pair::Print(i);`输出这张图
## Cactus
`vector<pair<int,int> >re=Cactus::Cactus(50000,500000,0.8);`生成一个有`50000`个点,**至多**`500000`条边的仙人掌,`0.8`是`炼铜系数`,越大联通块个数越少,为`1`是保证联通

`fprintf(IO::In,"%d %d\n",50000,re.size());`输出这个仙人掌的点数和边数

`for(auto i:re)Pair::Print(i);`输出这个仙人掌
## Function
`Function::Function("std_check.exe","ypa_test.in","ypa_test.out");`运行`std_check.exe`,从`ypa_test.in`中读取数据,输入到`ypa_test.out`中

## Fc
`Fc::Fc("ypa_test.out","ypa_test.ans");`判断`ypa_test.out`与`ypa_test.ans`是否相等

## std
`fclose(IO::In);`关闭文件,以供其他进程读取

