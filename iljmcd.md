代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jinqigufen.top/gtsrdojhto.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhaomingkeji.xyz/gthqxhrqzk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cheryme.top/gtwyrasjqu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yonumen.top/gtwvwaerkw.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hnqzz.top/gthojnuyif.html

Go:   func add(a, b int) int
来源：http://hz.hnxiangtu.top/gteydjcxnk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ydzc1.top/gtbuqapxak.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.quarkkingdee.top/gtndefzivf.html

[C14] 泛型函数
来源：http://hz.sufxvd.cn/gtrlnlvtef.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xuanzx.com/gtotfimdxp.html

PHP:  // 无泛型
来源：http://hz.havefunace.top/gtcexiuojp.html

JS:   // 无泛型
来源：http://hz.hysaishi.cn/gtbstqtvxj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cashguo.top/gtlgwftgqp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinyuanbaomall.cn/gtrhqdufla.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jqgfzy.top/gtmxmdmddn.html

Ruby: # 无泛型
来源：http://hz.jinqigfzy.top/gtembbqxfg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.sxryk.cn/gthlgoqxko.html

[C15] 解构 / 展开参数
来源：http://hz.sweek.top/gtmpvhwxrr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhongyouzk.top/gtdxllgyyq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yongpay.top/gtslunyuks.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.aibaodan.cn/gtnfopzszq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.tanke756.top/gtgmkrkfwl.html

Java: // 无解构
来源：http://hz.yueranfly.top/gtmbspmnwj.html

Go:   // 无解构
来源：http://hz.pycfn.com/gtjtbglnfu.html

Ruby: a, b = pair
来源：http://hz.hywenlv.cn/gtatpukcwm.html

C#:   var (a, b) = pair;
来源：http://hz.jinqigufen.top/gtiesysbxs.html

[C16] 函数 / 方法重载
来源：http://hz.jinghuilouyu.cn/gtscyxhnec.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.svipenyu.cn/gtjfpvcaxx.html

PHP:  // 无重载
来源：http://hz.yj20258888.top/gtbfcxclgn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yueranfly.top/gtdeocniue.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.0kj1m.cn/gtgqenzkqp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.vqdsnc.cn/gtpfcgznmf.html

Go:   // 无重载：用不同函数名
来源：http://hz.cheryme.top/gthkffgvoq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sysykeji.top/gtevmkajxr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.daxiang520.top/gtumvljzek.html

================================================================================
来源：http://hz.daxiang520.top/gtckdkqbwq.html

D. 数组 / 列表 / 集合
来源：http://hz.9152youxi.cn/gtsbuwunvt.html

================================================================================
来源：http://hz.mhx1999.top/gttiylnmfk.html

[D01] 创建数组 / 列表
来源：http://hz.ehwqpu.com/gtfvnrmmrh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.havefunace.top/gtfwawpzyg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.mhx1999.top/gtlcnjmkoe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.pycfn.com/gtifvpjofy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hnxiangtu.top/gtshdbzqjf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.chenzaomai.com/gtlctxrogd.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jinghuilouyu.cn/gthoefijod.html

Ruby: arr = [1, 2, 3]
来源：http://hz.sxryk.cn/gtklsjbcmq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.nwbrower.top/gtfejoutry.html

[D02] 追加元素到末尾
来源：http://hz.yuanzhike.top/gtxebqzfea.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhongyouzk.top/gtvazffjwi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.snrcjt.cn/gtdywlkdre.html

JS:   arr.push(4);
来源：http://hz.iojbl.cn/gteeluxncv.html

TS:   arr.push(4);
来源：http://hz.cqqwz.cn/gtewmjyvrw.html

Java: list.add(4);
来源：http://hz.pycfn.com/gtkmyzmvvx.html

Go:   arr = append(arr, 4)
来源：http://hz.pycfn.com/gtzhwboytc.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhongyouzk.top/gtnrgmetuv.html

C#:   list.Add(4);
来源：http://hz.andypj.xyz/gtlwholffl.html

[D03] 在指定位置插入元素
来源：http://hz.yj20258.top/gtypjtrzrv.html

Py:   arr.insert(0, 0)
来源：http://hz.aibaodan.cn/gtzdtjtozf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.guowangkeji.top/gtyngeoiaf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ppjwa.cn/gtrsqjgkgi.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ybcxt.top/gthwadllla.html

Java: list.add(0, 0);
来源：http://hz.jinqigfzy.top/gtpodmzuvk.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yvedp.cn/gtdkqvceyt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.bjfxy.top/gtfsdjiiur.html

C#:   list.Insert(0, 0);
来源：http://hz.zhaomingkeji.xyz/gtkhvicwar.html

[D04] 删除元素
来源：http://hz.jinqigufen.top/gtdrdpucxp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.tianlin.xyz/gtsqyfxcqp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.9152youxi.cn/gtwuteyzka.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jianghu66.top/gtsurfeuat.html

TS:   arr.splice(0, 1);
来源：http://hz.yanxiufei.cn/gtjzccnruw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.kuanghao11.cn/gtqdseamxx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ehwqpu.com/gtvddabgij.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.9152youxi.cn/gtogmbsikz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.quarkkingdee.top/gtpapvsdyx.html

[D05] 访问与修改元素
来源：http://hz.ydjk.org.cn/gtmfityoof.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtkzqgexlq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.bjfxy.top/gtaiphgcnj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shuidangran.top/gthfjfhxzm.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jinyuanbaomall.cn/gtdovqrzyd.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cdnleiting.top/gtnpxfwiwc.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.0kj1m.cn/gtrlbgkhuq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.pengpengdd.cyou/gtwtjgnweb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.tianlin.xyz/gtfgtgmgva.html

[D06] 数组长度
来源：http://hz.cdnleiting.top/gtagwjbldh.html

Py:   len(arr)
来源：http://hz.smart0.xyz/gtpfcdjkzs.html

PHP:  count($arr);
来源：http://hz.fzhhl.top/gttcsafhgn.html

JS:   arr.length
来源：http://hz.tianlin.xyz/gtyymdjdck.html

TS:   arr.length
来源：http://hz.ydjk.org.cn/gtzhladsoe.html

Java: list.size();
来源：http://hz.nanxinkj.top/gthmuqlnlo.html

Go:   len(arr)
来源：http://hz.c1oappe.top/gtzkuobait.html

Ruby: arr.length; arr.size
来源：http://hz.xinyue.icu/gtavvucwtt.html

C#:   list.Count;
来源：http://hz.zhaomingkeji.xyz/gtxmmdjapb.html

[D07] 切片 / 取子数组
来源：http://hz.52xcode.cn/gtopbhpomv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hysaishi.cn/gtvceizbym.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jinyuanbaomall.cn/gtiegsmsvz.html

JS:   arr.slice(1, 4);
来源：http://hz.hfpthk.cn/gtmzpecyzj.html

TS:   arr.slice(1, 4);
来源：http://hz.hywenlv.cn/gtkdlfnfwy.html

Java: list.subList(1, 4);
来源：http://hz.tanke756.top/gtbiyjefvw.html

Go:   arr[1:4]
来源：http://hz.chenjidiqi.icu/gtgzvxwpcs.html

Ruby: arr[1, 3]
来源：http://hz.wangshuangyany.cn/gtusvdfrki.html

C#:   list.GetRange(1, 3);
来源：http://hz.yonumen.top/gttzazmgcc.html

[D08] 合并两个数组
来源：http://hz.jlsjyb.cn/gtlosstxxy.html

Py:   a + b;  a.extend(b)
来源：http://hz.smart0.xyz/gtzqsvybki.html

PHP:  array_merge($a, $b);
来源：http://hz.zhoulong.xyz/gtzbfrddpq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.pycfn.com/gtxgcuysip.html

TS:   [...a, ...b];
来源：http://hz.jinyuanbaomall.cn/gtmxnnbjec.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.dianchejie.cn/gtwmywqbes.html

Go:   append(a, b...)
来源：http://hz.yanxiufei.cn/gtlayegjjd.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jlsjyb.cn/gtopxsdczx.html

C#:   a.Concat(b).ToList()
来源：http://hz.svipenyu.cn/gtmpoejxsz.html

[D09] 排序（升序）
来源：http://hz.0kj1m.cn/gtjtectgjv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yongpay.top/gtpdmvinku.html

PHP:  sort($arr);
来源：http://hz.sxryk.cn/gtgasstbsa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhixingplan.top/gttfdvlyxr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.0kj1m.cn/gtiwolbrpj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jinqigfzy.top/gtyggtsehf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gotoacloud.top/gtxzbgkiul.html

Ruby: arr.sort
来源：http://hz.vqdsnc.cn/gtrxcxrnlj.html

C#:   list.Sort();
来源：http://hz.ybcxt.top/gtxeswwrvh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.nanxuanxn.top/gtszdtrtzh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.birdmap.top/gturzhimqo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj202588.top/gtvzgkoopo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.guannengcc.top/gtnjrkmcal.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shuidangran.top/gtmdokqwnw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.svipenyu.cn/gtozbhyscn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.vqdsnc.cn/gtpydmfxlg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hnxiangtu.top/gtivkkjsgb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.smart0.xyz/gtsjcizkes.html

[D11] 反转数组
来源：http://hz.zhixingplan.top/gtvmajpoqk.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yj20258.top/gtyqpdubvl.html

PHP:  array_reverse($arr);
来源：http://hz.svipenyu.cn/gtpplznnzf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shangyingyoupin.top/gtwkmbxttg.html

TS:   [...arr].reverse();
来源：http://hz.nanxuanxn.top/gtztgdpapu.html

Java: Collections.reverse(list);
来源：http://hz.yangfankeji.com/gtomkqctdc.html

Go:   slices.Reverse(arr)
来源：http://hz.tanke756.top/gtnrsnbgmh.html

Ruby: arr.reverse
来源：http://hz.haohaochexian.top/gtyqrggkug.html

C#:   list.Reverse();
来源：http://hz.yvedp.cn/gtbqwtpqus.html

[D12] 查找元素下标
来源：http://hz.yongpay.top/gtzcbnwgxg.html

Py:   arr.index(x);  x in arr
来源：http://hz.sxryk.cn/gtphebyibz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.kuanghao11.cn/gtjpvvxfdg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhixingplan.top/gtvjqaawll.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sxryk.cn/gtunaqhqkp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xuanzx.com/gtzcftqkkn.html

Go:   slices.Index(arr, x)
来源：http://hz.hammf.cn/gtfpjztzqi.html

Ruby: arr.index(x)
来源：http://hz.jinyuanbaomall.cn/gtbepnsmkm.html

C#:   list.IndexOf(x);
来源：http://hz.yongpay.top/gtkhbvjybv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhengqikj.top/gtdkidhevn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hywenlv.cn/gtmkdvufgz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jiagoushi.top/gtygeafoyf.html

JS:   arr.filter(x => x > 3)
来源：http://hz.vqdsnc.cn/gthvckpbgn.html

TS:   arr.filter(x => x > 3)
来源：http://hz.sxryk.cn/gtvsgimkzy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jyoumei.cn/gtfnjnovzf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hnqzz.top/gtgulnkupy.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shanyushiyangtech.top/gtsrrepvhu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ydzc1.top/gtbmefpxjj.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hammf.cn/gtlqycvelw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.fengsongda.top/gtilldfqgn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xuetiantiany.cn/gtjplbjieu.html

JS:   arr.map(x => x * 2)
来源：http://hz.ehwqpu.com/gtqqwvrddd.html

TS:   arr.map(x => x * 2)
来源：http://hz.daria6918.cn/gtekmyptqz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.aizwys.cn/gthfvtepbj.html

Go:   // 手写循环
来源：http://hz.yonumen.top/gtwjaqoqpy.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.havefunace.top/gtehnvllwp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhiwuduotai.top/gtfnmprojs.html

[D15] 去重
来源：http://hz.jqgfzy.top/gtucrrbsyh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xinyue.icu/gtkaluxhnf.html

PHP:  array_unique($arr);
来源：http://hz.xuetiantiany.cn/gtojhziigy.html

JS:   [...new Set(arr)]
来源：http://hz.zhixingplan.top/gtcjbcqmql.html

TS:   [...new Set(arr)]
来源：http://hz.0kj1m.cn/gtekjliunl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.svipenyu.cn/gtneyfakuu.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xziqi.cn/gtmeybvuuk.html

Ruby: arr.uniq
来源：http://hz.mhx1999.top/gtmgzgwnne.html

C#:   list.Distinct().ToList()
来源：http://hz.jqgufenzy.top/gtblrakwji.html

[D16] 求和与平均值
来源：http://hz.hongshengwenyu.top/gthybqhrzk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.chenjidiqi.icu/gtlgfjyydj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jqgufenzy.top/gtichkagtd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yanxiufei.cn/gthzyxehpm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shanyushiyangtech.top/gtufxxknva.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yj20258.top/gtaxqfdxbi.html

Go:   // 手写循环累加
来源：http://hz.guowangkeji.top/gtalbohvlg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.aibaodan.cn/gtpwqhpfdl.html

C#:   list.Sum();  list.Average()
来源：http://hz.chenlongwang.top/gtbbasgrkv.html

[D17] 最大值与最小值
来源：http://hz.ydjk.org.cn/gtknibveha.html

Py:   max(arr);  min(arr)
来源：http://hz.52xcode.cn/gtkkwmlyka.html

PHP:  max($arr);  min($arr);
来源：http://hz.pycfn.com/gtgjvvmgpr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.0kj1m.cn/gtafaarnoo.html

TS:   Math.max(...arr);
来源：http://hz.hysaishi.cn/gtxrdadrsc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gaohongyu789.top/gtgfjyjgyc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jinghuilouyu.cn/gtmpymamzz.html

Ruby: arr.max;  arr.min
来源：http://hz.feifeiyinyue.top/gtmuvduamn.html

C#:   list.Max();  list.Min()
来源：http://hz.zycfv.cn/gthzotwmen.html

[D18] 扁平化嵌套数组
来源：http://hz.havefunace.top/gtdgulpima.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hnqzz.top/gtebzoxueo.html

PHP:  array_merge(...$nested);
来源：http://hz.xuetiantiany.cn/gtywjtlgph.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.aibaodan.cn/gtcydujdgp.html

TS:   nested.flat();
来源：http://hz.haohaochexian.top/gtxrkryxkg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shangyingyoupin.top/gttveevpxs.html

Go:   // 手写双层循环
来源：http://hz.daxiang520.top/gthjaprlmi.html

Ruby: nested.flatten
来源：http://hz.pycfn.com/gtnpugwfpm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.haohaochexian.top/gtyhethbpy.html

[D19] 按字段分组
来源：http://hz.birdmap.top/gtcgriapxj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yonumen.top/gthwamsdnz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xuetiantiany.cn/gtteebshsm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jqgufenzy.top/gtghbwpvql.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhaomingkeji.xyz/gthmodtuaj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.guannengcc.top/gtddzsemci.html

Go:   // 手写 map[string][]T
来源：http://hz.yonumen.top/gtbffkolke.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.chenjidiqi.icu/gtjnwccehy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shanyushiyangkeji.top/gtsxnpvdzh.html

[D20] 统计每个元素出现次数
来源：http://hz.chenlongwang.top/gtyndfgvde.html

Py:   Counter(arr)
来源：http://hz.sysykeji.top/gtgebnbgac.html

PHP:  array_count_values($arr);
来源：http://hz.sufxvd.cn/gtnxasiosc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxuanxn.top/gtsxebpgyp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gotoacloud.top/gtpeygwpia.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.chenlongwang.top/gthjslnlio.html

Go:   // 手写 map[T]int
来源：http://hz.xingfuxueyuan.xyz/gtbuydqvhz.html

Ruby: arr.tally
来源：http://hz.yj20258888.top/gtyfdojrfq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ybcxt.top/gtgtlvxhjs.html

[D21] 判断是否包含某元素
来源：http://hz.gaohongyu789.top/gtxjxxqrjf.html

Py:   x in arr
来源：http://hz.shuidangran.top/gtzivqsofs.html

PHP:  in_array($x, $arr, true);
来源：http://hz.wangdashe.top/gtswjtyuke.html

JS:   arr.includes(x)
来源：http://hz.zhongyouzk.top/gtozvqshjj.html

TS:   arr.includes(x)
来源：http://hz.xylfe.cn/gttwekpwly.html

Java: list.contains(x)
来源：http://hz.ppjwa.cn/gthjjtlkag.html

Go:   slices.Contains(arr, x)
来源：http://hz.kuanghao11.cn/gtafrcclde.html

Ruby: arr.include?(x)
来源：http://hz.gzhubu.top/gteykccufg.html

C#:   list.Contains(x)
来源：http://hz.redwolf501.top/gtlwvshiwd.html

[D22] 复制数组（避免共享引用）
来源：http://hz.aizwys.cn/gtszmibuvf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jinghuilouyu.cn/gtkkouynek.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.52xcode.cn/gthmihkums.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.birdmap.top/gtjqvezcjg.html

TS:   [...arr];
来源：http://hz.quarkkingdee.top/gtzqnrxidi.html

Java: new ArrayList<>(list);
来源：http://hz.yueranfly.top/gteavokmmp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xuetiantiany.cn/gtipxxjmdw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ehwqpu.com/gtefvxwirx.html

C#:   new List<int>(list);
来源：http://hz.tianlin.xyz/gtwaivwtmy.html

[D23] reduce 累积计算
来源：http://hz.jianghu66.top/gtmodnpddi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.daxiang520.top/gttltecucq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhaomingkeji.xyz/gtiykpqtob.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xinyue.icu/gtravzfbvg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gaohongyu789.top/gtwguyeaqs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.0kj1m.cn/gtvfwxkjzy.html

Go:   // 手写循环
来源：http://hz.jinghuilouyu.cn/gtbrntzwiy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.dianchejie.cn/gttxkfibbq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xuetiantiany.cn/gttasvjndl.html

[D24] 字典 / Map 基本操作
来源：http://hz.tian-w.cn/gtmxiepxpz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shuidangran.top/gtrixcajhe.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.tianlin.xyz/gtmlameber.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.dashuyun.cn/gtefqzixin.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.chenzaomai.com/gtlmrjxuww.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nanxinkj.top/gtcumrscsx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.9152youxi.cn/gtocsdfqfr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jianghu66.top/gtbtgnqlte.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.sysykeji.top/gtgfcrawza.html

[D25] Set 集合去重与交并差
来源：http://hz.zhaomingkeji.xyz/gtkpmlsxha.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.daria6918.cn/gtwlqmqwfi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cashguo.top/gtvijilotn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.guowangkeji.top/gtceywptpo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.pengpengdd.cyou/gtumgpavkx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.havefunace.top/gtidpbjcwo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sweek.top/gtpdilwkgo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.daxiang520.top/gtyjhjpcey.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hongshengwenyu.top/gtjwfwnrfr.html

[D26] 数组转字符串
来源：http://hz.tian-w.cn/gthsymamha.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhaomingkeji.xyz/gthbrbezyz.html

PHP:  implode(", ", $arr);
来源：http://hz.zhongyouzk.top/gtaobhuzeq.html

JS:   arr.join(", ")
来源：http://hz.0kj1m.cn/gtoysgjtnk.html

TS:   arr.join(", ")
来源：http://hz.ybcxt.top/gtbynubdmh.html

Java: String.join(", ", list)
来源：http://hz.feifeiyinyue.top/gtweyxggds.html

Go:   strings.Join(strs, ", ")
来源：http://hz.redwolf501.top/gtevojcycx.html

Ruby: arr.join(", ")
来源：http://hz.chenjidiqi.icu/gtylkqjtit.html

C#:   string.Join(", ", list)
来源：http://hz.zhongyouzk.top/gttwjzsoyo.html

================================================================================
来源：http://hz.daxiang520.top/gtyqutaoro.html

E. 字符串处理
来源：http://hz.shanyushiyangkeji.top/gtoyotxwea.html

================================================================================
来源：http://hz.yonumen.top/gtoypgfvoz.html

[E01] 拼接字符串
来源：http://hz.snrcjt.cn/gthnemtfxt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.daxiang520.top/gtjspvzwjb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gogol.net.cn/gtpdebpnwm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zycfv.cn/gtsakbtgwg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.meibo888.top/gtyqrnuysd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yonumen.top/gttvhmnlea.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.feifeiyinyue.top/gtvumwdwwj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ydjk.org.cn/gtimdsyyop.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shuidangran.top/gtxbacoyxe.html

[E02] 重复字符串
来源：http://hz.chenzaomai.com/gtskpbitep.html

Py:   "ab" * 3
来源：http://hz.cashguo.top/gtviyktzwd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.birdmap.top/gtyccvsvty.html

JS:   "ab".repeat(3)
来源：http://hz.jqgfzy.top/gtyzglcumf.html

TS:   "ab".repeat(3)
来源：http://hz.zhoulong.xyz/gtlxbezduo.html

Java: "ab".repeat(3)
来源：http://hz.yuanzhike.top/gtwrgumzmi.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.9152youxi.cn/gtdeqlnduk.html

Ruby: "ab" * 3
来源：http://hz.fengsongda.top/gtutqmmonk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ybcxt.top/gtfuxzcfkt.html

[E03] 截取子串
来源：http://hz.bjfxy.top/gtrmmdqdsp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.wangdashe.top/gtwnhjcwqn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jianghu66.top/gthyosgwjf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yj20258888.top/gtwwzarbmz.html

TS:   s.slice(1, 4)
来源：http://hz.tianlin.xyz/gtwgslqzba.html

Java: s.substring(1, 4)
来源：http://hz.yuanzhike.top/gtsdgffhpq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhaomingkeji.xyz/gtojfkmhqu.html


<!-- 参考信息 -->