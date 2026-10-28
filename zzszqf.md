代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xylfe.cn/gtidpohpfd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.smart0.xyz/gtyyjzocbv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ywan-chungtsiang.top/gtyordcaup.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.sufxvd.cn/gtcbfuueja.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gtxanninqh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tian-w.cn/gtgblyvnfh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xinyue.icu/gtssiujjfq.html

[D06] 数组长度
来源：http://hz.feifeiyinyue.top/gtmmwgubee.html

Py:   len(arr)
来源：http://hz.pycfn.com/gtldbanhgj.html

PHP:  count($arr);
来源：http://hz.xingfuxueyuan.xyz/gtnumxgidb.html

JS:   arr.length
来源：http://hz.vqdsnc.cn/gtqbnrhmzi.html

TS:   arr.length
来源：http://hz.redwolf501.top/gtiwodmnys.html

Java: list.size();
来源：http://hz.zhixingplan.top/gtoyqcbjzf.html

Go:   len(arr)
来源：http://hz.quarkkingdee.top/gtixpjqmpe.html

Ruby: arr.length; arr.size
来源：http://hz.bjfxy.top/gtlrtyhcuc.html

C#:   list.Count;
来源：http://hz.sxryk.cn/gtanqksdad.html

[D07] 切片 / 取子数组
来源：http://hz.jqgufenzy.top/gtrewhfeci.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yueranfly.top/gtcdenrmfu.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.9152youxi.cn/gtpmjiricy.html

JS:   arr.slice(1, 4);
来源：http://hz.zhengqikj.top/gtbqzfeeoh.html

TS:   arr.slice(1, 4);
来源：http://hz.wangshuangyany.cn/gtlgjnyhsi.html

Java: list.subList(1, 4);
来源：http://hz.shanyushiyangtech.top/gtilxvojjf.html

Go:   arr[1:4]
来源：http://hz.nanxuanxn.top/gtyebrrjms.html

Ruby: arr[1, 3]
来源：http://hz.snrcjt.cn/gtqutnxonc.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj202588.top/gtojhausng.html

[D08] 合并两个数组
来源：http://hz.havefunace.top/gtwpsspqds.html

Py:   a + b;  a.extend(b)
来源：http://hz.sxryk.cn/gtxrgdfryt.html

PHP:  array_merge($a, $b);
来源：http://hz.cheryme.top/gtfvspbdhc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yj20258888.top/gtpxcisrbi.html

TS:   [...a, ...b];
来源：http://hz.ydzc1.top/gtfvkiwxau.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ybcxt.top/gtaybtkavf.html

Go:   append(a, b...)
来源：http://hz.daxiang520.top/gtbzptgruv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xinyue.icu/gtlxhhfxcj.html

C#:   a.Concat(b).ToList()
来源：http://hz.daxiang520.top/gtrfrxoabf.html

[D09] 排序（升序）
来源：http://hz.shzxlz.cn/gtzmpeskee.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhijiandao.cn/gtvfkxwuea.html

PHP:  sort($arr);
来源：http://hz.guowangkeji.top/gtrwoxprol.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.tianlin.xyz/gtxzdngnur.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xingfuxueyuan.xyz/gtlblfantf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yvedp.cn/gtqlhokton.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gzhubu.top/gtvzxzqkoe.html

Ruby: arr.sort
来源：http://hz.pengpengdd.cyou/gtlarjucdl.html

C#:   list.Sort();
来源：http://hz.sxryk.cn/gtfbwrcsmm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jlsjyb.cn/gtwmchmqwa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.shzxlz.cn/gtiyxindps.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yueranfly.top/gtnusmlmcq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.haohaochexian.top/gtumtsoprh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhijiandao.cn/gtycynqean.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.nanxuanxn.top/gtmchkmhhd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.aizwys.cn/gtfqpspnji.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hnqzz.top/gtecbimzyj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yj202588.top/gtxkosjhjy.html

[D11] 反转数组
来源：http://hz.havefunace.top/gtrmojksic.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jqgfzy.top/gttqwwryeh.html

PHP:  array_reverse($arr);
来源：http://hz.redwolf501.top/gtelnkxuzu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.pycfn.com/gtklzteoyu.html

TS:   [...arr].reverse();
来源：http://hz.wangshuangyany.cn/gtjmyewwld.html

Java: Collections.reverse(list);
来源：http://hz.aizwys.cn/gtejldgyzu.html

Go:   slices.Reverse(arr)
来源：http://hz.zhaomingkeji.xyz/gtoxjwfcxe.html

Ruby: arr.reverse
来源：http://hz.nanxinkj.top/gtstkmqqig.html

C#:   list.Reverse();
来源：http://hz.ivvv.top/gtjdizhvpi.html

[D12] 查找元素下标
来源：http://hz.hongshengwenyu.top/gtuxxxynld.html

Py:   arr.index(x);  x in arr
来源：http://hz.pycfn.com/gtakjrupwq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.sysykeji.top/gtuftzcpvr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shuidangran.top/gtmcktfzlx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.bjfxy.top/gtrvfnmeid.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.aibaodan.cn/gtnidblmnf.html

Go:   slices.Index(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtsasnedvw.html

Ruby: arr.index(x)
来源：http://hz.jqgufenzy.top/gtlzzpacqt.html

C#:   list.IndexOf(x);
来源：http://hz.yueranfly.top/gtencziwqw.html

[D13] 过滤（保留满足条件的）
来源：http://hz.shanyushiyangtech.top/gtaaphxoso.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xuetiantiany.cn/gtsovhlngh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jyoumei.cn/gtzithofrh.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ehwqpu.com/gtdaetgorv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.snrcjt.cn/gtddlidtej.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hysaishi.cn/gtipelvlsi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.aibaodan.cn/gtkisdgywk.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.pycfn.com/gtswjvygrl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.gotoacloud.top/gtufcglmzn.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yanxiufei.cn/gttxogclpr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.andypj.xyz/gtdxtxmvvo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.chenlongwang.top/gtpirvlqaf.html

JS:   arr.map(x => x * 2)
来源：http://hz.fzhhl.top/gtydnzvkzr.html

TS:   arr.map(x => x * 2)
来源：http://hz.wangdashe.top/gtxcvyqjdq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hywenlv.cn/gtvczvwmjv.html

Go:   // 手写循环
来源：http://hz.kuanghao11.cn/gtorehyneb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.tianlin.xyz/gtpxqwagmd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xingfuxueyuan.xyz/gtwydhznjq.html

[D15] 去重
来源：http://hz.kuanghao11.cn/gtnrfcrqgz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.haohaochexian.top/gtzlwvgxlo.html

PHP:  array_unique($arr);
来源：http://hz.kuanghao11.cn/gtmzlbytmz.html

JS:   [...new Set(arr)]
来源：http://hz.kuanghao11.cn/gtmoxbggxl.html

TS:   [...new Set(arr)]
来源：http://hz.cucudq.cn/gtpdfcdrme.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hfpthk.cn/gtgbfouuit.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.fengsongda.top/gtwpjmpjhf.html

Ruby: arr.uniq
来源：http://hz.daxiang520.top/gtaqlkrgqf.html

C#:   list.Distinct().ToList()
来源：http://hz.feifeiyinyue.top/gtctabbylg.html

[D16] 求和与平均值
来源：http://hz.ydzc1.top/gtrknnburn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hongshengwenyu.top/gtulhsrnfu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.snrcjt.cn/gtghejsoct.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shanyushiyangkeji.top/gtfisifrap.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ehwqpu.com/gtvlotsqmm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.nwbrower.top/gtczhanmyn.html

Go:   // 手写循环累加
来源：http://hz.0kj1m.cn/gtuuacyoyf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhaomingkeji.xyz/gteypgxwqu.html

C#:   list.Sum();  list.Average()
来源：http://hz.fzhhl.top/gtiozpsaib.html

[D17] 最大值与最小值
来源：http://hz.pengpengdd.cyou/gtbuweumyw.html

Py:   max(arr);  min(arr)
来源：http://hz.guowangkeji.top/gtyaofbory.html

PHP:  max($arr);  min($arr);
来源：http://hz.gogol.net.cn/gtklhwpzaa.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shzxlz.cn/gtliajvwkh.html

TS:   Math.max(...arr);
来源：http://hz.0kj1m.cn/gtmjrzkkhn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.bjfxy.top/gtihbjlbjb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.guowangkeji.top/gtmykmkigy.html

Ruby: arr.max;  arr.min
来源：http://hz.tanke756.top/gtmubbltsj.html

C#:   list.Max();  list.Min()
来源：http://hz.guowangkeji.top/gtfsjmjgzo.html

[D18] 扁平化嵌套数组
来源：http://hz.nanxuanxn.top/gtahnsemit.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sweek.top/gtticykigy.html

PHP:  array_merge(...$nested);
来源：http://hz.xingfuxueyuan.xyz/gtvigujlyf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhaomingkeji.xyz/gtwjmmsevw.html

TS:   nested.flat();
来源：http://hz.quarkkingdee.top/gtnzajhkja.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ivvv.top/gtyoonmnjo.html

Go:   // 手写双层循环
来源：http://hz.hammf.cn/gtoiuxttoh.html

Ruby: nested.flatten
来源：http://hz.jyoumei.cn/gtpbzmqhin.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ydjk.org.cn/gtiywjwibb.html

[D19] 按字段分组
来源：http://hz.yj202588.top/gtbdkhagpe.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.dashuyun.cn/gtoczghbzp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj20258.top/gtydhokbdn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhengqikj.top/gtvvjczteq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gaohongyu789.top/gtbdfxqntz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ydzc1.top/gtkabruhkj.html

Go:   // 手写 map[string][]T
来源：http://hz.hywenlv.cn/gteuprumsr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.tanke756.top/gtyiltoyil.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ehwqpu.com/gtdvikqtsf.html

[D20] 统计每个元素出现次数
来源：http://hz.meibo888.top/gtclfbhcth.html

Py:   Counter(arr)
来源：http://hz.jinyuanbaomall.cn/gttyuigptd.html

PHP:  array_count_values($arr);
来源：http://hz.xziqi.cn/gtpciuibay.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhoulong.xyz/gtwuftsfir.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangdashe.top/gtjvtaqtcw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shzxlz.cn/gtltbuftit.html

Go:   // 手写 map[T]int
来源：http://hz.chenlongwang.top/gtthcrkczy.html

Ruby: arr.tally
来源：http://hz.gzhubu.top/gtzvrnjvbk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.wangdashe.top/gtnsiafkwg.html

[D21] 判断是否包含某元素
来源：http://hz.ehwqpu.com/gtndeenjra.html

Py:   x in arr
来源：http://hz.yuanzhike.top/gtbtmsghdd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.9152youxi.cn/gthsabtpog.html

JS:   arr.includes(x)
来源：http://hz.haohaochexian.top/gtdtfricxw.html

TS:   arr.includes(x)
来源：http://hz.jqgfzy.top/gturkfuufr.html

Java: list.contains(x)
来源：http://hz.yueranfly.top/gtnuieigxm.html

Go:   slices.Contains(arr, x)
来源：http://hz.nwbrower.top/gtmshgichq.html

Ruby: arr.include?(x)
来源：http://hz.birdmap.top/gtkdylsfym.html

C#:   list.Contains(x)
来源：http://hz.316326.xyz/gtszjzzscm.html

[D22] 复制数组（避免共享引用）
来源：http://hz.aizwys.cn/gtzhkqumwx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.kuanghao11.cn/gthyjdjtpb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.bjfxy.top/gtkajgrefa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hongshengwenyu.top/gtlocnczki.html

TS:   [...arr];
来源：http://hz.ywan-chungtsiang.top/gtralxjqtk.html

Java: new ArrayList<>(list);
来源：http://hz.jinyuanbaomall.cn/gtirjfqyrs.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ydjk.org.cn/gtnpjgtpuz.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xuanzx.com/gtxsaegwjy.html

C#:   new List<int>(list);
来源：http://hz.xylfe.cn/gtjhdirzsi.html

[D23] reduce 累积计算
来源：http://hz.daxiang520.top/gtytabkzph.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.aibaodan.cn/gtcixizqkq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.birdmap.top/gtrksdewzk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydzc1.top/gtoiioyvgj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gzhubu.top/gtwxmctdjm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.daria6918.cn/gtohwywayc.html

Go:   // 手写循环
来源：http://hz.c1oappe.top/gtrqernekn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.nwbrower.top/gtivemwxae.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.daria6918.cn/gtqqlprzdh.html

[D24] 字典 / Map 基本操作
来源：http://hz.aizwys.cn/gticqcvjcc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.daxiang520.top/gteinsqptl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.chenjidiqi.icu/gtbqmielif.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhixingplan.top/gtvaiqjzux.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hongshengwenyu.top/gthevhuzgd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xuanzx.com/gtkdauvrrp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yangfankeji.com/gtlxvgmdnx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sxryk.cn/gtolzhrcez.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.snrcjt.cn/gtjzwbanzk.html

[D25] Set 集合去重与交并差
来源：http://hz.fzhhl.top/gtqqxwblrq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.9152youxi.cn/gteonuhffy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jlsjyb.cn/gtunwjbqws.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.quarkkingdee.top/gthgndezle.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jlsjyb.cn/gtryjnylpo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hnqzz.top/gtxszosxxo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hammf.cn/gtwblueniz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.wangshuangyany.cn/gteaarzacd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sweek.top/gtahhcufst.html

[D26] 数组转字符串
来源：http://hz.birdmap.top/gtlkddxbjp.html

Py:   ", ".join(map(str, arr))
来源：http://hz.9152youxi.cn/gtopnnylvj.html

PHP:  implode(", ", $arr);
来源：http://hz.yuanzhike.top/gtvpviqwbk.html

JS:   arr.join(", ")
来源：http://hz.gaohongyu789.top/gtjipayjgd.html

TS:   arr.join(", ")
来源：http://hz.52xcode.cn/gtmchydnzq.html

Java: String.join(", ", list)
来源：http://hz.redwolf501.top/gtphdleqmx.html

Go:   strings.Join(strs, ", ")
来源：http://hz.shanyushiyangkeji.top/gtlsviiumx.html

Ruby: arr.join(", ")
来源：http://hz.gogol.net.cn/gtncrabnra.html

C#:   string.Join(", ", list)
来源：http://hz.cucudq.cn/gthqjyzalb.html

================================================================================
来源：http://hz.meibo888.top/gtvdlusged.html

E. 字符串处理
来源：http://hz.xinyue.icu/gtyzvfpphr.html

================================================================================
来源：http://hz.ydjk.org.cn/gtwawigmut.html

[E01] 拼接字符串
来源：http://hz.pengpengdd.cyou/gtxgydvelh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ybcxt.top/gtnpxnqysb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.meibo888.top/gtonbvttex.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jyoumei.cn/gtalewdoun.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnxiangtu.top/gtjckibkao.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.dashuyun.cn/gtlvompqhm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.quarkkingdee.top/gtvrqqtlrp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhijiandao.cn/gtxoxbujof.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.fengsongda.top/gtqgsoeaxg.html

[E02] 重复字符串
来源：http://hz.zdqjudy.top/gtjqtzfqzi.html

Py:   "ab" * 3
来源：http://hz.chenzaomai.com/gttstlhzvu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xylfe.cn/gtjsryswff.html

JS:   "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtlshfhofi.html

TS:   "ab".repeat(3)
来源：http://hz.quarkkingdee.top/gtfjpprekc.html

Java: "ab".repeat(3)
来源：http://hz.yj20258.top/gtexjzubzm.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.aibaodan.cn/gtwcmznlxh.html

Ruby: "ab" * 3
来源：http://hz.zycfv.cn/gtxmiskvvi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yuxming.cn/gtrzupqedy.html

[E03] 截取子串
来源：http://hz.dianchejie.cn/gtaaawyuol.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hammf.cn/gtclsnwynr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yj20258.top/gtayvppecb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shuidangran.top/gtvqvhywzi.html

TS:   s.slice(1, 4)
来源：http://hz.yueranfly.top/gtcuaaksud.html

Java: s.substring(1, 4)
来源：http://hz.kuanghao11.cn/gtrsjurzjo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.nanxuanxn.top/gtkltputsd.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jiagoushi.top/gtbijrbhgi.html

C#:   s.Substring(1, 3)
来源：http://hz.jianghu66.top/gtkyjudhre.html

[E04] 查找子串位置
来源：http://hz.svipenyu.cn/gtlqlzhbjc.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ywan-chungtsiang.top/gtmmuafang.html

PHP:  strpos($s, "x");
来源：http://hz.jinghuilouyu.cn/gtoddlljba.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.tian-w.cn/gtzwrbnilq.html

TS:   s.indexOf("x")
来源：http://hz.yvedp.cn/gtyyubujlw.html

Java: s.indexOf("x")
来源：http://hz.jyoumei.cn/gtsdpfzqlx.html

Go:   strings.Index(s, "x")
来源：http://hz.jqgfzy.top/gtzsqajppq.html

Ruby: s.index("x")
来源：http://hz.cucudq.cn/gtcnpioswj.html

C#:   s.IndexOf("x")
来源：http://hz.hywenlv.cn/gtanwfccdn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xuanzx.com/gthqhnnzyb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shanyushiyangkeji.top/gtrkfpnhjq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jiagoushi.top/gtwmocvoss.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hongshengwenyu.top/gtvnjenaly.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.smart0.xyz/gtzylynisc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hysaishi.cn/gtnyblzebf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.haohaochexian.top/gthqoxhddd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xinyue.icu/gtouwguagp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinqigufen.top/gtvctvvdhy.html

[E06] 替换子串
来源：http://hz.jiagoushi.top/gtdlqrkvvq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhoulong.xyz/gtsylwnjhh.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shuidangran.top/gtyngyasgm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gtewveytde.html

TS:   s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtoxyhcikw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.quarkkingdee.top/gtihshfklt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jinqigufen.top/gtqhwgvraa.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.gotoacloud.top/gtegvuknhf.html

C#:   s.Replace("a", "b")
来源：http://hz.ydzc1.top/gtiwrowlsh.html

[E07] 按分隔符拆分
来源：http://hz.mhx1999.top/gtoobitfdu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhiwuduotai.top/gtrdjsvjll.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hnqzz.top/gtplrkryoa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jianghu66.top/gtjwmvtakp.html

TS:   s.split(",")
来源：http://hz.daxiang520.top/gtgrcjsmuh.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhixingplan.top/gtmcmhvcjg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.tian-w.cn/gtddagqnwg.html

Ruby: s.split(",");  s.split
来源：http://hz.svipenyu.cn/gtxwpvjibp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.haohaochexian.top/gtbqogpuaa.html

[E08] 数组按分隔符合并
来源：http://hz.sysykeji.top/gttizvrtnk.html

Py:   ",".join(items)
来源：http://hz.zhongyouzk.top/gtjtjyjakx.html

PHP:  implode(",", $items);
来源：http://hz.yj20258888.top/gtryyochon.html

JS:   items.join(",")
来源：http://hz.9152youxi.cn/gttdhddlbj.html

TS:   items.join(",")
来源：http://hz.quarkkingdee.top/gtzauppeuo.html

Java: String.join(",", items)
来源：http://hz.yanxiufei.cn/gtrhjmidhw.html

Go:   strings.Join(items, ",")
来源：http://hz.haohaochexian.top/gtiphpgktn.html

Ruby: items.join(",")
来源：http://hz.shuidangran.top/gtfakhniew.html

C#:   string.Join(",", items)
来源：http://hz.zhaomingkeji.xyz/gtjmrswqxh.html

[E09] 去除所有空白字符
来源：http://hz.kuanghao11.cn/gtfumzdxtl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.pycfn.com/gtjetrzsyq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.wangshuangyany.cn/gtvqocbjwp.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangkeji.top/gtdeoeohxc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.0kj1m.cn/gteyadgkqs.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yj20258.top/gtltyusobw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cucudq.cn/gtarosdsti.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.daria6918.cn/gtjurkkrkn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.iojbl.cn/gtrmwqszep.html

[E10] 左侧补零 / 定长填充
来源：http://hz.quarkkingdee.top/gtgllcfnqf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.sxryk.cn/gtjvjooljp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yj202588.top/gtakjcqflb.html

JS:   "7".padStart(3, "0")
来源：http://hz.nwbrower.top/gtrblzaiey.html

TS:   "7".padStart(3, "0")
来源：http://hz.yangfankeji.com/gtkktxvgkz.html

Java: String.format("%03d", 7)
来源：http://hz.gogol.net.cn/gtyhbzmepu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cashguo.top/gtghavwgia.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ybcxt.top/gtngwblrzx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinghuilouyu.cn/gtuhfrbyro.html

[E11] 反转字符串
来源：http://hz.cucudq.cn/gtgjchuhuv.html

Py:   s[::-1]
来源：http://hz.havefunace.top/gtozranxha.html

PHP:  strrev($s);
来源：http://hz.vqdsnc.cn/gtaasbthck.html

JS:   [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtyojywnxc.html

TS:   [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gttkyezhlp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zdqjudy.top/gtybfbcsko.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hfpthk.cn/gtklyhpvho.html

Ruby: s.reverse
来源：http://hz.ppjwa.cn/gtuzoqthib.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.chenzaomai.com/gtmvkowweu.html

[E12] 统计某字符出现次数
来源：http://hz.zhengqikj.top/gtlbizoaxm.html

Py:   s.count("a")
来源：http://hz.svipenyu.cn/gtnrxflrme.html


<!-- 参考信息 -->