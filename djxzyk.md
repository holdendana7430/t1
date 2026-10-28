代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://hz.shanyushiyangkeji.top/gtihdmaeyf.html

Ruby: -> { puts "run" }.call
来源：http://hz.aizwys.cn/gtrkfzteyd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ywan-chungtsiang.top/gtblgjxlss.html

[C13] 类型声明 / 类型注解
来源：http://hz.fzhhl.top/gtxvcpekfa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.havefunace.top/gtbmhqhdao.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xziqi.cn/gtuhqalpai.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.pycfn.com/gtaylndkjk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.daria6918.cn/gtjacgwlgm.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zdqjudy.top/gtwyqzwgyl.html

Go:   func add(a, b int) int
来源：http://hz.hongshengwenyu.top/gtcepamhxv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hnxiangtu.top/gtndgcichh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ivvv.top/gttxvtxwvz.html

[C14] 泛型函数
来源：http://hz.yj202588.top/gtpmoeiqsh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.chenlongwang.top/gtbhspmvbv.html

PHP:  // 无泛型
来源：http://hz.zhongyouzk.top/gtyaipzmxu.html

JS:   // 无泛型
来源：http://hz.sysykeji.top/gtmotrbwxe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xylfe.cn/gtohvzzldz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.kuanghao11.cn/gtzljvfukp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.tanke756.top/gthauzmfkl.html

Ruby: # 无泛型
来源：http://hz.redwolf501.top/gtdvtnxobc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.fengsongda.top/gtinuqzvjr.html

[C15] 解构 / 展开参数
来源：http://hz.guannengcc.top/gtpnwwuvyb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.iojbl.cn/gtaxslxkcm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.pengpengdd.cyou/gthopqqqqw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jiagoushi.top/gtmpkbfzuq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.bjfxy.top/gttlpzsipz.html

Java: // 无解构
来源：http://hz.ydzc1.top/gtlkokdwck.html

Go:   // 无解构
来源：http://hz.chenjidiqi.icu/gtssrkznvj.html

Ruby: a, b = pair
来源：http://hz.zhaomingkeji.xyz/gtdkelxcod.html

C#:   var (a, b) = pair;
来源：http://hz.xylfe.cn/gtytpvzkvi.html

[C16] 函数 / 方法重载
来源：http://hz.sweek.top/gtlmcurydr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.iojbl.cn/gtjidgupwr.html

PHP:  // 无重载
来源：http://hz.ywan-chungtsiang.top/gtbsvzmkeu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hywenlv.cn/gtphjkvyvr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinqigfzy.top/gtufpesjih.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ppjwa.cn/gtiiluzzfx.html

Go:   // 无重载：用不同函数名
来源：http://hz.pycfn.com/gthtwfpqzn.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shanyushiyangtech.top/gtwzalkxpp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hnqzz.top/gtgfrylwfm.html

================================================================================
来源：http://hz.yangfankeji.com/gtccmcedsh.html

D. 数组 / 列表 / 集合
来源：http://hz.pengpengdd.cyou/gtqllresfe.html

================================================================================
来源：http://hz.zhoulong.xyz/gtohtdnxqh.html

[D01] 创建数组 / 列表
来源：http://hz.yj202588.top/gtibfaygkb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yonumen.top/gtfntajnmr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.andypj.xyz/gtczikysgj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.daxiang520.top/gtcbbbokng.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.52xcode.cn/gthvnxibph.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yj20258888.top/gtfmqcohnz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yvedp.cn/gtcwttojnc.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhiwuduotai.top/gtqdvywnzw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ivvv.top/gtrbxeygxb.html

[D02] 追加元素到末尾
来源：http://hz.zhiwuduotai.top/gthdhraaoa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shzxlz.cn/gttavdqxax.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hfpthk.cn/gtxzttdsbi.html

JS:   arr.push(4);
来源：http://hz.hnqzz.top/gtkhhzovmf.html

TS:   arr.push(4);
来源：http://hz.haohaochexian.top/gtzblewbvh.html

Java: list.add(4);
来源：http://hz.smart0.xyz/gtxwwsvuym.html

Go:   arr = append(arr, 4)
来源：http://hz.daria6918.cn/gtymmucyrf.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xuetiantiany.cn/gtavsmxutv.html

C#:   list.Add(4);
来源：http://hz.yangfankeji.com/gtrfimblhl.html

[D03] 在指定位置插入元素
来源：http://hz.xziqi.cn/gtdypgcrym.html

Py:   arr.insert(0, 0)
来源：http://hz.guannengcc.top/gteukjjpqs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.fengsongda.top/gtruvnuqdp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.9152youxi.cn/gtcpxzfhyh.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.meibo888.top/gtuzlckdsx.html

Java: list.add(0, 0);
来源：http://hz.gaohongyu789.top/gtzvbepvos.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.0kj1m.cn/gtdkpktxka.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhijiandao.cn/gtjznrqrmy.html

C#:   list.Insert(0, 0);
来源：http://hz.xziqi.cn/gtvytjjbyw.html

[D04] 删除元素
来源：http://hz.svipenyu.cn/gtybajhszj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.aizwys.cn/gtzxjwwdxa.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.fzhhl.top/gtbowatwsy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hysaishi.cn/gtajwsumaq.html

TS:   arr.splice(0, 1);
来源：http://hz.gotoacloud.top/gtsmkjyfsn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ehwqpu.com/gttwnxndda.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yongpay.top/gtkjxgssws.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.snrcjt.cn/gtsuuywgga.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.gaohongyu789.top/gtlcxqadgv.html

[D05] 访问与修改元素
来源：http://hz.zhijiandao.cn/gtqgvhtpji.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sxryk.cn/gtyvklcenc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.wangdashe.top/gtyxeatjdr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.chenlongwang.top/gtyvjieyqp.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shanyushiyangkeji.top/gtxhkhcvjz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yj20258888.top/gtaozwymop.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.wangdashe.top/gtllddophz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangshuangyany.cn/gtxkzkohmn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.gogol.net.cn/gtdpbhooxp.html

[D06] 数组长度
来源：http://hz.ydjk.org.cn/gtnwpdwcza.html

Py:   len(arr)
来源：http://hz.jyoumei.cn/gtltisyigf.html

PHP:  count($arr);
来源：http://hz.havefunace.top/gtryutkylh.html

JS:   arr.length
来源：http://hz.zhiwuduotai.top/gthhwvisse.html

TS:   arr.length
来源：http://hz.zdqjudy.top/gtykapxvqz.html

Java: list.size();
来源：http://hz.zhengqikj.top/gtuerblhks.html

Go:   len(arr)
来源：http://hz.316326.xyz/gtpfhpozhd.html

Ruby: arr.length; arr.size
来源：http://hz.shanyushiyangtech.top/gtwxosupte.html

C#:   list.Count;
来源：http://hz.feifeiyinyue.top/gtgsefcsjl.html

[D07] 切片 / 取子数组
来源：http://hz.feifeiyinyue.top/gttpfgvaio.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinqigfzy.top/gttyxejzxo.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xylfe.cn/gtapagknry.html

JS:   arr.slice(1, 4);
来源：http://hz.yongpay.top/gtcyqvqdbu.html

TS:   arr.slice(1, 4);
来源：http://hz.jqgufenzy.top/gtpqwmesrk.html

Java: list.subList(1, 4);
来源：http://hz.zhengqikj.top/gtiqtiaehr.html

Go:   arr[1:4]
来源：http://hz.quarkkingdee.top/gteheacpmt.html

Ruby: arr[1, 3]
来源：http://hz.aizwys.cn/gthsbhmbyi.html

C#:   list.GetRange(1, 3);
来源：http://hz.tanke756.top/gtfhwryhgj.html

[D08] 合并两个数组
来源：http://hz.9152youxi.cn/gtnqmhjmjv.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhixingplan.top/gtwbfonfud.html

PHP:  array_merge($a, $b);
来源：http://hz.nanxuanxn.top/gtncqfrvll.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hfpthk.cn/gtzowntgst.html

TS:   [...a, ...b];
来源：http://hz.kuanghao11.cn/gtqibueacr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhixingplan.top/gthaeauxon.html

Go:   append(a, b...)
来源：http://hz.c1oappe.top/gtqtdtprks.html

Ruby: a + b;  a.concat(b)
来源：http://hz.gotoacloud.top/gtallatkan.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinqigfzy.top/gtfubnfxim.html

[D09] 排序（升序）
来源：http://hz.yangfankeji.com/gtxdpmhsvs.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sweek.top/gtavauavkw.html

PHP:  sort($arr);
来源：http://hz.cdnleiting.top/gtlbkzhljn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hammf.cn/gtfvuvafup.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.gaohongyu789.top/gtemjzcvbv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.wangdashe.top/gtrqbhtplw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.tanke756.top/gtldtzkhaz.html

Ruby: arr.sort
来源：http://hz.ybcxt.top/gtvtlbekfd.html

C#:   list.Sort();
来源：http://hz.shzxlz.cn/gtegmillhp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ywan-chungtsiang.top/gtzvzuzvji.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ydzc1.top/gtedezhzeq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jiagoushi.top/gtmftexqok.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.pycfn.com/gtzefrtzzq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ydzc1.top/gtffyfqmkn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yonumen.top/gtdltlghrm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.sxryk.cn/gtxqhueams.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.andypj.xyz/gthunxbubn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.havefunace.top/gtocwarvlt.html

[D11] 反转数组
来源：http://hz.aibaodan.cn/gtnfxhuivt.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cdnleiting.top/gthixvkkfn.html

PHP:  array_reverse($arr);
来源：http://hz.zhongyouzk.top/gtnanmzumc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinqigufen.top/gtlranebbi.html

TS:   [...arr].reverse();
来源：http://hz.sufxvd.cn/gtzusvwgwc.html

Java: Collections.reverse(list);
来源：http://hz.zhongyouzk.top/gtwnksardf.html

Go:   slices.Reverse(arr)
来源：http://hz.hnqzz.top/gtsjvlzivz.html

Ruby: arr.reverse
来源：http://hz.zhoulong.xyz/gtohzstdpx.html

C#:   list.Reverse();
来源：http://hz.316326.xyz/gtsuyntaak.html

[D12] 查找元素下标
来源：http://hz.pengpengdd.cyou/gtdbxbzcwn.html

Py:   arr.index(x);  x in arr
来源：http://hz.shanyushiyangkeji.top/gtzdsasqfw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.sysykeji.top/gtqzbaajcs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.meibo888.top/gtaylxinez.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.bjfxy.top/gtlvixknif.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhengqikj.top/gtxuulwiqt.html

Go:   slices.Index(arr, x)
来源：http://hz.sysykeji.top/gthbslmjxt.html

Ruby: arr.index(x)
来源：http://hz.sysykeji.top/gtmlflqlrc.html

C#:   list.IndexOf(x);
来源：http://hz.0kj1m.cn/gtqkihcxqu.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hfpthk.cn/gtbtsxlxpc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hongshengwenyu.top/gtljkgflmr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhaomingkeji.xyz/gtpjflgqgt.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jinqigufen.top/gtuknggsmp.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhengqikj.top/gtxtlafmjh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.tian-w.cn/gtetebfxit.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yangfankeji.com/gtopjnwznz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ybcxt.top/gtnksdcnwl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.chenlongwang.top/gtjqtrahid.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ehwqpu.com/gtkamjzmvi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sysykeji.top/gtbuqwhkkg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ybcxt.top/gtlrsirdru.html

JS:   arr.map(x => x * 2)
来源：http://hz.9152youxi.cn/gtkmiwmito.html

TS:   arr.map(x => x * 2)
来源：http://hz.gogol.net.cn/gtsfyjrrbx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.guannengcc.top/gtsbplmjpo.html

Go:   // 手写循环
来源：http://hz.daxiang520.top/gtiktcjiuu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.andypj.xyz/gtpqrdyqiw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hysaishi.cn/gttpgdgvfu.html

[D15] 去重
来源：http://hz.c1oappe.top/gtpvqyejgz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.guowangkeji.top/gtipknhhxn.html

PHP:  array_unique($arr);
来源：http://hz.xingfuxueyuan.xyz/gtziozeuwy.html

JS:   [...new Set(arr)]
来源：http://hz.andypj.xyz/gtdecbehqa.html

TS:   [...new Set(arr)]
来源：http://hz.jinghuilouyu.cn/gtlietxezj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhiwuduotai.top/gtrgcixopk.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.guowangkeji.top/gtohipzzah.html

Ruby: arr.uniq
来源：http://hz.sweek.top/gtotrjzhgp.html

C#:   list.Distinct().ToList()
来源：http://hz.dianchejie.cn/gtmywsaaqr.html

[D16] 求和与平均值
来源：http://hz.xingfuxueyuan.xyz/gtftkjbsnf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hongshengwenyu.top/gtflvfsxwy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jianghu66.top/gtuszujkbe.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258888.top/gtfrnzfzys.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258.top/gtsonsxxvg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.vqdsnc.cn/gtoobxasew.html

Go:   // 手写循环累加
来源：http://hz.zhixingplan.top/gtvlfksekm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.svipenyu.cn/gtdwepqygz.html

C#:   list.Sum();  list.Average()
来源：http://hz.shuidangran.top/gtravfrcqk.html

[D17] 最大值与最小值
来源：http://hz.shanyushiyangtech.top/gtnqssphuv.html

Py:   max(arr);  min(arr)
来源：http://hz.yj202588.top/gtlmtxmecw.html

PHP:  max($arr);  min($arr);
来源：http://hz.zdqjudy.top/gtyssjpbdo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.birdmap.top/gtoyzhywbr.html

TS:   Math.max(...arr);
来源：http://hz.zhongyouzk.top/gtplsckroz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zycfv.cn/gtcmlyedql.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ywan-chungtsiang.top/gtxhvbguix.html

Ruby: arr.max;  arr.min
来源：http://hz.316326.xyz/gttwfbilwf.html

C#:   list.Max();  list.Min()
来源：http://hz.sxryk.cn/gtmhzyfdvg.html

[D18] 扁平化嵌套数组
来源：http://hz.jyoumei.cn/gtouhduabt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shanyushiyangtech.top/gtamwxodwx.html

PHP:  array_merge(...$nested);
来源：http://hz.tanke756.top/gtzhhfgajt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.gzhubu.top/gtjulyspxi.html

TS:   nested.flat();
来源：http://hz.yueranfly.top/gtsxwobnrs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gaohongyu789.top/gtypmrekat.html

Go:   // 手写双层循环
来源：http://hz.hnqzz.top/gttisjpsvu.html

Ruby: nested.flatten
来源：http://hz.cdnleiting.top/gtkocsyzat.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hammf.cn/gtcqituivv.html

[D19] 按字段分组
来源：http://hz.birdmap.top/gttvyqntid.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhijiandao.cn/gtoyjtjxkp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hongshengwenyu.top/gtkgdjphxk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yj20258888.top/gtnibhsmwg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.daria6918.cn/gttmqkmcgo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yj20258888.top/gtdnubqkbx.html

Go:   // 手写 map[string][]T
来源：http://hz.pycfn.com/gtggraqlfy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xziqi.cn/gtzkcsquxt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.havefunace.top/gtcohqazgc.html

[D20] 统计每个元素出现次数
来源：http://hz.chenjidiqi.icu/gtbgcaezel.html

Py:   Counter(arr)
来源：http://hz.xziqi.cn/gtkobkxlrp.html

PHP:  array_count_values($arr);
来源：http://hz.cashguo.top/gtugyyvesi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.guannengcc.top/gtoklwofov.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.52xcode.cn/gtgnueinos.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yuxming.cn/gtngqhxsao.html

Go:   // 手写 map[T]int
来源：http://hz.hongshengwenyu.top/gtvylkclrb.html

Ruby: arr.tally
来源：http://hz.sufxvd.cn/gtfvlmcvdu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.guannengcc.top/gtznmsvjfo.html

[D21] 判断是否包含某元素
来源：http://hz.shzxlz.cn/gtuaopcgdt.html

Py:   x in arr
来源：http://hz.daxiang520.top/gtaptfmoeq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gogol.net.cn/gtcglzkuqu.html

JS:   arr.includes(x)
来源：http://hz.svipenyu.cn/gtcojqrccd.html

TS:   arr.includes(x)
来源：http://hz.52xcode.cn/gtwsxlzxal.html

Java: list.contains(x)
来源：http://hz.haohaochexian.top/gtwkqmaikz.html

Go:   slices.Contains(arr, x)
来源：http://hz.hongshengwenyu.top/gtjvqxnjso.html

Ruby: arr.include?(x)
来源：http://hz.yonumen.top/gtxinalwpg.html

C#:   list.Contains(x)
来源：http://hz.hnqzz.top/gtqliktltx.html

[D22] 复制数组（避免共享引用）
来源：http://hz.daria6918.cn/gtsrbjjome.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.kuanghao11.cn/gtjlnirtto.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ppjwa.cn/gtxzaqdnjz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jqgfzy.top/gtrksbwzoo.html

TS:   [...arr];
来源：http://hz.meibo888.top/gtgmspvbin.html

Java: new ArrayList<>(list);
来源：http://hz.jinyuanbaomall.cn/gtbweaqeaf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.0kj1m.cn/gtplfbgsdy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhoulong.xyz/gtnaprggsh.html

C#:   new List<int>(list);
来源：http://hz.xziqi.cn/gtpoutjrut.html

[D23] reduce 累积计算
来源：http://hz.xylfe.cn/gtbfyofjts.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xziqi.cn/gtdmcdrpuj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.shuidangran.top/gtrqtdomcs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhengqikj.top/gttnepnpge.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xinyue.icu/gtxnnpegfv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gogol.net.cn/gtvjrnfmul.html

Go:   // 手写循环
来源：http://hz.gzhubu.top/gtomtfiorl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.meibo888.top/gtmiuvbdcy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenjidiqi.icu/gtpqoeucub.html

[D24] 字典 / Map 基本操作
来源：http://hz.yuanzhike.top/gtjjwvzgwi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ivvv.top/gtcirhzcrh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.guowangkeji.top/gthamlofgw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.fzhhl.top/gtwpzowbbr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.vqdsnc.cn/gtxtnxqnig.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hywenlv.cn/gtqosffpso.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.sxryk.cn/gtpbpakrxf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinqigfzy.top/gttlgaysmm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.sufxvd.cn/gtccymehgf.html

[D25] Set 集合去重与交并差
来源：http://hz.ybcxt.top/gtajxjhbyy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.feifeiyinyue.top/gtxbrbeabx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nwbrower.top/gtjexhebbd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cheryme.top/gtwgusguzg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zdqjudy.top/gttolzbtvu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.smart0.xyz/gtvzvterlz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.haohaochexian.top/gtjrujblzq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinqigufen.top/gtizbetoas.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhiwuduotai.top/gtryhgspxm.html

[D26] 数组转字符串
来源：http://hz.sysykeji.top/gtmanizbcg.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cheryme.top/gtckimxgga.html

PHP:  implode(", ", $arr);
来源：http://hz.sweek.top/gtzvwwnekw.html

JS:   arr.join(", ")
来源：http://hz.shanyushiyangkeji.top/gtwluhagff.html

TS:   arr.join(", ")
来源：http://hz.hfpthk.cn/gtxyxkzgem.html

Java: String.join(", ", list)
来源：http://hz.meibo888.top/gtbkfoommq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gzhubu.top/gtkjwrrbmw.html

Ruby: arr.join(", ")
来源：http://hz.jlsjyb.cn/gtasuwnfya.html

C#:   string.Join(", ", list)
来源：http://hz.yonumen.top/gtadaacutm.html

================================================================================
来源：http://hz.yongpay.top/gtsyyiulcg.html

E. 字符串处理
来源：http://hz.hammf.cn/gtblbzuwys.html

================================================================================
来源：http://hz.smart0.xyz/gtusqawngi.html

[E01] 拼接字符串
来源：http://hz.jinqigfzy.top/gtncimknjk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hysaishi.cn/gtmlxtvpdd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xuetiantiany.cn/gtwjauxejr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sweek.top/gtnwrsmvfs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.fzhhl.top/gtbyltwyvm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yanxiufei.cn/gtztovbtab.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhixingplan.top/gtftqspggi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ppjwa.cn/gtzlzswakw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.nwbrower.top/gtweudjsie.html

[E02] 重复字符串
来源：http://hz.nanxuanxn.top/gtoamjydbt.html

Py:   "ab" * 3
来源：http://hz.yj20258.top/gtrzywgvof.html

PHP:  str_repeat("ab", 3);
来源：http://hz.meibo888.top/gtoecjugxz.html

JS:   "ab".repeat(3)
来源：http://hz.aizwys.cn/gtdyqugcut.html

TS:   "ab".repeat(3)
来源：http://hz.chenjidiqi.icu/gtufsqvbns.html

Java: "ab".repeat(3)
来源：http://hz.meibo888.top/gtrgdtnspv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.tanke756.top/gtiysqhfhy.html

Ruby: "ab" * 3
来源：http://hz.shanyushiyangkeji.top/gtluhcfbeh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yongpay.top/gtlcbhnvka.html

[E03] 截取子串
来源：http://hz.yonumen.top/gtoottoago.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sysykeji.top/gtiweqdhuc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.meibo888.top/gtxxvfihzu.html


<!-- 参考信息 -->