代发 wailian999

TS:   arr.slice(1, 4);
来源：http://hz.ydjk.org.cn/gtvofpqlru.html

Java: list.subList(1, 4);
来源：http://hz.zhoulong.xyz/gtzezelqje.html

Go:   arr[1:4]
来源：http://hz.hfpthk.cn/gtfeaqzjej.html

Ruby: arr[1, 3]
来源：http://hz.hysaishi.cn/gtqtvcuuoo.html

C#:   list.GetRange(1, 3);
来源：http://hz.yvedp.cn/gtxcfimaij.html

[D08] 合并两个数组
来源：http://hz.hywenlv.cn/gtqejigboq.html

Py:   a + b;  a.extend(b)
来源：http://hz.birdmap.top/gtwwkyaedu.html

PHP:  array_merge($a, $b);
来源：http://hz.snrcjt.cn/gtymwscqzn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xuetiantiany.cn/gtybfpscbo.html

TS:   [...a, ...b];
来源：http://hz.daria6918.cn/gtujzquxja.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yuanzhike.top/gtabfacxqa.html

Go:   append(a, b...)
来源：http://hz.wangdashe.top/gtuqrxtsvn.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhixingplan.top/gtyuhbclzk.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenjidiqi.icu/gtqvmrzkyq.html

[D09] 排序（升序）
来源：http://hz.ydzc1.top/gtrjehebol.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jianghu66.top/gtskzxwerr.html

PHP:  sort($arr);
来源：http://hz.yj20258888.top/gtpszjmvsq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.chenjidiqi.icu/gtqyyvowdv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xuanzx.com/gtekszevno.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yuanzhike.top/gtstlhkwqx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gotoacloud.top/gtqhapowkv.html

Ruby: arr.sort
来源：http://hz.jyoumei.cn/gtnhjhmlzl.html

C#:   list.Sort();
来源：http://hz.0kj1m.cn/gtggxfgfjl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cashguo.top/gtrrfhslkx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jiagoushi.top/gtpgmxgoem.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.havefunace.top/gtcyjvjirm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daria6918.cn/gttabvojhh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gaohongyu789.top/gtdnysuyds.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hnqzz.top/gtpmxprigy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hnxiangtu.top/gtierexidm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.kuanghao11.cn/gtoemnvoju.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cashguo.top/gtmcetafpe.html

[D11] 反转数组
来源：http://hz.xylfe.cn/gtpubmiwmi.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.dianchejie.cn/gtewpyfrgs.html

PHP:  array_reverse($arr);
来源：http://hz.yongpay.top/gtkruchwce.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhaomingkeji.xyz/gtxnkfkaeb.html

TS:   [...arr].reverse();
来源：http://hz.sxryk.cn/gtzjljbphb.html

Java: Collections.reverse(list);
来源：http://hz.zdqjudy.top/gtedrqiosj.html

Go:   slices.Reverse(arr)
来源：http://hz.yvedp.cn/gtzjzyovcv.html

Ruby: arr.reverse
来源：http://hz.0kj1m.cn/gtdupffljb.html

C#:   list.Reverse();
来源：http://hz.ywan-chungtsiang.top/gtuustnfli.html

[D12] 查找元素下标
来源：http://hz.quarkkingdee.top/gtodyxmavr.html

Py:   arr.index(x);  x in arr
来源：http://hz.tanke756.top/gtlxodibyj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ywan-chungtsiang.top/gtndgdbmpv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhengqikj.top/gtwqzmhkzn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ywan-chungtsiang.top/gtdxxjaplc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ybcxt.top/gtbmynfgbw.html

Go:   slices.Index(arr, x)
来源：http://hz.ydzc1.top/gtadddnrnj.html

Ruby: arr.index(x)
来源：http://hz.zhiwuduotai.top/gtlvgrfylj.html

C#:   list.IndexOf(x);
来源：http://hz.ehwqpu.com/gtzwxixakj.html

[D13] 过滤（保留满足条件的）
来源：http://hz.sxryk.cn/gtpmqbqtmu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.smart0.xyz/gtumkafsfw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yueranfly.top/gthnlqoovb.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jianghu66.top/gtorcptvnf.html

TS:   arr.filter(x => x > 3)
来源：http://hz.nanxuanxn.top/gtkmdewdtq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhengqikj.top/gtsatjtpoy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ydjk.org.cn/gtarnsugma.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ivvv.top/gtgqffbbja.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhixingplan.top/gtihggmpvj.html

[D14] 映射转换（每个元素变形）
来源：http://hz.pycfn.com/gtixwpcuoj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.pycfn.com/gtkuoppjws.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yuanzhike.top/gtqpwbqrck.html

JS:   arr.map(x => x * 2)
来源：http://hz.mhx1999.top/gtragwekic.html

TS:   arr.map(x => x * 2)
来源：http://hz.tianlin.xyz/gtdxncljht.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.smart0.xyz/gtqvzkpzew.html

Go:   // 手写循环
来源：http://hz.guowangkeji.top/gtdedcxnqi.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.guannengcc.top/gtfhmagdxy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.havefunace.top/gtgsuitsls.html

[D15] 去重
来源：http://hz.hfpthk.cn/gtfhoorxiw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yuanzhike.top/gtxbydtrkg.html

PHP:  array_unique($arr);
来源：http://hz.chenzaomai.com/gtumdhakri.html

JS:   [...new Set(arr)]
来源：http://hz.zhixingplan.top/gtdszvpjwi.html

TS:   [...new Set(arr)]
来源：http://hz.c1oappe.top/gtaoewzbkh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hnxiangtu.top/gtoecjoplt.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.tanke756.top/gtcdpnwxpz.html

Ruby: arr.uniq
来源：http://hz.jinyuanbaomall.cn/gtldxxobhg.html

C#:   list.Distinct().ToList()
来源：http://hz.chenjidiqi.icu/gtexzohcma.html

[D16] 求和与平均值
来源：http://hz.jlsjyb.cn/gtqpovynxm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yj20258888.top/gtlczzlyut.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nanxuanxn.top/gtsbocticu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.vqdsnc.cn/gtmrvpvjqz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nwbrower.top/gtghyglamd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ydzc1.top/gtfhyacesh.html

Go:   // 手写循环累加
来源：http://hz.daxiang520.top/gtfltcskiv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hfpthk.cn/gtzktmqykp.html

C#:   list.Sum();  list.Average()
来源：http://hz.sufxvd.cn/gtlispnxks.html

[D17] 最大值与最小值
来源：http://hz.gaohongyu789.top/gtmplzzmsy.html

Py:   max(arr);  min(arr)
来源：http://hz.fzhhl.top/gtwxmbgwdr.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhongyouzk.top/gtgjuqqlpb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.guannengcc.top/gtbojnqxzp.html

TS:   Math.max(...arr);
来源：http://hz.yj20258.top/gtifydubrk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.guannengcc.top/gtwuofdyzl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.quarkkingdee.top/gtjmscktch.html

Ruby: arr.max;  arr.min
来源：http://hz.daria6918.cn/gttsjomczh.html

C#:   list.Max();  list.Min()
来源：http://hz.gotoacloud.top/gtsdcpzvfo.html

[D18] 扁平化嵌套数组
来源：http://hz.sysykeji.top/gtnesxvvma.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.wangshuangyany.cn/gtxoobevjl.html

PHP:  array_merge(...$nested);
来源：http://hz.haohaochexian.top/gtpsvlsydz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhaomingkeji.xyz/gtzqvpzwjx.html

TS:   nested.flat();
来源：http://hz.jqgfzy.top/gtsuzipnyo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hnqzz.top/gthkegbnxr.html

Go:   // 手写双层循环
来源：http://hz.yuxming.cn/gtockeanwj.html

Ruby: nested.flatten
来源：http://hz.nwbrower.top/gtnwtzhrbi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.redwolf501.top/gthlchelag.html

[D19] 按字段分组
来源：http://hz.snrcjt.cn/gttlrckutf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shanyushiyangkeji.top/gtirvqcojt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.c1oappe.top/gtbdhnmxfl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gzhubu.top/gthmlypcbv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.guowangkeji.top/gtozdxtiya.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cashguo.top/gtbictnnhu.html

Go:   // 手写 map[string][]T
来源：http://hz.yueranfly.top/gtsxsaevkn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.vqdsnc.cn/gtfmnqtcid.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.smart0.xyz/gtvlgwjlel.html

[D20] 统计每个元素出现次数
来源：http://hz.jianghu66.top/gtfczouxpd.html

Py:   Counter(arr)
来源：http://hz.gzhubu.top/gtqnvrdgxb.html

PHP:  array_count_values($arr);
来源：http://hz.gotoacloud.top/gtjgzktemf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yanxiufei.cn/gtdxarxalh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenzaomai.com/gtwpctpbta.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.chenzaomai.com/gtqqspurkb.html

Go:   // 手写 map[T]int
来源：http://hz.shanyushiyangtech.top/gtzeqhgyly.html

Ruby: arr.tally
来源：http://hz.ppjwa.cn/gtpulhccwv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ppjwa.cn/gtkjsvevse.html

[D21] 判断是否包含某元素
来源：http://hz.aizwys.cn/gtxishjgox.html

Py:   x in arr
来源：http://hz.shzxlz.cn/gtgrqdevwx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ywan-chungtsiang.top/gtnxydegic.html

JS:   arr.includes(x)
来源：http://hz.snrcjt.cn/gtlwoljrxn.html

TS:   arr.includes(x)
来源：http://hz.jinghuilouyu.cn/gtxchxwdul.html

Java: list.contains(x)
来源：http://hz.jyoumei.cn/gtkriwlhlh.html

Go:   slices.Contains(arr, x)
来源：http://hz.aibaodan.cn/gtdvdadwye.html

Ruby: arr.include?(x)
来源：http://hz.9152youxi.cn/gtjrawxdji.html

C#:   list.Contains(x)
来源：http://hz.tianlin.xyz/gtoekmaoyt.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hfpthk.cn/gtnojjsexr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.sysykeji.top/gtnvxomcfe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tianlin.xyz/gtofonutuw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ppjwa.cn/gtduumriwp.html

TS:   [...arr];
来源：http://hz.meibo888.top/gtmvzwbsrr.html

Java: new ArrayList<>(list);
来源：http://hz.zhixingplan.top/gtrkiiczjo.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.aizwys.cn/gtfuxxkwtl.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hysaishi.cn/gtdptwfkro.html

C#:   new List<int>(list);
来源：http://hz.havefunace.top/gtejycqpzg.html

[D23] reduce 累积计算
来源：http://hz.feifeiyinyue.top/gtdqhvxljy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.gaohongyu789.top/gtcvbdsprr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhijiandao.cn/gtccdwfnzk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cqqwz.cn/gtmxmcbdcd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jyoumei.cn/gtchedqqqq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tianlin.xyz/gtnuynkhqz.html

Go:   // 手写循环
来源：http://hz.nanxuanxn.top/gtdbdhowxk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ppjwa.cn/gtndrngbxn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yj202588.top/gtpmrxuqhe.html

[D24] 字典 / Map 基本操作
来源：http://hz.chenzaomai.com/gtlmkezzat.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.haohaochexian.top/gtamfatxlz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.chenzaomai.com/gtrsgaqzmt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zycfv.cn/gtgqygnshm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zdqjudy.top/gtafgtawee.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhiwuduotai.top/gtvjscpntl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cheryme.top/gtfwxhnxix.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shuidangran.top/gtocdlhcsf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yuanzhike.top/gttuyvrgdr.html

[D25] Set 集合去重与交并差
来源：http://hz.zhongyouzk.top/gtjjztdewq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yj20258888.top/gtqeibpgra.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hammf.cn/gtigfinzni.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.guannengcc.top/gthpazvqzh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yanxiufei.cn/gtmqufyrba.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yvedp.cn/gtpbopdcjm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.dianchejie.cn/gtqzewbeda.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.svipenyu.cn/gtjciblowv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xylfe.cn/gtrxiayiki.html

[D26] 数组转字符串
来源：http://hz.ybcxt.top/gtnygppquj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cqqwz.cn/gtcddzkafv.html

PHP:  implode(", ", $arr);
来源：http://hz.chenlongwang.top/gtkptayrwp.html

JS:   arr.join(", ")
来源：http://hz.chenjidiqi.icu/gtrmhrjnai.html

TS:   arr.join(", ")
来源：http://hz.zdqjudy.top/gtwyzrzfnq.html

Java: String.join(", ", list)
来源：http://hz.hysaishi.cn/gtkcoakpix.html

Go:   strings.Join(strs, ", ")
来源：http://hz.wangshuangyany.cn/gtnixiyojb.html

Ruby: arr.join(", ")
来源：http://hz.zhoulong.xyz/gtbjednflp.html

C#:   string.Join(", ", list)
来源：http://hz.shuidangran.top/gtuacahles.html

================================================================================
来源：http://hz.kuanghao11.cn/gtvolxhdfs.html

E. 字符串处理
来源：http://hz.shangyingyoupin.top/gtsvdgwcvd.html

================================================================================
来源：http://hz.guowangkeji.top/gtilbouljl.html

[E01] 拼接字符串
来源：http://hz.ehwqpu.com/gtxrxkqubx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinghuilouyu.cn/gtvzytwxxg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.sweek.top/gtobrqskcp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnqzz.top/gtkydbzwmd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xylfe.cn/gtwvzokgef.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yanxiufei.cn/gtxtittbyl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xuanzx.com/gthrwqcinm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hnqzz.top/gtfsgctcot.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.birdmap.top/gthbryyvyb.html

[E02] 重复字符串
来源：http://hz.meibo888.top/gtpesdtoex.html

Py:   "ab" * 3
来源：http://hz.wangshuangyany.cn/gtuoybpmze.html

PHP:  str_repeat("ab", 3);
来源：http://hz.meibo888.top/gtnwrnzpjo.html

JS:   "ab".repeat(3)
来源：http://hz.shzxlz.cn/gthtymttbu.html

TS:   "ab".repeat(3)
来源：http://hz.cucudq.cn/gtnfvdxcjf.html

Java: "ab".repeat(3)
来源：http://hz.zhengqikj.top/gtpnnrmkjj.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.fzhhl.top/gtxgmhdpjo.html

Ruby: "ab" * 3
来源：http://hz.hysaishi.cn/gtizbbqigs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.andypj.xyz/gtrhhcldmm.html

[E03] 截取子串
来源：http://hz.cashguo.top/gtfdqgsjkl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yuanzhike.top/gtrvtyitwo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yj20258.top/gtfjayrtpi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jlsjyb.cn/gtaiwshbhv.html

TS:   s.slice(1, 4)
来源：http://hz.yvedp.cn/gtwcdkrsoy.html

Java: s.substring(1, 4)
来源：http://hz.hysaishi.cn/gtnrozxbro.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xylfe.cn/gtkxzafbjs.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.iojbl.cn/gtfnuiapco.html

C#:   s.Substring(1, 3)
来源：http://hz.jinyuanbaomall.cn/gtsesmfqus.html

[E04] 查找子串位置
来源：http://hz.fzhhl.top/gtafrysaap.html

Py:   s.find("x");  s.index("x")
来源：http://hz.smart0.xyz/gtrkqjwylk.html

PHP:  strpos($s, "x");
来源：http://hz.fengsongda.top/gtpdwkojlc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jqgufenzy.top/gtoscepwfq.html

TS:   s.indexOf("x")
来源：http://hz.sysykeji.top/gtgssmkhzn.html

Java: s.indexOf("x")
来源：http://hz.chenjidiqi.icu/gtaevaydkp.html

Go:   strings.Index(s, "x")
来源：http://hz.sxryk.cn/gtwhjusuyp.html

Ruby: s.index("x")
来源：http://hz.nwbrower.top/gtocbumjfu.html

C#:   s.IndexOf("x")
来源：http://hz.zhijiandao.cn/gtuoylayzc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.birdmap.top/gtksxpeszn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.haohaochexian.top/gtenbcpsjf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.guannengcc.top/gttvdjagie.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yueranfly.top/gtrtugylqo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.guannengcc.top/gtiusqopwa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinyuanbaomall.cn/gterxkkuso.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.sxryk.cn/gtuhjpzqeq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hnqzz.top/gtsgrlickh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.dianchejie.cn/gtignbzqwk.html

[E06] 替换子串
来源：http://hz.xuetiantiany.cn/gtjazqutgd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yuanzhike.top/gtgvwxzhnn.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hnxiangtu.top/gttevmissr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258888.top/gtypqynlmx.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtpaxwzfzc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuetiantiany.cn/gtsphohcbb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cheryme.top/gtcbbnxezt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtlqgxvhyh.html

C#:   s.Replace("a", "b")
来源：http://hz.xylfe.cn/gtygarkejx.html

[E07] 按分隔符拆分
来源：http://hz.cheryme.top/gtgxylhsin.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.daxiang520.top/gtkwrvouec.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xuanzx.com/gtgqwqsqdq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xuetiantiany.cn/gtqkpmjmbi.html

TS:   s.split(",")
来源：http://hz.dashuyun.cn/gtlqccgkuw.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jyoumei.cn/gtgrdezpxi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.tian-w.cn/gtfuziyclp.html

Ruby: s.split(",");  s.split
来源：http://hz.sufxvd.cn/gtvvgvufci.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gzhubu.top/gtqifpxjss.html

[E08] 数组按分隔符合并
来源：http://hz.shuidangran.top/gtyqzhzpzj.html

Py:   ",".join(items)
来源：http://hz.gogol.net.cn/gtuuyonruc.html

PHP:  implode(",", $items);
来源：http://hz.shanyushiyangkeji.top/gtdyzmkdmo.html

JS:   items.join(",")
来源：http://hz.wangshuangyany.cn/gtnleiholq.html

TS:   items.join(",")
来源：http://hz.sysykeji.top/gtnjhamdaz.html

Java: String.join(",", items)
来源：http://hz.jinqigufen.top/gtizvyawsd.html

Go:   strings.Join(items, ",")
来源：http://hz.nanxinkj.top/gtuczexbsx.html

Ruby: items.join(",")
来源：http://hz.haohaochexian.top/gtpflrylyw.html

C#:   string.Join(",", items)
来源：http://hz.yanxiufei.cn/gtsmzlhvep.html

[E09] 去除所有空白字符
来源：http://hz.ybcxt.top/gtswuikvkz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhaomingkeji.xyz/gtlqswmehr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hnxiangtu.top/gtzcaofalh.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.mhx1999.top/gtojdlgtwg.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhengqikj.top/gtcuebnmsl.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinqigfzy.top/gtbqzkcrlj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.havefunace.top/gtsofajgnn.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.birdmap.top/gtjgtiewld.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sysykeji.top/gtpgqktosy.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xziqi.cn/gtyovmnwdh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yj20258.top/gtlgfbnvdi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhengqikj.top/gtjarmynau.html

JS:   "7".padStart(3, "0")
来源：http://hz.xinyue.icu/gtbltxioua.html

TS:   "7".padStart(3, "0")
来源：http://hz.jinghuilouyu.cn/gtfcpnlljn.html

Java: String.format("%03d", 7)
来源：http://hz.cucudq.cn/gtllmqyftt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ivvv.top/gtsqyxffpv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gtsvifonte.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.fengsongda.top/gtxlubbxnf.html

[E11] 反转字符串
来源：http://hz.bjfxy.top/gtoblfdged.html

Py:   s[::-1]
来源：http://hz.nwbrower.top/gtvsujgzgt.html

PHP:  strrev($s);
来源：http://hz.shanyushiyangkeji.top/gtnuonsjmr.html

JS:   [...s].reverse().join("")
来源：http://hz.havefunace.top/gtgndmdxzo.html

TS:   [...s].reverse().join("")
来源：http://hz.0kj1m.cn/gtfgvicumf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.iojbl.cn/gtmfhmqedc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhiwuduotai.top/gtgpxpqkll.html

Ruby: s.reverse
来源：http://hz.zhengqikj.top/gtoxkjomdm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.smart0.xyz/gtcywapbqb.html

[E12] 统计某字符出现次数
来源：http://hz.cheryme.top/gtonuwedqw.html

Py:   s.count("a")
来源：http://hz.andypj.xyz/gttgdcuvgh.html

PHP:  substr_count($s, "a");
来源：http://hz.bjfxy.top/gtjlxokctx.html

JS:   s.split("a").length - 1
来源：http://hz.meibo888.top/gtmabjvkpp.html

TS:   s.split("a").length - 1
来源：http://hz.tanke756.top/gtobbaqhrr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hywenlv.cn/gtdfnfxgrp.html

Go:   strings.Count(s, "a")
来源：http://hz.jqgfzy.top/gticarkiza.html

Ruby: s.count("a")
来源：http://hz.jlsjyb.cn/gtgettzlnn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinyuanbaomall.cn/gteijrpgje.html

[E13] 逐字符遍历
来源：http://hz.gogol.net.cn/gtybugglqm.html

Py:   for ch in s: print(ch)
来源：http://hz.shuidangran.top/gtlqipatek.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.c1oappe.top/gtsuutfcqb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sweek.top/gtovfxiyfw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ehwqpu.com/gtubixpqqt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jyoumei.cn/gtuytfvzot.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jqgufenzy.top/gtsxjoybze.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.sufxvd.cn/gtgmmvdnwy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jqgfzy.top/gtvwejusmu.html

[E14] URL 编码与 Base64
来源：http://hz.hnqzz.top/gtxpjwvxek.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.316326.xyz/gtfiiqhkqj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jiagoushi.top/gtgkvwhozz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.chenzaomai.com/gtyjtccelp.html


<!-- 参考信息 -->