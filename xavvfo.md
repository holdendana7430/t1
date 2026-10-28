代发 wailian999

Py:   len(arr)
来源：http://hz.snrcjt.cn/gtaqmvrmqs.html

PHP:  count($arr);
来源：http://hz.jinghuilouyu.cn/gttoqbfitp.html

JS:   arr.length
来源：http://hz.cdnleiting.top/gtvwlfylyo.html

TS:   arr.length
来源：http://hz.jlsjyb.cn/gtmlfnbxqw.html

Java: list.size();
来源：http://hz.zhiwuduotai.top/gtlbqiajlu.html

Go:   len(arr)
来源：http://hz.jqgufenzy.top/gtuseuasbd.html

Ruby: arr.length; arr.size
来源：http://hz.chenlongwang.top/gtunpfpyfy.html

C#:   list.Count;
来源：http://hz.svipenyu.cn/gtzfwnvwkk.html

[D07] 切片 / 取子数组
来源：http://hz.yanxiufei.cn/gtovhoyeht.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hnqzz.top/gtrcirlznf.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xinyue.icu/gtveiuwxom.html

JS:   arr.slice(1, 4);
来源：http://hz.sysykeji.top/gtpmrobnpt.html

TS:   arr.slice(1, 4);
来源：http://hz.meibo888.top/gtgcylxytn.html

Java: list.subList(1, 4);
来源：http://hz.kuanghao11.cn/gtevueggqr.html

Go:   arr[1:4]
来源：http://hz.zhiwuduotai.top/gtmxqqwyva.html

Ruby: arr[1, 3]
来源：http://hz.zhijiandao.cn/gtyxxtohqy.html

C#:   list.GetRange(1, 3);
来源：http://hz.meibo888.top/gtpsavnyvg.html

[D08] 合并两个数组
来源：http://hz.jinqigufen.top/gtnsdppywh.html

Py:   a + b;  a.extend(b)
来源：http://hz.316326.xyz/gthoilbeos.html

PHP:  array_merge($a, $b);
来源：http://hz.hammf.cn/gtodscykqb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hnxiangtu.top/gtazbyeikz.html

TS:   [...a, ...b];
来源：http://hz.ybcxt.top/gtcjlemmqx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.nanxuanxn.top/gtmdvzmgen.html

Go:   append(a, b...)
来源：http://hz.xingfuxueyuan.xyz/gthfyncgwd.html

Ruby: a + b;  a.concat(b)
来源：http://hz.daria6918.cn/gtejilchom.html

C#:   a.Concat(b).ToList()
来源：http://hz.hysaishi.cn/gtbtoqvxih.html

[D09] 排序（升序）
来源：http://hz.cdnleiting.top/gtspkbeciu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.aizwys.cn/gtyhmrccmf.html

PHP:  sort($arr);
来源：http://hz.cheryme.top/gtnzghlyrg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hysaishi.cn/gttifqzawn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xingfuxueyuan.xyz/gtatommvxu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.aibaodan.cn/gtxnghpbtw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ydjk.org.cn/gtyuucgiix.html

Ruby: arr.sort
来源：http://hz.zdqjudy.top/gtbcdylgam.html

C#:   list.Sort();
来源：http://hz.aizwys.cn/gtlxmhvmys.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yanxiufei.cn/gtewmlkrjy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cdnleiting.top/gtmmxgfbsm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.pycfn.com/gtygvelvqw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.c1oappe.top/gtdahhoenm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yanxiufei.cn/gtaddezube.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.vqdsnc.cn/gtniiyqgdb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinqigufen.top/gtlwcpctyd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.kuanghao11.cn/gtsknnmdit.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.sysykeji.top/gtuysnzyxt.html

[D11] 反转数组
来源：http://hz.hnxiangtu.top/gtlsnudghh.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hnxiangtu.top/gtltcvhgjr.html

PHP:  array_reverse($arr);
来源：http://hz.birdmap.top/gtsggsonee.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.guannengcc.top/gttdokxfrv.html

TS:   [...arr].reverse();
来源：http://hz.quarkkingdee.top/gtpwhktgre.html

Java: Collections.reverse(list);
来源：http://hz.yj20258.top/gtoobfcgbi.html

Go:   slices.Reverse(arr)
来源：http://hz.daxiang520.top/gtlsrrserw.html

Ruby: arr.reverse
来源：http://hz.zhoulong.xyz/gtvqbapscl.html

C#:   list.Reverse();
来源：http://hz.jlsjyb.cn/gtyaglkhet.html

[D12] 查找元素下标
来源：http://hz.sufxvd.cn/gtstldxmvc.html

Py:   arr.index(x);  x in arr
来源：http://hz.ivvv.top/gtzndiznpp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yueranfly.top/gtqlzvgayr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zdqjudy.top/gtxlqxaxmy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuxming.cn/gtyqvtwjhc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.nanxinkj.top/gtvdvshyrv.html

Go:   slices.Index(arr, x)
来源：http://hz.xziqi.cn/gthpewpnlc.html

Ruby: arr.index(x)
来源：http://hz.hnxiangtu.top/gtwrdiwpwo.html

C#:   list.IndexOf(x);
来源：http://hz.tian-w.cn/gtyvlxuvlo.html

[D13] 过滤（保留满足条件的）
来源：http://hz.wangdashe.top/gtdcjmqjeo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cheryme.top/gtnenlbhum.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.haohaochexian.top/gtogsqshzq.html

JS:   arr.filter(x => x > 3)
来源：http://hz.sufxvd.cn/gtslkimxfw.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhijiandao.cn/gtqesemirq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sweek.top/gtnttchtwm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hongshengwenyu.top/gtkwlivzzb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.vqdsnc.cn/gtvqsipdwr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yanxiufei.cn/gtqlyysqqk.html

[D14] 映射转换（每个元素变形）
来源：http://hz.9152youxi.cn/gtrpcpbugg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ywan-chungtsiang.top/gtutcrqbku.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.fzhhl.top/gtqaawauso.html

JS:   arr.map(x => x * 2)
来源：http://hz.hnqzz.top/gtpuurlpil.html

TS:   arr.map(x => x * 2)
来源：http://hz.nwbrower.top/gtiarabebb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.meibo888.top/gtpwfcgwym.html

Go:   // 手写循环
来源：http://hz.svipenyu.cn/gtqcodbxer.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sysykeji.top/gtvdvjfswu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhengqikj.top/gtxhtmfnxa.html

[D15] 去重
来源：http://hz.gotoacloud.top/gtewduavkh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yuanzhike.top/gtynwsxbqw.html

PHP:  array_unique($arr);
来源：http://hz.hongshengwenyu.top/gtrsdwkgel.html

JS:   [...new Set(arr)]
来源：http://hz.zhixingplan.top/gtvjmhylvv.html

TS:   [...new Set(arr)]
来源：http://hz.gotoacloud.top/gtqwyrqfsj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yonumen.top/gtyligkpwz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cqqwz.cn/gtjbvqfxra.html

Ruby: arr.uniq
来源：http://hz.shanyushiyangkeji.top/gtkldqjdet.html

C#:   list.Distinct().ToList()
来源：http://hz.wangshuangyany.cn/gtgizgbwqj.html

[D16] 求和与平均值
来源：http://hz.sufxvd.cn/gtdpgeifav.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.52xcode.cn/gtsmjelgtb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.guannengcc.top/gthulvwrlx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xuetiantiany.cn/gtowfifjkz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xylfe.cn/gtugguimnb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.andypj.xyz/gtfzlwrkbb.html

Go:   // 手写循环累加
来源：http://hz.xylfe.cn/gtmbnpuqdt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.9152youxi.cn/gtrvevwuqj.html

C#:   list.Sum();  list.Average()
来源：http://hz.yj20258.top/gtbboxhpwu.html

[D17] 最大值与最小值
来源：http://hz.pengpengdd.cyou/gtnhfvrmyc.html

Py:   max(arr);  min(arr)
来源：http://hz.andypj.xyz/gtweatygbg.html

PHP:  max($arr);  min($arr);
来源：http://hz.hammf.cn/gtthnqozok.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cdnleiting.top/gtgpxandgq.html

TS:   Math.max(...arr);
来源：http://hz.shzxlz.cn/gtrrqdoipa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sysykeji.top/gttyezcvbc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.mhx1999.top/gtsyxsrfnq.html

Ruby: arr.max;  arr.min
来源：http://hz.xinyue.icu/gtwjluoutk.html

C#:   list.Max();  list.Min()
来源：http://hz.smart0.xyz/gtmwuevbwi.html

[D18] 扁平化嵌套数组
来源：http://hz.fengsongda.top/gtbxdpceez.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.daxiang520.top/gtmwrdtlkc.html

PHP:  array_merge(...$nested);
来源：http://hz.smart0.xyz/gtghzyjbcd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.dianchejie.cn/gtfpoxmndq.html

TS:   nested.flat();
来源：http://hz.zhongyouzk.top/gtfdohiocb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.bjfxy.top/gtuqtfcpyt.html

Go:   // 手写双层循环
来源：http://hz.tanke756.top/gtipfxnlob.html

Ruby: nested.flatten
来源：http://hz.xziqi.cn/gtqjsuebom.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hysaishi.cn/gtyhmkqquh.html

[D19] 按字段分组
来源：http://hz.hongshengwenyu.top/gtbwemebbn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hnxiangtu.top/gtoykpfvvg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hammf.cn/gtpxsfmkhp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.dianchejie.cn/gtoeursvpc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.iojbl.cn/gtcclildoj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.tanke756.top/gtapbgoxcn.html

Go:   // 手写 map[string][]T
来源：http://hz.xuetiantiany.cn/gtaopjuyyp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xziqi.cn/gthclxhxxr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.tanke756.top/gtlkypjqmx.html

[D20] 统计每个元素出现次数
来源：http://hz.smart0.xyz/gtfjoswqdk.html

Py:   Counter(arr)
来源：http://hz.gzhubu.top/gtqpilypfu.html

PHP:  array_count_values($arr);
来源：http://hz.nwbrower.top/gtdpzdfvpv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnqzz.top/gtteazbejh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.meibo888.top/gtmxvibhyo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.chenlongwang.top/gtrzrcsmpg.html

Go:   // 手写 map[T]int
来源：http://hz.jianghu66.top/gtaknwiarh.html

Ruby: arr.tally
来源：http://hz.zhongyouzk.top/gtkzdrqlkz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.birdmap.top/gtcglylxdt.html

[D21] 判断是否包含某元素
来源：http://hz.shangyingyoupin.top/gtneasyfcm.html

Py:   x in arr
来源：http://hz.52xcode.cn/gtcvumjauf.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gotoacloud.top/gtqhtnbsuo.html

JS:   arr.includes(x)
来源：http://hz.jyoumei.cn/gtywzfmrvn.html

TS:   arr.includes(x)
来源：http://hz.quarkkingdee.top/gtovxyjxtu.html

Java: list.contains(x)
来源：http://hz.cdnleiting.top/gtukrveffr.html

Go:   slices.Contains(arr, x)
来源：http://hz.sysykeji.top/gtqjxnwiam.html

Ruby: arr.include?(x)
来源：http://hz.guowangkeji.top/gtjpbnaxza.html

C#:   list.Contains(x)
来源：http://hz.jinghuilouyu.cn/gtltixvned.html

[D22] 复制数组（避免共享引用）
来源：http://hz.dianchejie.cn/gthothpfat.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hnqzz.top/gtuocbubmb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hnxiangtu.top/gtjestvkgr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.52xcode.cn/gtlzefxnph.html

TS:   [...arr];
来源：http://hz.hammf.cn/gtudehmeua.html

Java: new ArrayList<>(list);
来源：http://hz.hnqzz.top/gtpurvvhgp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yuxming.cn/gtgpmcgkrb.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nwbrower.top/gtnqrfcafz.html

C#:   new List<int>(list);
来源：http://hz.mhx1999.top/gtmnumhpve.html

[D23] reduce 累积计算
来源：http://hz.tanke756.top/gtvnrnarsl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hnxiangtu.top/gtfqqnhtfa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ehwqpu.com/gtmjuarnph.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xuetiantiany.cn/gtulgxrgps.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yongpay.top/gtbpmkbbzx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hnqzz.top/gtvefxyaiy.html

Go:   // 手写循环
来源：http://hz.kuanghao11.cn/gtzuztwtlv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ehwqpu.com/gtndianetn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.daria6918.cn/gtbyubxnqu.html

[D24] 字典 / Map 基本操作
来源：http://hz.nanxinkj.top/gtqylwxmdb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.fengsongda.top/gtymqxjaic.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.daria6918.cn/gtztxyyybx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.feifeiyinyue.top/gtbxyfuozl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jqgufenzy.top/gtvzbzmbln.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.dianchejie.cn/gtjdksoijl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.9152youxi.cn/gtbrcrjcyv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.guowangkeji.top/gtbsmpjzfr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.aibaodan.cn/gtuvredhjs.html

[D25] Set 集合去重与交并差
来源：http://hz.chenzaomai.com/gtfalliume.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xziqi.cn/gtaxznmcwu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.0kj1m.cn/gtzbtrtbza.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ybcxt.top/gtektobvlu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hammf.cn/gtyjqrkupm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yueranfly.top/gtgmzewdzz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yj20258888.top/gtngkqiuub.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zycfv.cn/gtalycxwbs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hfpthk.cn/gtujwplapu.html

[D26] 数组转字符串
来源：http://hz.guowangkeji.top/gtxzfiqxgs.html

Py:   ", ".join(map(str, arr))
来源：http://hz.guannengcc.top/gtudyfvvjq.html

PHP:  implode(", ", $arr);
来源：http://hz.ydzc1.top/gtzdgfivqm.html

JS:   arr.join(", ")
来源：http://hz.jinghuilouyu.cn/gtxjoxeqdh.html

TS:   arr.join(", ")
来源：http://hz.cucudq.cn/gtckcekihm.html

Java: String.join(", ", list)
来源：http://hz.vqdsnc.cn/gtlnqgddit.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cqqwz.cn/gtupnpdkzo.html

Ruby: arr.join(", ")
来源：http://hz.wangshuangyany.cn/gtcqgadket.html

C#:   string.Join(", ", list)
来源：http://hz.xuetiantiany.cn/gtvpiexbsc.html

================================================================================
来源：http://hz.hnqzz.top/gtklkbbnsd.html

E. 字符串处理
来源：http://hz.meibo888.top/gtwajuashg.html

================================================================================
来源：http://hz.havefunace.top/gtvvcwyxjm.html

[E01] 拼接字符串
来源：http://hz.316326.xyz/gtgzwrhjay.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.dashuyun.cn/gtbnbsezjs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.52xcode.cn/gtiudathzj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xylfe.cn/gtpkvsvlup.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sufxvd.cn/gtkpyamcxz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.iojbl.cn/gtyzcpqwem.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhixingplan.top/gtxwfjxszx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj20258.top/gtyrkprviu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cucudq.cn/gtjraczbnu.html

[E02] 重复字符串
来源：http://hz.yj20258888.top/gtqxllkesh.html

Py:   "ab" * 3
来源：http://hz.vqdsnc.cn/gtowhtlicf.html

PHP:  str_repeat("ab", 3);
来源：http://hz.shzxlz.cn/gtenbjiniz.html

JS:   "ab".repeat(3)
来源：http://hz.nwbrower.top/gtjxljeyju.html

TS:   "ab".repeat(3)
来源：http://hz.wangdashe.top/gtpacsgkvd.html

Java: "ab".repeat(3)
来源：http://hz.cheryme.top/gtzpxwcney.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yj20258888.top/gtoqgpqhvy.html

Ruby: "ab" * 3
来源：http://hz.ywan-chungtsiang.top/gtmmeiinhc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shuidangran.top/gttvuhdowy.html

[E03] 截取子串
来源：http://hz.birdmap.top/gtkqhrjwvw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ydjk.org.cn/gtzqlteljl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ppjwa.cn/gtzrzhnnfg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.aizwys.cn/gtajoadnwx.html

TS:   s.slice(1, 4)
来源：http://hz.yj20258.top/gtfpecdjjg.html

Java: s.substring(1, 4)
来源：http://hz.52xcode.cn/gtxtpfvmwn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.sysykeji.top/gtmfpfwops.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xinyue.icu/gtezmqrieb.html

C#:   s.Substring(1, 3)
来源：http://hz.mhx1999.top/gtqeauawst.html

[E04] 查找子串位置
来源：http://hz.aibaodan.cn/gtbnsiwtib.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhongyouzk.top/gtxwnpqcns.html

PHP:  strpos($s, "x");
来源：http://hz.shanyushiyangkeji.top/gtmixrcqmy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.haohaochexian.top/gtiextxyrk.html

TS:   s.indexOf("x")
来源：http://hz.hammf.cn/gtslvhhjzz.html

Java: s.indexOf("x")
来源：http://hz.yj202588.top/gthkftmeeb.html

Go:   strings.Index(s, "x")
来源：http://hz.jyoumei.cn/gtaejgvtnd.html

Ruby: s.index("x")
来源：http://hz.kuanghao11.cn/gtwdlfpyau.html

C#:   s.IndexOf("x")
来源：http://hz.andypj.xyz/gtekcudxge.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhiwuduotai.top/gtxlttaoqr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.sufxvd.cn/gtophmknuv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.cqqwz.cn/gtnwdezsig.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tianlin.xyz/gtnkepbxuv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhoulong.xyz/gtvhcglafb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shuidangran.top/gtaartvzmx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.daria6918.cn/gthemocnjn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yueranfly.top/gtuuevmecj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cucudq.cn/gturifjpjw.html

[E06] 替换子串
来源：http://hz.ydjk.org.cn/gtswaihhgi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.meibo888.top/gtttdvsvts.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hywenlv.cn/gtbkbmgbzs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shuidangran.top/gtbzozdmxb.html

TS:   s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gtpimvdgln.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sweek.top/gtvifadamu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yj202588.top/gtkznppjtu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jinqigfzy.top/gtopvjmavk.html

C#:   s.Replace("a", "b")
来源：http://hz.aizwys.cn/gtrjpyyloq.html

[E07] 按分隔符拆分
来源：http://hz.hfpthk.cn/gtmrtwiezm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.vqdsnc.cn/gtsneqahgb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cashguo.top/gtucdiyjzd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yueranfly.top/gthkfjzhbo.html

TS:   s.split(",")
来源：http://hz.jinqigufen.top/gtplaevios.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cheryme.top/gtltkkohwr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhoulong.xyz/gtcrarkcnc.html

Ruby: s.split(",");  s.split
来源：http://hz.yvedp.cn/gtcvucrecb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ivvv.top/gtaasmdrwa.html

[E08] 数组按分隔符合并
来源：http://hz.birdmap.top/gtzeevlfsk.html

Py:   ",".join(items)
来源：http://hz.yanxiufei.cn/gtcpiqkwhz.html

PHP:  implode(",", $items);
来源：http://hz.shanyushiyangtech.top/gtqrghmydt.html

JS:   items.join(",")
来源：http://hz.jinqigufen.top/gtnmfugenq.html

TS:   items.join(",")
来源：http://hz.svipenyu.cn/gtpdkgemcg.html

Java: String.join(",", items)
来源：http://hz.xziqi.cn/gtlxiygmrk.html

Go:   strings.Join(items, ",")
来源：http://hz.yongpay.top/gtbfzlltdn.html

Ruby: items.join(",")
来源：http://hz.dianchejie.cn/gtoezkbedf.html

C#:   string.Join(",", items)
来源：http://hz.jianghu66.top/gtyxlbmpoo.html

[E09] 去除所有空白字符
来源：http://hz.ydzc1.top/gtgwtdmsjj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jyoumei.cn/gtjkefhmoh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhongyouzk.top/gtpytwofmw.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.pycfn.com/gtomaqtjum.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shangyingyoupin.top/gtpwdbgzzh.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenzaomai.com/gtajkzeojb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shanyushiyangkeji.top/gtutktenje.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ivvv.top/gtkccqqexa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jqgfzy.top/gtewzntjwn.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ydzc1.top/gtdurcgkjt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.daxiang520.top/gtqsqjclih.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jyoumei.cn/gtzhtkugsc.html

JS:   "7".padStart(3, "0")
来源：http://hz.0kj1m.cn/gtcwlnzttp.html

TS:   "7".padStart(3, "0")
来源：http://hz.nanxuanxn.top/gtwuaxvaez.html

Java: String.format("%03d", 7)
来源：http://hz.jinqigfzy.top/gtifkwemcr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.daria6918.cn/gticyxtkba.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hysaishi.cn/gtxfmftats.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.pengpengdd.cyou/gtletdqmza.html

[E11] 反转字符串
来源：http://hz.jyoumei.cn/gtyxrlktew.html

Py:   s[::-1]
来源：http://hz.xingfuxueyuan.xyz/gtcoaugfao.html

PHP:  strrev($s);
来源：http://hz.smart0.xyz/gtbcyrjuda.html

JS:   [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtrijbawtn.html

TS:   [...s].reverse().join("")
来源：http://hz.kuanghao11.cn/gtzchouscz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jianghu66.top/gtnxukkqgg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.wangshuangyany.cn/gtcizizkdv.html

Ruby: s.reverse
来源：http://hz.xylfe.cn/gtsvbvqhnb.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhaomingkeji.xyz/gtutthslzj.html

[E12] 统计某字符出现次数
来源：http://hz.andypj.xyz/gtqxxsjoio.html

Py:   s.count("a")
来源：http://hz.52xcode.cn/gtcxxmbnka.html

PHP:  substr_count($s, "a");
来源：http://hz.chenlongwang.top/gtlmxksqsz.html

JS:   s.split("a").length - 1
来源：http://hz.jyoumei.cn/gtzjmebcjh.html

TS:   s.split("a").length - 1
来源：http://hz.hnqzz.top/gtfgmyezef.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.dashuyun.cn/gtfhmilgwj.html

Go:   strings.Count(s, "a")
来源：http://hz.yuxming.cn/gtioizrlsm.html

Ruby: s.count("a")
来源：http://hz.wangshuangyany.cn/gtoanvsbjv.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ydzc1.top/gtravcbxzz.html

[E13] 逐字符遍历
来源：http://hz.zhijiandao.cn/gtyvealzmp.html


<!-- 参考信息 -->