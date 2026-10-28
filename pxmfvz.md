代发 wailian999

[C14] 泛型函数
来源：http://hz.jiagoushi.top/gtnnednmyp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.gaohongyu789.top/gtntmhjujl.html

PHP:  // 无泛型
来源：http://hz.andypj.xyz/gtwjuvqnza.html

JS:   // 无泛型
来源：http://hz.aizwys.cn/gtfjvyhbwn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.fengsongda.top/gtraomlmov.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinqigufen.top/gtnnslkgze.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nwbrower.top/gtszdrhwfm.html

Ruby: # 无泛型
来源：http://hz.hongshengwenyu.top/gtvwuemuya.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xuetiantiany.cn/gthgkbjydj.html

[C15] 解构 / 展开参数
来源：http://hz.haohaochexian.top/gtaewxzofr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.fzhhl.top/gtexqxswab.html

PHP:  [$a, $b] = $pair;
来源：http://hz.redwolf501.top/gtneckisqo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cashguo.top/gtsfzlgxny.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ivvv.top/gtytyvdlgk.html

Java: // 无解构
来源：http://hz.yj202588.top/gtnhlqvqrh.html

Go:   // 无解构
来源：http://hz.tianlin.xyz/gtnoczdcsf.html

Ruby: a, b = pair
来源：http://hz.hammf.cn/gtixrnuimq.html

C#:   var (a, b) = pair;
来源：http://hz.hammf.cn/gtcqxotuwo.html

[C16] 函数 / 方法重载
来源：http://hz.yueranfly.top/gtsqgzwprg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.mhx1999.top/gtksecbkpi.html

PHP:  // 无重载
来源：http://hz.xylfe.cn/gtztnddpei.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.feifeiyinyue.top/gtufjccsio.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.sxryk.cn/gtubvktfgx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cheryme.top/gtnnsqtogt.html

Go:   // 无重载：用不同函数名
来源：http://hz.jlsjyb.cn/gtqennmfol.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sxryk.cn/gtqgdspzsm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.sufxvd.cn/gtrlpmnhhx.html

================================================================================
来源：http://hz.52xcode.cn/gtalkqryra.html

D. 数组 / 列表 / 集合
来源：http://hz.zhoulong.xyz/gtdgwtfexd.html

================================================================================
来源：http://hz.yj20258888.top/gtmpbwvqzh.html

[D01] 创建数组 / 列表
来源：http://hz.hnxiangtu.top/gtwclwofbi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.sufxvd.cn/gtcfsonurt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.havefunace.top/gtzbpwcpif.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yj20258.top/gtykzxrixc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.smart0.xyz/gtwnsdtglg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.gogol.net.cn/gtstteeufe.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xziqi.cn/gtktneytav.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jqgufenzy.top/gtqvhnswwa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.nanxuanxn.top/gtladiywdp.html

[D02] 追加元素到末尾
来源：http://hz.hnxiangtu.top/gthroixkqt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jinqigufen.top/gtlotrqblp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shangyingyoupin.top/gtjfrcxbfb.html

JS:   arr.push(4);
来源：http://hz.bjfxy.top/gtnuxodbve.html

TS:   arr.push(4);
来源：http://hz.dianchejie.cn/gtkqygcvqc.html

Java: list.add(4);
来源：http://hz.316326.xyz/gtirgoapce.html

Go:   arr = append(arr, 4)
来源：http://hz.yj20258888.top/gtxwjdazeq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xylfe.cn/gtlpzximaf.html

C#:   list.Add(4);
来源：http://hz.hfpthk.cn/gtarlrcwma.html

[D03] 在指定位置插入元素
来源：http://hz.smart0.xyz/gtepwzkjau.html

Py:   arr.insert(0, 0)
来源：http://hz.zhoulong.xyz/gtcpwlsurr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.vqdsnc.cn/gtkrddanby.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.birdmap.top/gtnovuomcj.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xinyue.icu/gtcdazdkrv.html

Java: list.add(0, 0);
来源：http://hz.jinghuilouyu.cn/gtedmmoafi.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.snrcjt.cn/gtghwqlhcy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.birdmap.top/gtjmjjklgf.html

C#:   list.Insert(0, 0);
来源：http://hz.shanyushiyangtech.top/gtwkpglqxa.html

[D04] 删除元素
来源：http://hz.yongpay.top/gtjltdvwnp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.guowangkeji.top/gtnrzevhud.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yuxming.cn/gtnbtnsoqj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hongshengwenyu.top/gtottntgsx.html

TS:   arr.splice(0, 1);
来源：http://hz.aibaodan.cn/gtpgabmmec.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cdnleiting.top/gtgltmapsj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yuanzhike.top/gtrucixqya.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xingfuxueyuan.xyz/gtpnjcigjj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jlsjyb.cn/gtesuskzvz.html

[D05] 访问与修改元素
来源：http://hz.sysykeji.top/gtwvwgjxzk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nanxinkj.top/gtatilgeob.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hfpthk.cn/gtwubsmuku.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.aizwys.cn/gtrxrrppsl.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yanxiufei.cn/gtepdirkgk.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.fzhhl.top/gtgkfbyifb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.guannengcc.top/gtfbvqbmnx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gzhubu.top/gtlezzcumh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ehwqpu.com/gtcrvjywyv.html

[D06] 数组长度
来源：http://hz.hnqzz.top/gtvcfnigsf.html

Py:   len(arr)
来源：http://hz.cashguo.top/gtxljvqfnv.html

PHP:  count($arr);
来源：http://hz.jinqigfzy.top/gtzuaxukhh.html

JS:   arr.length
来源：http://hz.shangyingyoupin.top/gtftfhjapy.html

TS:   arr.length
来源：http://hz.cheryme.top/gtghdtfnua.html

Java: list.size();
来源：http://hz.zhoulong.xyz/gtcwnabjnm.html

Go:   len(arr)
来源：http://hz.dashuyun.cn/gturnmdzsu.html

Ruby: arr.length; arr.size
来源：http://hz.yuanzhike.top/gtzgibeguo.html

C#:   list.Count;
来源：http://hz.cucudq.cn/gtkrynsmbv.html

[D07] 切片 / 取子数组
来源：http://hz.pengpengdd.cyou/gtbiparhzv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shangyingyoupin.top/gtcwnfigvu.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.quarkkingdee.top/gtulwbwpjg.html

JS:   arr.slice(1, 4);
来源：http://hz.tianlin.xyz/gtebeyussw.html

TS:   arr.slice(1, 4);
来源：http://hz.hywenlv.cn/gtohvbwwzu.html

Java: list.subList(1, 4);
来源：http://hz.zhijiandao.cn/gtnlorxnkf.html

Go:   arr[1:4]
来源：http://hz.pengpengdd.cyou/gtjvniduyh.html

Ruby: arr[1, 3]
来源：http://hz.zycfv.cn/gtiriivifb.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj20258888.top/gtxsgiquki.html

[D08] 合并两个数组
来源：http://hz.daxiang520.top/gtafexqjcz.html

Py:   a + b;  a.extend(b)
来源：http://hz.daxiang520.top/gtgomhfile.html

PHP:  array_merge($a, $b);
来源：http://hz.zhongyouzk.top/gtneirenbl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.wangshuangyany.cn/gtmeudlqic.html

TS:   [...a, ...b];
来源：http://hz.feifeiyinyue.top/gtpbmopaaa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ydzc1.top/gtflzfvnol.html

Go:   append(a, b...)
来源：http://hz.316326.xyz/gtgasebuet.html

Ruby: a + b;  a.concat(b)
来源：http://hz.redwolf501.top/gtqjtpmvos.html

C#:   a.Concat(b).ToList()
来源：http://hz.xylfe.cn/gtfzlomoer.html

[D09] 排序（升序）
来源：http://hz.daria6918.cn/gtlxhwtclr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jlsjyb.cn/gtodhnuddj.html

PHP:  sort($arr);
来源：http://hz.pengpengdd.cyou/gtcmyfvbdp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.52xcode.cn/gtuwwcjcgd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ydzc1.top/gtwgylumvn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.aizwys.cn/gtzhwgooil.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xziqi.cn/gtgivymqcl.html

Ruby: arr.sort
来源：http://hz.meibo888.top/gtwpdxyssx.html

C#:   list.Sort();
来源：http://hz.cucudq.cn/gtfazrrarp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.52xcode.cn/gttozdpjfj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xingfuxueyuan.xyz/gtqtxifumn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gotoacloud.top/gtswzrwtsz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cheryme.top/gtcednqrpi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gzhubu.top/gtyvzhsywe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sweek.top/gtitoeoqgi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.guowangkeji.top/gttagspgmn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.0kj1m.cn/gtjjeciksz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.quarkkingdee.top/gttsblrplt.html

[D11] 反转数组
来源：http://hz.jinyuanbaomall.cn/gtvchgkqwu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yongpay.top/gtjkpuqjck.html

PHP:  array_reverse($arr);
来源：http://hz.jinqigfzy.top/gtjrrkjewo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.guowangkeji.top/gtcbufmabn.html

TS:   [...arr].reverse();
来源：http://hz.hysaishi.cn/gtthgrjkji.html

Java: Collections.reverse(list);
来源：http://hz.jqgfzy.top/gtprqjuigb.html

Go:   slices.Reverse(arr)
来源：http://hz.chenjidiqi.icu/gtjmssajbv.html

Ruby: arr.reverse
来源：http://hz.hammf.cn/gtnumuixwu.html

C#:   list.Reverse();
来源：http://hz.daria6918.cn/gtzfeuawue.html

[D12] 查找元素下标
来源：http://hz.pycfn.com/gtnzqtrroe.html

Py:   arr.index(x);  x in arr
来源：http://hz.meibo888.top/gtdyrtwlgs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.chenjidiqi.icu/gtwjolnupn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tanke756.top/gtuthjvuli.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuanzhike.top/gtjrorblrs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hywenlv.cn/gthfiiekal.html

Go:   slices.Index(arr, x)
来源：http://hz.nanxinkj.top/gtnzmtdxyz.html

Ruby: arr.index(x)
来源：http://hz.zycfv.cn/gtemqqbmgq.html

C#:   list.IndexOf(x);
来源：http://hz.jinyuanbaomall.cn/gthtximnyv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jianghu66.top/gtakptozvk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.meibo888.top/gteybvjjtr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.wangdashe.top/gthoddgqsx.html

JS:   arr.filter(x => x > 3)
来源：http://hz.fzhhl.top/gtwfvrioel.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shzxlz.cn/gtgqvbvowb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jianghu66.top/gtocidgirn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hysaishi.cn/gtqebzejsr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zdqjudy.top/gtsotltbix.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xuanzx.com/gtvmcubzyu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.feifeiyinyue.top/gtaxupjgkz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jyoumei.cn/gtjsoqgwwv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.chenzaomai.com/gtnubobsnx.html

JS:   arr.map(x => x * 2)
来源：http://hz.zdqjudy.top/gtbidifvfg.html

TS:   arr.map(x => x * 2)
来源：http://hz.cucudq.cn/gtdhvsuuar.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.0kj1m.cn/gtjvhsohbo.html

Go:   // 手写循环
来源：http://hz.pycfn.com/gtzbxapaxi.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jinqigfzy.top/gtkoodijqn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shangyingyoupin.top/gtcwmvnbje.html

[D15] 去重
来源：http://hz.hongshengwenyu.top/gtqbzufonb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.daria6918.cn/gttkstiegj.html

PHP:  array_unique($arr);
来源：http://hz.svipenyu.cn/gtctpnvpth.html

JS:   [...new Set(arr)]
来源：http://hz.iojbl.cn/gtyantisly.html

TS:   [...new Set(arr)]
来源：http://hz.tanke756.top/gtocrtusfj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ydjk.org.cn/gtrewhyfmi.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jinyuanbaomall.cn/gtggehxfpl.html

Ruby: arr.uniq
来源：http://hz.yuxming.cn/gtivndjxbx.html

C#:   list.Distinct().ToList()
来源：http://hz.yongpay.top/gtidwhsosn.html

[D16] 求和与平均值
来源：http://hz.shanyushiyangkeji.top/gtkhjloifr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.svipenyu.cn/gtulvnouwv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yuanzhike.top/gtqbwinolz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daxiang520.top/gtmobzvfce.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yongpay.top/gtuefdovrw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yvedp.cn/gtikoxbjad.html

Go:   // 手写循环累加
来源：http://hz.ydzc1.top/gtrbeqcsrm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.mhx1999.top/gtgbbdrqbb.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhengqikj.top/gtlzeewhad.html

[D17] 最大值与最小值
来源：http://hz.mhx1999.top/gteffvxjkk.html

Py:   max(arr);  min(arr)
来源：http://hz.daria6918.cn/gtbircpkuf.html

PHP:  max($arr);  min($arr);
来源：http://hz.vqdsnc.cn/gtpnyhnmmu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.aizwys.cn/gtbgaljlha.html

TS:   Math.max(...arr);
来源：http://hz.chenzaomai.com/gtsfjwhboh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xziqi.cn/gtbogyeklb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hammf.cn/gtoveckkir.html

Ruby: arr.max;  arr.min
来源：http://hz.xziqi.cn/gtmbqixuho.html

C#:   list.Max();  list.Min()
来源：http://hz.jqgufenzy.top/gtlkzvtynv.html

[D18] 扁平化嵌套数组
来源：http://hz.c1oappe.top/gtawroytgm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nwbrower.top/gtygjvztvr.html

PHP:  array_merge(...$nested);
来源：http://hz.zhongyouzk.top/gtvqtikomj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yuxming.cn/gtpphdxbwl.html

TS:   nested.flat();
来源：http://hz.nanxuanxn.top/gtoshaeqhv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.nanxinkj.top/gtdisjxkig.html

Go:   // 手写双层循环
来源：http://hz.snrcjt.cn/gtpiuxyptf.html

Ruby: nested.flatten
来源：http://hz.shuidangran.top/gtfwffkili.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.pycfn.com/gttqcjtqnc.html

[D19] 按字段分组
来源：http://hz.hywenlv.cn/gtjlftvccx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hongshengwenyu.top/gtyjtcdeat.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shanyushiyangtech.top/gtyaergxuc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.0kj1m.cn/gtepsvlwzc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.guannengcc.top/gtqlueqtos.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.fzhhl.top/gtdpeooyqx.html

Go:   // 手写 map[string][]T
来源：http://hz.hnqzz.top/gthloxwvau.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.wangdashe.top/gtjbczxafq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.sufxvd.cn/gtdzbpxube.html

[D20] 统计每个元素出现次数
来源：http://hz.vqdsnc.cn/gtgxpnqutn.html

Py:   Counter(arr)
来源：http://hz.aibaodan.cn/gtonfjtoea.html

PHP:  array_count_values($arr);
来源：http://hz.shuidangran.top/gthhuvdrgj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangtech.top/gtnjcyedkf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinghuilouyu.cn/gtqwoqmalf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jiagoushi.top/gthyokpdse.html

Go:   // 手写 map[T]int
来源：http://hz.wangdashe.top/gtykuazewf.html

Ruby: arr.tally
来源：http://hz.nanxinkj.top/gtfvtisxhb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hnqzz.top/gtyacelapl.html

[D21] 判断是否包含某元素
来源：http://hz.cdnleiting.top/gtuouaukby.html

Py:   x in arr
来源：http://hz.chenjidiqi.icu/gtjhyqspnx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jyoumei.cn/gtuxwidwet.html

JS:   arr.includes(x)
来源：http://hz.fengsongda.top/gtpxzrrjur.html

TS:   arr.includes(x)
来源：http://hz.9152youxi.cn/gtmthfqypa.html

Java: list.contains(x)
来源：http://hz.aizwys.cn/gtduvsaghp.html

Go:   slices.Contains(arr, x)
来源：http://hz.yuanzhike.top/gtkvbhbthf.html

Ruby: arr.include?(x)
来源：http://hz.zhengqikj.top/gtxkzvhpqu.html

C#:   list.Contains(x)
来源：http://hz.vqdsnc.cn/gtuddhrchu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hfpthk.cn/gtxxfylcll.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.guowangkeji.top/gthpbnjzhf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhongyouzk.top/gtivtfkvba.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.vqdsnc.cn/gtwstwfsrs.html

TS:   [...arr];
来源：http://hz.kuanghao11.cn/gtjhfahldd.html

Java: new ArrayList<>(list);
来源：http://hz.jyoumei.cn/gtajumlbvc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shangyingyoupin.top/gtaxtgzocd.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ehwqpu.com/gtcwujcnlv.html

C#:   new List<int>(list);
来源：http://hz.cucudq.cn/gtalvyvcov.html

[D23] reduce 累积计算
来源：http://hz.ybcxt.top/gtuilwxpbi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhoulong.xyz/gtfjduagdb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhaomingkeji.xyz/gtaotqdgdm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jlsjyb.cn/gtjapfyiun.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zycfv.cn/gttydsupgs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhiwuduotai.top/gtnigblhjb.html

Go:   // 手写循环
来源：http://hz.cashguo.top/gtdzeufmgk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.gotoacloud.top/gtqaawrdbd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ybcxt.top/gtjtswawgw.html

[D24] 字典 / Map 基本操作
来源：http://hz.fengsongda.top/gtipsactyw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hammf.cn/gtlheygvas.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cqqwz.cn/gtolyjflmm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.iojbl.cn/gtyjgghvme.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.haohaochexian.top/gtucmwwalk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jiagoushi.top/gttnfbnymu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yj20258888.top/gtvsruvmqq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.tianlin.xyz/gttgwjptec.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinghuilouyu.cn/gtyxmxgjwa.html

[D25] Set 集合去重与交并差
来源：http://hz.shangyingyoupin.top/gtmeinnoqk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shanyushiyangtech.top/gtzogxysng.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.chenzaomai.com/gtfbzpnamc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.pengpengdd.cyou/gteqmpeazb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.tanke756.top/gttasfnamc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sxryk.cn/gtvfibuvwj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shzxlz.cn/gtrdzbgrca.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.pycfn.com/gtwghxcvpz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.pycfn.com/gtjvswwsaj.html

[D26] 数组转字符串
来源：http://hz.xylfe.cn/gtzwqwmvho.html

Py:   ", ".join(map(str, arr))
来源：http://hz.dashuyun.cn/gtjuolyrgu.html

PHP:  implode(", ", $arr);
来源：http://hz.0kj1m.cn/gtgrmtgwmn.html

JS:   arr.join(", ")
来源：http://hz.smart0.xyz/gtmfojbotw.html

TS:   arr.join(", ")
来源：http://hz.chenjidiqi.icu/gtxmpwyzna.html

Java: String.join(", ", list)
来源：http://hz.shanyushiyangkeji.top/gtkhghqxba.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yvedp.cn/gtnskvzdsc.html

Ruby: arr.join(", ")
来源：http://hz.jinqigfzy.top/gtoycbbism.html

C#:   string.Join(", ", list)
来源：http://hz.xingfuxueyuan.xyz/gtveqnwopk.html

================================================================================
来源：http://hz.fengsongda.top/gtqazuctct.html

E. 字符串处理
来源：http://hz.snrcjt.cn/gtalhntabt.html

================================================================================
来源：http://hz.yonumen.top/gtftwtecqw.html

[E01] 拼接字符串
来源：http://hz.xingfuxueyuan.xyz/gtngcpcite.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.mhx1999.top/gtfedhrxxa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cqqwz.cn/gtjjnjxkxb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenlongwang.top/gtdledezkv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xziqi.cn/gtrgyadhvt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.snrcjt.cn/gtgqijplwo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yongpay.top/gtrwxzjwbc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhoulong.xyz/gtgebbunes.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.dianchejie.cn/gtmyjxqkau.html

[E02] 重复字符串
来源：http://hz.cucudq.cn/gtyjmkjnlf.html

Py:   "ab" * 3
来源：http://hz.jianghu66.top/gtcxpzfpnv.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ybcxt.top/gtdaesidhh.html

JS:   "ab".repeat(3)
来源：http://hz.ydjk.org.cn/gtvemxeekk.html

TS:   "ab".repeat(3)
来源：http://hz.jinqigufen.top/gtbnsotzhv.html

Java: "ab".repeat(3)
来源：http://hz.hammf.cn/gthatmghzk.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.gogol.net.cn/gtyacmyzgj.html

Ruby: "ab" * 3
来源：http://hz.andypj.xyz/gtqlwiuogw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nanxuanxn.top/gtkkwdsbqp.html

[E03] 截取子串
来源：http://hz.nwbrower.top/gttliijrrz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hnqzz.top/gtxemdvezp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gogol.net.cn/gtzsjweyle.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sxryk.cn/gtlyuypzzx.html

TS:   s.slice(1, 4)
来源：http://hz.chenlongwang.top/gtcvapznse.html

Java: s.substring(1, 4)
来源：http://hz.wangdashe.top/gtafuauiod.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.fengsongda.top/gtmsctdksq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinqigfzy.top/gtdcuczokr.html

C#:   s.Substring(1, 3)
来源：http://hz.316326.xyz/gtaynwcifs.html

[E04] 查找子串位置
来源：http://hz.gaohongyu789.top/gtzlugjrmw.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xingfuxueyuan.xyz/gtjlsmshik.html

PHP:  strpos($s, "x");
来源：http://hz.sweek.top/gtmtmseoxt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.tianlin.xyz/gthmslmlht.html

TS:   s.indexOf("x")
来源：http://hz.shangyingyoupin.top/gtwgxeyrfp.html

Java: s.indexOf("x")
来源：http://hz.xylfe.cn/gtapisgcfc.html


<!-- 参考信息 -->