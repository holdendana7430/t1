代发 wailian999

TS:   arr.slice(1, 4);
来源：http://hz.zhixingplan.top/gtkaoimkvg.html

Java: list.subList(1, 4);
来源：http://hz.jinqigfzy.top/gtjgzrwryk.html

Go:   arr[1:4]
来源：http://hz.316326.xyz/gtgoakdgij.html

Ruby: arr[1, 3]
来源：http://hz.zhoulong.xyz/gtskagtfew.html

C#:   list.GetRange(1, 3);
来源：http://hz.0kj1m.cn/gttwkbwcqr.html

[D08] 合并两个数组
来源：http://hz.cqqwz.cn/gtsfyuhcud.html

Py:   a + b;  a.extend(b)
来源：http://hz.daxiang520.top/gtebpgldvm.html

PHP:  array_merge($a, $b);
来源：http://hz.xziqi.cn/gtwcfbkfuy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhixingplan.top/gtcsfjexpr.html

TS:   [...a, ...b];
来源：http://hz.zdqjudy.top/gtuaebdwkd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shzxlz.cn/gturmxfobn.html

Go:   append(a, b...)
来源：http://hz.zhongyouzk.top/gtplcllirx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cqqwz.cn/gtauqdgjra.html

C#:   a.Concat(b).ToList()
来源：http://hz.guannengcc.top/gtaemzakmy.html

[D09] 排序（升序）
来源：http://hz.andypj.xyz/gtjgkjsoqk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ppjwa.cn/gtdizyyduk.html

PHP:  sort($arr);
来源：http://hz.zhengqikj.top/gtxyhrlqrc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hnxiangtu.top/gtuzucumgx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yvedp.cn/gtjalieuye.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yj20258.top/gtcxylamvr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cdnleiting.top/gtgdapdirk.html

Ruby: arr.sort
来源：http://hz.mhx1999.top/gtiktutgzr.html

C#:   list.Sort();
来源：http://hz.c1oappe.top/gtixztzbob.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.mhx1999.top/gtduycaqss.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.shanyushiyangtech.top/gtqnysmowr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.iojbl.cn/gtoavetsbl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.dashuyun.cn/gtzetnsfqs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.guannengcc.top/gteiymbjpu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.aizwys.cn/gtjdkuwmju.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gzhubu.top/gtdsfkdqwg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.gaohongyu789.top/gtbuiqodiv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.gzhubu.top/gtdxzuxhbh.html

[D11] 反转数组
来源：http://hz.gaohongyu789.top/gtntrtofny.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.9152youxi.cn/gtyfjcxmts.html

PHP:  array_reverse($arr);
来源：http://hz.hammf.cn/gttxosvfxr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.daxiang520.top/gtcbwebxtv.html

TS:   [...arr].reverse();
来源：http://hz.jyoumei.cn/gtxnsxmutx.html

Java: Collections.reverse(list);
来源：http://hz.hywenlv.cn/gtkzefzryf.html

Go:   slices.Reverse(arr)
来源：http://hz.sxryk.cn/gtdbdpiasv.html

Ruby: arr.reverse
来源：http://hz.meibo888.top/gtmkyygezu.html

C#:   list.Reverse();
来源：http://hz.chenjidiqi.icu/gtzahrvjwl.html

[D12] 查找元素下标
来源：http://hz.ivvv.top/gtskcidjvp.html

Py:   arr.index(x);  x in arr
来源：http://hz.tanke756.top/gtjugxqkth.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.kuanghao11.cn/gtrlijnbus.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yonumen.top/gtuuzekdav.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tian-w.cn/gthzpizolh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gogol.net.cn/gtvwuouwqo.html

Go:   slices.Index(arr, x)
来源：http://hz.fzhhl.top/gtxbbassgw.html

Ruby: arr.index(x)
来源：http://hz.jqgufenzy.top/gtgugyrgzn.html

C#:   list.IndexOf(x);
来源：http://hz.sufxvd.cn/gtrmbghhca.html

[D13] 过滤（保留满足条件的）
来源：http://hz.chenzaomai.com/gtktrdlkos.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.c1oappe.top/gtkhqcgqze.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ehwqpu.com/gtpneonwtg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.smart0.xyz/gtgywliahi.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hnqzz.top/gtncjtvzwf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.vqdsnc.cn/gtzgqqphsz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.andypj.xyz/gtxrbfjqvq.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yj20258888.top/gtnmeggsyh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.gaohongyu789.top/gtyzlnhtgl.html

[D14] 映射转换（每个元素变形）
来源：http://hz.feifeiyinyue.top/gtdipjcpjg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.wangdashe.top/gtspsapzid.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.pycfn.com/gtperyfxjs.html

JS:   arr.map(x => x * 2)
来源：http://hz.pycfn.com/gticndqzgw.html

TS:   arr.map(x => x * 2)
来源：http://hz.ehwqpu.com/gtgspkgqxg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zycfv.cn/gtlyacbuay.html

Go:   // 手写循环
来源：http://hz.zhengqikj.top/gtkdnbiayv.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ivvv.top/gtdjtsvown.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yanxiufei.cn/gtmqqiepvc.html

[D15] 去重
来源：http://hz.jqgfzy.top/gtolwwapte.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.haohaochexian.top/gtovykjmjh.html

PHP:  array_unique($arr);
来源：http://hz.zhijiandao.cn/gtcpalnmse.html

JS:   [...new Set(arr)]
来源：http://hz.ydjk.org.cn/gteftkaylu.html

TS:   [...new Set(arr)]
来源：http://hz.zhijiandao.cn/gtmwahdfkj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.pycfn.com/gtizmwiogl.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhixingplan.top/gtllryqsdg.html

Ruby: arr.uniq
来源：http://hz.aibaodan.cn/gtgvosbiqd.html

C#:   list.Distinct().ToList()
来源：http://hz.gzhubu.top/gtpxxktikn.html

[D16] 求和与平均值
来源：http://hz.wangdashe.top/gtwqbpqgar.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ybcxt.top/gtsdzmkata.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xziqi.cn/gtzjxknpgw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.c1oappe.top/gtoyxwpvkt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigufen.top/gthwglplum.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.meibo888.top/gtngtyuefl.html

Go:   // 手写循环累加
来源：http://hz.yvedp.cn/gtbdijurvq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shzxlz.cn/gtiwmaaggb.html

C#:   list.Sum();  list.Average()
来源：http://hz.ybcxt.top/gthpdikxcu.html

[D17] 最大值与最小值
来源：http://hz.tanke756.top/gtqvigbwdx.html

Py:   max(arr);  min(arr)
来源：http://hz.wangshuangyany.cn/gtpqoioxys.html

PHP:  max($arr);  min($arr);
来源：http://hz.jyoumei.cn/gtwnrnnmgv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sweek.top/gtjmlhiubq.html

TS:   Math.max(...arr);
来源：http://hz.jinyuanbaomall.cn/gtujhgvvyf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.feifeiyinyue.top/gtkzoaoumc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhoulong.xyz/gtleyhubyy.html

Ruby: arr.max;  arr.min
来源：http://hz.quarkkingdee.top/gteljoujqc.html

C#:   list.Max();  list.Min()
来源：http://hz.jinghuilouyu.cn/gtreemeqnd.html

[D18] 扁平化嵌套数组
来源：http://hz.dianchejie.cn/gtaaxloytx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cqqwz.cn/gtiwuroeeu.html

PHP:  array_merge(...$nested);
来源：http://hz.sysykeji.top/gtzlwggsmg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sysykeji.top/gtlklxdebw.html

TS:   nested.flat();
来源：http://hz.jiagoushi.top/gtsrcnatrf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yangfankeji.com/gtkvflexhy.html

Go:   // 手写双层循环
来源：http://hz.yuxming.cn/gtkbkrvgsk.html

Ruby: nested.flatten
来源：http://hz.mhx1999.top/gtxzqxhfqc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ivvv.top/gtauhlwefp.html

[D19] 按字段分组
来源：http://hz.zhengqikj.top/gtruhxttqb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.smart0.xyz/gtjpnbyogb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shanyushiyangtech.top/gtwpfimdmj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jyoumei.cn/gtxhpisnze.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.birdmap.top/gtioibfqdj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.wangshuangyany.cn/gtndpcjkcr.html

Go:   // 手写 map[string][]T
来源：http://hz.nwbrower.top/gtavcqdisv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.guannengcc.top/gtpycgxrli.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gotoacloud.top/gtuqxwwvwv.html

[D20] 统计每个元素出现次数
来源：http://hz.nwbrower.top/gtazaomasn.html

Py:   Counter(arr)
来源：http://hz.aibaodan.cn/gtxyodrylk.html

PHP:  array_count_values($arr);
来源：http://hz.shzxlz.cn/gtbgixynmm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.snrcjt.cn/gtkhqyqswh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.kuanghao11.cn/gtgyqkuutc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hysaishi.cn/gtvpqjdszf.html

Go:   // 手写 map[T]int
来源：http://hz.cucudq.cn/gtcoxltjch.html

Ruby: arr.tally
来源：http://hz.pengpengdd.cyou/gtchowtmec.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.9152youxi.cn/gtfbrxosqx.html

[D21] 判断是否包含某元素
来源：http://hz.feifeiyinyue.top/gtudogqczz.html

Py:   x in arr
来源：http://hz.gogol.net.cn/gtzqvggidg.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gzhubu.top/gtwjfsdejy.html

JS:   arr.includes(x)
来源：http://hz.hysaishi.cn/gtmcwxkman.html

TS:   arr.includes(x)
来源：http://hz.cucudq.cn/gtcjzfteip.html

Java: list.contains(x)
来源：http://hz.xylfe.cn/gtmmvgqgsx.html

Go:   slices.Contains(arr, x)
来源：http://hz.yongpay.top/gtphlumqap.html

Ruby: arr.include?(x)
来源：http://hz.ydzc1.top/gtpwjbntpb.html

C#:   list.Contains(x)
来源：http://hz.jinghuilouyu.cn/gtkwnmtduc.html

[D22] 复制数组（避免共享引用）
来源：http://hz.quarkkingdee.top/gtxyjwzfad.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.havefunace.top/gtvmkdmjvr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yj202588.top/gtnsgrrdnb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.pycfn.com/gtimpeuitm.html

TS:   [...arr];
来源：http://hz.zycfv.cn/gthulkgcej.html

Java: new ArrayList<>(list);
来源：http://hz.yangfankeji.com/gtpwjulvqy.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.feifeiyinyue.top/gtclrjlaio.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yangfankeji.com/gthvysnjno.html

C#:   new List<int>(list);
来源：http://hz.feifeiyinyue.top/gtqustfwkh.html

[D23] reduce 累积计算
来源：http://hz.jinghuilouyu.cn/gthadsvmre.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinqigfzy.top/gtfhtagyfv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xinyue.icu/gtfqptajob.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.0kj1m.cn/gtyopqktvl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigufen.top/gtbvyyfjzi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.wangdashe.top/gtdrshyfih.html

Go:   // 手写循环
来源：http://hz.smart0.xyz/gtudlwqser.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yangfankeji.com/gtpipolmtl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhaomingkeji.xyz/gtvghlubvs.html

[D24] 字典 / Map 基本操作
来源：http://hz.chenjidiqi.icu/gtbknrdgnv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ivvv.top/gtqmzucevp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhiwuduotai.top/gtfepemedn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ywan-chungtsiang.top/gtvwdlgdvq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.birdmap.top/gtffhedccc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jlsjyb.cn/gtaandmeuq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zdqjudy.top/gtworwiyaj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cqqwz.cn/gtbquzgyst.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yanxiufei.cn/gttxxhvlsp.html

[D25] Set 集合去重与交并差
来源：http://hz.zhengqikj.top/gtfxrurlfs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shangyingyoupin.top/gtvybpepjw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.vqdsnc.cn/gtxwawnllj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shzxlz.cn/gtncwqzfqd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhengqikj.top/gtjygciful.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yonumen.top/gtezfnwisk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yj20258.top/gtkchsbpiy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jianghu66.top/gtmseuyivl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.meibo888.top/gtftglghkn.html

[D26] 数组转字符串
来源：http://hz.nanxuanxn.top/gtcrthkthw.html

Py:   ", ".join(map(str, arr))
来源：http://hz.haohaochexian.top/gtyzbgfirh.html

PHP:  implode(", ", $arr);
来源：http://hz.chenzaomai.com/gtpiwivpxf.html

JS:   arr.join(", ")
来源：http://hz.ybcxt.top/gtqeosoljk.html

TS:   arr.join(", ")
来源：http://hz.yuanzhike.top/gtljeyxvmr.html

Java: String.join(", ", list)
来源：http://hz.xziqi.cn/gtnqcaflwc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.kuanghao11.cn/gtzhvrryxy.html

Ruby: arr.join(", ")
来源：http://hz.feifeiyinyue.top/gthqpreqxe.html

C#:   string.Join(", ", list)
来源：http://hz.shanyushiyangtech.top/gtdjrzjioj.html

================================================================================
来源：http://hz.zhoulong.xyz/gtoidqoczw.html

E. 字符串处理
来源：http://hz.yuxming.cn/gtcaeosrml.html

================================================================================
来源：http://hz.sweek.top/gtxuvdvctc.html

[E01] 拼接字符串
来源：http://hz.gaohongyu789.top/gtzgqmglvk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.chenlongwang.top/gtvkmgwrbs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yj20258.top/gtzytvcbfm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhongyouzk.top/gtfjnzrltw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xinyue.icu/gtoxofuckp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ybcxt.top/gtekuhritb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jinghuilouyu.cn/gtqmyvdtgw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.fengsongda.top/gtezlxyscs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cdnleiting.top/gttxofppmq.html

[E02] 重复字符串
来源：http://hz.pycfn.com/gtppevpmsq.html

Py:   "ab" * 3
来源：http://hz.mhx1999.top/gthfxonujz.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sxryk.cn/gtltzzmvvm.html

JS:   "ab".repeat(3)
来源：http://hz.shuidangran.top/gtptnbqfvy.html

TS:   "ab".repeat(3)
来源：http://hz.andypj.xyz/gtfecubgdw.html

Java: "ab".repeat(3)
来源：http://hz.quarkkingdee.top/gtecmgxmqa.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.sufxvd.cn/gtnomagsnv.html

Ruby: "ab" * 3
来源：http://hz.chenzaomai.com/gtuhoddvjn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jinyuanbaomall.cn/gtvdwjcujn.html

[E03] 截取子串
来源：http://hz.guannengcc.top/gtyzxjchfd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.daxiang520.top/gtksyrkscv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.0kj1m.cn/gtlvwozdbj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hnxiangtu.top/gtlnkpuucs.html

TS:   s.slice(1, 4)
来源：http://hz.wangshuangyany.cn/gtxfutwuow.html

Java: s.substring(1, 4)
来源：http://hz.316326.xyz/gtgelpnhrz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.haohaochexian.top/gtcergfdvd.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.kuanghao11.cn/gtxuidgzur.html

C#:   s.Substring(1, 3)
来源：http://hz.feifeiyinyue.top/gtekwgiqhj.html

[E04] 查找子串位置
来源：http://hz.shuidangran.top/gtftifbepn.html

Py:   s.find("x");  s.index("x")
来源：http://hz.gzhubu.top/gtkowkcdud.html

PHP:  strpos($s, "x");
来源：http://hz.chenlongwang.top/gttomigplx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.316326.xyz/gtxbeoswyy.html

TS:   s.indexOf("x")
来源：http://hz.wangshuangyany.cn/gtqebbeavv.html

Java: s.indexOf("x")
来源：http://hz.zhijiandao.cn/gtoevbuzrs.html

Go:   strings.Index(s, "x")
来源：http://hz.xinyue.icu/gtokqgyppy.html

Ruby: s.index("x")
来源：http://hz.nwbrower.top/gtlnowmmgk.html

C#:   s.IndexOf("x")
来源：http://hz.zhongyouzk.top/gtkzbsywcc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yongpay.top/gtzwhznixk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hnqzz.top/gtacnhjzvl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.meibo888.top/gtrnlrgart.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yanxiufei.cn/gtbdhzqlpj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.nanxuanxn.top/gtqrytkqcs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gogol.net.cn/gtgbajqbky.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.iojbl.cn/gtldtprqqy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.mhx1999.top/gtfhaldgpr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cdnleiting.top/gtqyfhtrgr.html

[E06] 替换子串
来源：http://hz.xinyue.icu/gtihbmjzsm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hongshengwenyu.top/gtakulgbxz.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.dianchejie.cn/gtifnnqomp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cashguo.top/gtrkwwxdxt.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gtszkblwxu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hnxiangtu.top/gteeofbvcm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ppjwa.cn/gtrqftglhu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.snrcjt.cn/gthnaozylc.html

C#:   s.Replace("a", "b")
来源：http://hz.xylfe.cn/gtfkqtsyti.html

[E07] 按分隔符拆分
来源：http://hz.ybcxt.top/gtpfersxzm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.guowangkeji.top/gtiobbevso.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.sxryk.cn/gtchehsxea.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.birdmap.top/gtflgprrcy.html

TS:   s.split(",")
来源：http://hz.aizwys.cn/gtlrrujwsj.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jlsjyb.cn/gtsacnmeaj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.chenlongwang.top/gtjeqvhtfy.html

Ruby: s.split(",");  s.split
来源：http://hz.jqgufenzy.top/gtbqtfojor.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.dianchejie.cn/gtkmxnaiqt.html

[E08] 数组按分隔符合并
来源：http://hz.sufxvd.cn/gtmizfrlya.html

Py:   ",".join(items)
来源：http://hz.sufxvd.cn/gtdaymzgxi.html

PHP:  implode(",", $items);
来源：http://hz.nanxuanxn.top/gtgwlmnjtv.html

JS:   items.join(",")
来源：http://hz.gotoacloud.top/gthfapkumw.html

TS:   items.join(",")
来源：http://hz.vqdsnc.cn/gtcmadibkb.html

Java: String.join(",", items)
来源：http://hz.52xcode.cn/gtxvyqojzf.html

Go:   strings.Join(items, ",")
来源：http://hz.dashuyun.cn/gtcrclzuha.html

Ruby: items.join(",")
来源：http://hz.cashguo.top/gtlyvxtlke.html

C#:   string.Join(",", items)
来源：http://hz.kuanghao11.cn/gtqarwezpw.html

[E09] 去除所有空白字符
来源：http://hz.hysaishi.cn/gtemctscot.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hnxiangtu.top/gtrmimuojz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xuanzx.com/gthhskyiic.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jqgfzy.top/gtvewyowkc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cheryme.top/gtsqtdcciz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.cdnleiting.top/gtiwnwxbqr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.daria6918.cn/gteqnxqlwc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sufxvd.cn/gtyszipirs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yueranfly.top/gtjyayoefm.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hysaishi.cn/gtglvizpkd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.pycfn.com/gtwlwqcjiz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yuanzhike.top/gtlrxrqpkg.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhaomingkeji.xyz/gtbnlqraja.html

TS:   "7".padStart(3, "0")
来源：http://hz.hongshengwenyu.top/gteyyvwudm.html

Java: String.format("%03d", 7)
来源：http://hz.pycfn.com/gtcnkqfsti.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.meibo888.top/gtqbzrjsaw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gaohongyu789.top/gtudzubigf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ydjk.org.cn/gtnczpdaxj.html

[E11] 反转字符串
来源：http://hz.hnqzz.top/gtnvdsoqty.html

Py:   s[::-1]
来源：http://hz.hfpthk.cn/gtkvqldqyq.html

PHP:  strrev($s);
来源：http://hz.fengsongda.top/gtnwuaeizs.html

JS:   [...s].reverse().join("")
来源：http://hz.hammf.cn/gtzptyhozi.html

TS:   [...s].reverse().join("")
来源：http://hz.kuanghao11.cn/gtpipdoorz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ydzc1.top/gtduxlmbic.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yanxiufei.cn/gtlvvxorzg.html

Ruby: s.reverse
来源：http://hz.hnxiangtu.top/gteouirzgt.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jqgufenzy.top/gtvmuiyyku.html

[E12] 统计某字符出现次数
来源：http://hz.zhaomingkeji.xyz/gtrqvqelad.html

Py:   s.count("a")
来源：http://hz.sysykeji.top/gtumkyuqod.html

PHP:  substr_count($s, "a");
来源：http://hz.hongshengwenyu.top/gtqzxkvjgw.html

JS:   s.split("a").length - 1
来源：http://hz.andypj.xyz/gtqwpvupps.html

TS:   s.split("a").length - 1
来源：http://hz.ydjk.org.cn/gtaomdbyiv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jiagoushi.top/gtfxpqqyzk.html

Go:   strings.Count(s, "a")
来源：http://hz.gaohongyu789.top/gtufyxvcsq.html

Ruby: s.count("a")
来源：http://hz.zhoulong.xyz/gthlpjdzvk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xinyue.icu/gtyolaqofz.html

[E13] 逐字符遍历
来源：http://hz.xylfe.cn/gteuqqtpde.html

Py:   for ch in s: print(ch)
来源：http://hz.hnxiangtu.top/gtevzadzva.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ydjk.org.cn/gtjfemhugi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xziqi.cn/gtwkevjnwv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yueranfly.top/gtolnpveix.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ehwqpu.com/gtolsillnv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.aibaodan.cn/gthbcafqbd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shanyushiyangtech.top/gtdejomxlc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.9152youxi.cn/gtfzubhymt.html

[E14] URL 编码与 Base64
来源：http://hz.bjfxy.top/gtqosrahnj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shangyingyoupin.top/gtyiicacvs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.bjfxy.top/gthapapmkd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hfpthk.cn/gtlugocaox.html


<!-- 参考信息 -->