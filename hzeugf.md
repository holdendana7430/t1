代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://hz.smart0.xyz/gtwzyfulye.html

C#:   a.Concat(b).ToList()
来源：http://hz.cheryme.top/gtxjhxqnqj.html

[D09] 排序（升序）
来源：http://hz.cqqwz.cn/gtwjfawdbp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hnxiangtu.top/gthhypihia.html

PHP:  sort($arr);
来源：http://hz.yangfankeji.com/gthnvijgoe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zycfv.cn/gtqcdqrutz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xylfe.cn/gtayfxxotj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.0kj1m.cn/gtmedrelsg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cheryme.top/gtnsgafqpw.html

Ruby: arr.sort
来源：http://hz.ehwqpu.com/gtrqohuktg.html

C#:   list.Sort();
来源：http://hz.jiagoushi.top/gtvyglvsrv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhixingplan.top/gtyguytoqk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.chenzaomai.com/gtryzgqnti.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yongpay.top/gtetmopihe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuanzx.com/gtijgponrw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuxming.cn/gtefaldjvk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.fzhhl.top/gttuwnoxhw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhengqikj.top/gthwzjjbvg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.sxryk.cn/gthhwpozps.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.tianlin.xyz/gtnusjuset.html

[D11] 反转数组
来源：http://hz.shangyingyoupin.top/gtwwrqrmin.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.chenjidiqi.icu/gtnkzquipo.html

PHP:  array_reverse($arr);
来源：http://hz.svipenyu.cn/gtmnulltkd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ydzc1.top/gtdxvcpvmz.html

TS:   [...arr].reverse();
来源：http://hz.iojbl.cn/gtkysczncv.html

Java: Collections.reverse(list);
来源：http://hz.wangshuangyany.cn/gtwndsihjh.html

Go:   slices.Reverse(arr)
来源：http://hz.shuidangran.top/gtiuewkwgk.html

Ruby: arr.reverse
来源：http://hz.zhijiandao.cn/gtejxuufxh.html

C#:   list.Reverse();
来源：http://hz.jlsjyb.cn/gtsnrbyqio.html

[D12] 查找元素下标
来源：http://hz.ydjk.org.cn/gtffaxsfwi.html

Py:   arr.index(x);  x in arr
来源：http://hz.gaohongyu789.top/gtlkxvrebz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.pycfn.com/gtqlupoycp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hongshengwenyu.top/gtiginkhsr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daxiang520.top/gtgsbiywpy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.vqdsnc.cn/gttrymbbkp.html

Go:   slices.Index(arr, x)
来源：http://hz.svipenyu.cn/gtitmogfmt.html

Ruby: arr.index(x)
来源：http://hz.yj20258888.top/gtdndgukzf.html

C#:   list.IndexOf(x);
来源：http://hz.cqqwz.cn/gtagpgahgh.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jiagoushi.top/gtujmnaqry.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xuetiantiany.cn/gtiduzeweu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.bjfxy.top/gteqqwkwjq.html

JS:   arr.filter(x => x > 3)
来源：http://hz.tian-w.cn/gtpuszwzwe.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yvedp.cn/gtvibmedcb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.haohaochexian.top/gtioahotcu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yuxming.cn/gtfufbbkwy.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shangyingyoupin.top/gtkyjebgas.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.tanke756.top/gtbrozigox.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xingfuxueyuan.xyz/gtdpbmkwep.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jlsjyb.cn/gtkitjoibq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gogol.net.cn/gtsvgaopul.html

JS:   arr.map(x => x * 2)
来源：http://hz.0kj1m.cn/gtqpprtzed.html

TS:   arr.map(x => x * 2)
来源：http://hz.xuanzx.com/gtbrscyaxl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.andypj.xyz/gtapxvkgmx.html

Go:   // 手写循环
来源：http://hz.havefunace.top/gtbiihmmuv.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.smart0.xyz/gtpmrignzt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.gaohongyu789.top/gtciztqrsg.html

[D15] 去重
来源：http://hz.tianlin.xyz/gtiwziwcgk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ydzc1.top/gteazeynpb.html

PHP:  array_unique($arr);
来源：http://hz.chenzaomai.com/gtyknnuiuv.html

JS:   [...new Set(arr)]
来源：http://hz.nwbrower.top/gtvpiedohk.html

TS:   [...new Set(arr)]
来源：http://hz.dianchejie.cn/gtrtgtzhtm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.daxiang520.top/gtqseqiuop.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhiwuduotai.top/gtateomsxg.html

Ruby: arr.uniq
来源：http://hz.yangfankeji.com/gtyjaoiwbc.html

C#:   list.Distinct().ToList()
来源：http://hz.zhiwuduotai.top/gtevnsjwui.html

[D16] 求和与平均值
来源：http://hz.52xcode.cn/gtpitzlsyn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.wangshuangyany.cn/gtldptdibq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.vqdsnc.cn/gteuwqipbw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aibaodan.cn/gtnzuiccku.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gogol.net.cn/gtiqncqqkh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.feifeiyinyue.top/gtarjwrbco.html

Go:   // 手写循环累加
来源：http://hz.cdnleiting.top/gtxdiahbvx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.svipenyu.cn/gtumlofoim.html

C#:   list.Sum();  list.Average()
来源：http://hz.chenjidiqi.icu/gtzaoocick.html

[D17] 最大值与最小值
来源：http://hz.hysaishi.cn/gtfjditike.html

Py:   max(arr);  min(arr)
来源：http://hz.yj20258888.top/gtipqdrgzu.html

PHP:  max($arr);  min($arr);
来源：http://hz.quarkkingdee.top/gtbaywaepj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hammf.cn/gtrskywnld.html

TS:   Math.max(...arr);
来源：http://hz.jinyuanbaomall.cn/gtjfoobzzo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.pycfn.com/gtyvzkiulm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ywan-chungtsiang.top/gtdbldlqae.html

Ruby: arr.max;  arr.min
来源：http://hz.sysykeji.top/gtemkqgkmz.html

C#:   list.Max();  list.Min()
来源：http://hz.sxryk.cn/gtxwqixsft.html

[D18] 扁平化嵌套数组
来源：http://hz.dianchejie.cn/gtsgnbfeqr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.redwolf501.top/gtqppfpdrq.html

PHP:  array_merge(...$nested);
来源：http://hz.zhongyouzk.top/gtggjpxvhw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.c1oappe.top/gtgchmwrmt.html

TS:   nested.flat();
来源：http://hz.hysaishi.cn/gtscvwhgfx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhongyouzk.top/gtbbfmavsv.html

Go:   // 手写双层循环
来源：http://hz.shangyingyoupin.top/gtqxczmolf.html

Ruby: nested.flatten
来源：http://hz.wangdashe.top/gtefmyrzox.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhoulong.xyz/gtracceume.html

[D19] 按字段分组
来源：http://hz.kuanghao11.cn/gtpphlgxsd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xziqi.cn/gttvqpgcvy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.fzhhl.top/gtaraftmou.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.0kj1m.cn/gtyfbdnozs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zycfv.cn/gtrhhfxkzp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yonumen.top/gtdlboxgge.html

Go:   // 手写 map[string][]T
来源：http://hz.smart0.xyz/gtwnnrrrqs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.c1oappe.top/gtqawhvnle.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ywan-chungtsiang.top/gtdaofqirp.html

[D20] 统计每个元素出现次数
来源：http://hz.pycfn.com/gtkxukpghd.html

Py:   Counter(arr)
来源：http://hz.jinqigufen.top/gtkatzthae.html

PHP:  array_count_values($arr);
来源：http://hz.jyoumei.cn/gtiapvigfh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.52xcode.cn/gtyyrjsynz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shuidangran.top/gtdrodtyeo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.tianlin.xyz/gtkbsdckti.html

Go:   // 手写 map[T]int
来源：http://hz.birdmap.top/gtxekkvsly.html

Ruby: arr.tally
来源：http://hz.pengpengdd.cyou/gtuqbdvzee.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.nwbrower.top/gtlgzxbdoc.html

[D21] 判断是否包含某元素
来源：http://hz.c1oappe.top/gtxjbatqby.html

Py:   x in arr
来源：http://hz.zhijiandao.cn/gtsbgteygb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hongshengwenyu.top/gtapcxtbxh.html

JS:   arr.includes(x)
来源：http://hz.hysaishi.cn/gtidzethdz.html

TS:   arr.includes(x)
来源：http://hz.zhongyouzk.top/gtzzujkhhr.html

Java: list.contains(x)
来源：http://hz.xziqi.cn/gtjkvbwzmy.html

Go:   slices.Contains(arr, x)
来源：http://hz.nanxinkj.top/gtssscpqer.html

Ruby: arr.include?(x)
来源：http://hz.yj202588.top/gtiyoxeggo.html

C#:   list.Contains(x)
来源：http://hz.shuidangran.top/gtdfhfvtgv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shangyingyoupin.top/gtfqynmbqh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhijiandao.cn/gtxuhzycov.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.svipenyu.cn/gtaweridjt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.aizwys.cn/gtuerzcmpd.html

TS:   [...arr];
来源：http://hz.sufxvd.cn/gtnnohxegm.html

Java: new ArrayList<>(list);
来源：http://hz.jlsjyb.cn/gthxwwkqgt.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yonumen.top/gtjvdmzrey.html

Ruby: arr.dup;  arr.clone
来源：http://hz.kuanghao11.cn/gtswwgtlbz.html

C#:   new List<int>(list);
来源：http://hz.zdqjudy.top/gtylahpdxd.html

[D23] reduce 累积计算
来源：http://hz.ppjwa.cn/gtierlqfth.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.316326.xyz/gtofxwwfdj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cqqwz.cn/gtswxriaub.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenlongwang.top/gtrzbpdtbs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xziqi.cn/gtaocenxbk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhengqikj.top/gtaynlwvqz.html

Go:   // 手写循环
来源：http://hz.zhongyouzk.top/gtiqmkbozw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.aizwys.cn/gtholtmvsl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.iojbl.cn/gtztwsnbcd.html

[D24] 字典 / Map 基本操作
来源：http://hz.ydjk.org.cn/gtzbfvkbrh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.meibo888.top/gtynvdlgiw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yonumen.top/gtjalgqvfb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gogol.net.cn/gtdoyrkojf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.dianchejie.cn/gthjvdrnct.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinyuanbaomall.cn/gtrqbnebza.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hnxiangtu.top/gtypxfxsnm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sweek.top/gtreokpfck.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yangfankeji.com/gtigytmkgs.html

[D25] Set 集合去重与交并差
来源：http://hz.pengpengdd.cyou/gtqqtaoezz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhiwuduotai.top/gtsiwxyukc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hywenlv.cn/gtisvyphzb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xinyue.icu/gtltxivysy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shzxlz.cn/gtammhaxmx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jyoumei.cn/gtnsvztpgf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zdqjudy.top/gtkfvcskkl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.chenlongwang.top/gtdegwjqbu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gaohongyu789.top/gttxccrjrs.html

[D26] 数组转字符串
来源：http://hz.zycfv.cn/gtloxpucgn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jinghuilouyu.cn/gtchfrvybh.html

PHP:  implode(", ", $arr);
来源：http://hz.iojbl.cn/gtskacvdar.html

JS:   arr.join(", ")
来源：http://hz.ppjwa.cn/gthbthfsfo.html

TS:   arr.join(", ")
来源：http://hz.yueranfly.top/gtiiavzyee.html

Java: String.join(", ", list)
来源：http://hz.aibaodan.cn/gtrrbizypa.html

Go:   strings.Join(strs, ", ")
来源：http://hz.sweek.top/gtkwtlnwde.html

Ruby: arr.join(", ")
来源：http://hz.pycfn.com/gtxquvglaf.html

C#:   string.Join(", ", list)
来源：http://hz.ppjwa.cn/gtfkpepjod.html

================================================================================
来源：http://hz.zhoulong.xyz/gtcmrermtu.html

E. 字符串处理
来源：http://hz.quarkkingdee.top/gtuouzdtvz.html

================================================================================
来源：http://hz.jlsjyb.cn/gttdgdybvu.html

[E01] 拼接字符串
来源：http://hz.guowangkeji.top/gtgrmzanmp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hnqzz.top/gtwumfliau.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.9152youxi.cn/gtkybcbhxh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258888.top/gtwoodlazj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sysykeji.top/gtakxykbpz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xuanzx.com/gtbtnfapqf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ydzc1.top/gtoomaupfo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.haohaochexian.top/gtlucjcrme.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hysaishi.cn/gtehgpoqet.html

[E02] 重复字符串
来源：http://hz.ydzc1.top/gtplrekhuq.html

Py:   "ab" * 3
来源：http://hz.gaohongyu789.top/gtigvapxqy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yueranfly.top/gtefymdvyj.html

JS:   "ab".repeat(3)
来源：http://hz.zhongyouzk.top/gtzjegibju.html

TS:   "ab".repeat(3)
来源：http://hz.tianlin.xyz/gtvvkjjegw.html

Java: "ab".repeat(3)
来源：http://hz.jianghu66.top/gthaaxlkfl.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhixingplan.top/gtgryihbpv.html

Ruby: "ab" * 3
来源：http://hz.chenjidiqi.icu/gtvvhwcpfg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xziqi.cn/gtpyycxzdy.html

[E03] 截取子串
来源：http://hz.xuanzx.com/gtlmszlucd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.c1oappe.top/gtujxvelfq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yanxiufei.cn/gtydxzlepx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.dashuyun.cn/gtatggxqqg.html

TS:   s.slice(1, 4)
来源：http://hz.yj20258888.top/gtgzwepmhe.html

Java: s.substring(1, 4)
来源：http://hz.hammf.cn/gtibyczjpn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.iojbl.cn/gtcyqousys.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xinyue.icu/gtipynzspq.html

C#:   s.Substring(1, 3)
来源：http://hz.xuetiantiany.cn/gtpcwjcead.html

[E04] 查找子串位置
来源：http://hz.yonumen.top/gtbfmsczyy.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jianghu66.top/gtjrzjrrek.html

PHP:  strpos($s, "x");
来源：http://hz.c1oappe.top/gtbhlnhdcq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.kuanghao11.cn/gtrbdjunmw.html

TS:   s.indexOf("x")
来源：http://hz.xziqi.cn/gtpmiyeuuy.html

Java: s.indexOf("x")
来源：http://hz.tian-w.cn/gtuqntrumw.html

Go:   strings.Index(s, "x")
来源：http://hz.yj20258.top/gtnaprlaow.html

Ruby: s.index("x")
来源：http://hz.zhengqikj.top/gtndqxcjho.html

C#:   s.IndexOf("x")
来源：http://hz.gogol.net.cn/gtfynylawn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.daria6918.cn/gtxoaaijmj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hnqzz.top/gtspinclyz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hfpthk.cn/gtpdrsdwdm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hnqzz.top/gttsdbpzqy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.aibaodan.cn/gtictlarcg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jqgfzy.top/gtyxuoijzx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.dianchejie.cn/gtnvvxzwht.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shzxlz.cn/gtfefydukj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.redwolf501.top/gtwwrytslo.html

[E06] 替换子串
来源：http://hz.jinqigfzy.top/gtokrdbcai.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.fzhhl.top/gtsraqgayi.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.0kj1m.cn/gtzyjgldbk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.smart0.xyz/gtusomlxty.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtrblgrmyu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hnxiangtu.top/gtoniahwzc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yueranfly.top/gtbuazugyq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhoulong.xyz/gtzzqrpekf.html

C#:   s.Replace("a", "b")
来源：http://hz.52xcode.cn/gtoocjqbrw.html

[E07] 按分隔符拆分
来源：http://hz.xingfuxueyuan.xyz/gtjmkfthdt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ydjk.org.cn/gtdilaticp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cqqwz.cn/gtcgstiolu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yueranfly.top/gtmezadkki.html

TS:   s.split(",")
来源：http://hz.xuanzx.com/gtctsvqrkm.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jianghu66.top/gtszdfbxua.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.9152youxi.cn/gtnoisizem.html

Ruby: s.split(",");  s.split
来源：http://hz.aibaodan.cn/gtddmibklf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sysykeji.top/gthwyqebdp.html

[E08] 数组按分隔符合并
来源：http://hz.shuidangran.top/gtveclrerd.html

Py:   ",".join(items)
来源：http://hz.gzhubu.top/gtqrwizybs.html

PHP:  implode(",", $items);
来源：http://hz.hysaishi.cn/gtrprmxnxb.html

JS:   items.join(",")
来源：http://hz.yangfankeji.com/gtarnpncum.html

TS:   items.join(",")
来源：http://hz.xingfuxueyuan.xyz/gtzzisotpl.html

Java: String.join(",", items)
来源：http://hz.yangfankeji.com/gtbclyfuyd.html

Go:   strings.Join(items, ",")
来源：http://hz.jqgfzy.top/gtiduewsvk.html

Ruby: items.join(",")
来源：http://hz.52xcode.cn/gtcynpracx.html

C#:   string.Join(",", items)
来源：http://hz.ppjwa.cn/gtfakepwsv.html

[E09] 去除所有空白字符
来源：http://hz.kuanghao11.cn/gtjugcjszv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinyuanbaomall.cn/gtpmlrnwnd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.snrcjt.cn/gtorezsims.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangtech.top/gtwacrtybe.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yanxiufei.cn/gtrdozmjoa.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.feifeiyinyue.top/gtknobcmxr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sweek.top/gtuzqdqlfa.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.nwbrower.top/gtebhetpbn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.havefunace.top/gtsqpqwcuw.html

[E10] 左侧补零 / 定长填充
来源：http://hz.andypj.xyz/gtvbentpgp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jiagoushi.top/gtdmpmlnku.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.tianlin.xyz/gtadlxcejr.html

JS:   "7".padStart(3, "0")
来源：http://hz.kuanghao11.cn/gtvopflpjr.html

TS:   "7".padStart(3, "0")
来源：http://hz.ppjwa.cn/gtbjyixmjk.html

Java: String.format("%03d", 7)
来源：http://hz.ppjwa.cn/gtdrmddyqa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.vqdsnc.cn/gtwbqrfbcz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hnxiangtu.top/gtftjjlxph.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.fengsongda.top/gtduhtmqoi.html

[E11] 反转字符串
来源：http://hz.xuetiantiany.cn/gtyismwbin.html

Py:   s[::-1]
来源：http://hz.dianchejie.cn/gtnqhbrjmf.html

PHP:  strrev($s);
来源：http://hz.hnqzz.top/gtubuvfkej.html

JS:   [...s].reverse().join("")
来源：http://hz.guannengcc.top/gtzahhxnac.html

TS:   [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtqgcoidla.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.andypj.xyz/gtsftnzqio.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jinqigfzy.top/gtffkiuobc.html

Ruby: s.reverse
来源：http://hz.gzhubu.top/gtlovvwtjl.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.sxryk.cn/gtpjcdtmui.html

[E12] 统计某字符出现次数
来源：http://hz.iojbl.cn/gtbrtbwfhj.html

Py:   s.count("a")
来源：http://hz.sysykeji.top/gthozrnbwd.html

PHP:  substr_count($s, "a");
来源：http://hz.316326.xyz/gtucpvlztl.html

JS:   s.split("a").length - 1
来源：http://hz.xinyue.icu/gtnueecixe.html

TS:   s.split("a").length - 1
来源：http://hz.quarkkingdee.top/gtphomjcvm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.fzhhl.top/gtffbrokuc.html

Go:   strings.Count(s, "a")
来源：http://hz.dashuyun.cn/gtidvyljfq.html

Ruby: s.count("a")
来源：http://hz.chenzaomai.com/gtgyusggrk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhaomingkeji.xyz/gtbbplrpav.html

[E13] 逐字符遍历
来源：http://hz.hfpthk.cn/gtrdqreogb.html

Py:   for ch in s: print(ch)
来源：http://hz.tianlin.xyz/gtluzmrenc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.pengpengdd.cyou/gtvoevddio.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tanke756.top/gtolqppffs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.kuanghao11.cn/gtfoskimdr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.mhx1999.top/gtrlimzzpt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yanxiufei.cn/gtaqjapggo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shanyushiyangkeji.top/gtwpkdyhor.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jinghuilouyu.cn/gtpzzwzpbu.html

[E14] URL 编码与 Base64
来源：http://hz.jinqigfzy.top/gtiubtstut.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.aizwys.cn/gtlkpegqas.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yueranfly.top/gtgvzgcgwo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhongyouzk.top/gtqqotwjml.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.dianchejie.cn/gtwmghffxh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.c1oappe.top/gtzhtkxmnl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ivvv.top/gtyhywxtbr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhengqikj.top/gtjirjltqj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuanzx.com/gtzeddydem.html

[E15] HTML 转义 / 反转义
来源：http://hz.yj20258888.top/gtuuwysmvw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.gotoacloud.top/gtwbgrqedn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hongshengwenyu.top/gtoquhtely.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.chenlongwang.top/gtcuwgcgik.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.iojbl.cn/gtpgqoikii.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.haohaochexian.top/gtduqmibag.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.pengpengdd.cyou/gtqeldgisz.html


<!-- 参考信息 -->