代发 wailian999

Py:   len(arr)
来源：http://hz.jiagoushi.top/gtomgzybcd.html

PHP:  count($arr);
来源：http://hz.dashuyun.cn/gtyfagamaa.html

JS:   arr.length
来源：http://hz.xylfe.cn/gtahavxgew.html

TS:   arr.length
来源：http://hz.kuanghao11.cn/gturpejajm.html

Java: list.size();
来源：http://hz.yangfankeji.com/gtdkyjlbfk.html

Go:   len(arr)
来源：http://hz.jinqigufen.top/gtkcgsnfko.html

Ruby: arr.length; arr.size
来源：http://hz.yj20258.top/gtwdnanipn.html

C#:   list.Count;
来源：http://hz.hammf.cn/gtbdmtvyau.html

[D07] 切片 / 取子数组
来源：http://hz.xingfuxueyuan.xyz/gtijzhgkjq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sxryk.cn/gtbvurrcwj.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hnqzz.top/gtmdqyagxt.html

JS:   arr.slice(1, 4);
来源：http://hz.nanxinkj.top/gtatvriwge.html

TS:   arr.slice(1, 4);
来源：http://hz.redwolf501.top/gtjgkmzfgp.html

Java: list.subList(1, 4);
来源：http://hz.xingfuxueyuan.xyz/gtkrvnpocf.html

Go:   arr[1:4]
来源：http://hz.yj20258.top/gtnihiuwez.html

Ruby: arr[1, 3]
来源：http://hz.jinghuilouyu.cn/gtiglpbfug.html

C#:   list.GetRange(1, 3);
来源：http://hz.shanyushiyangtech.top/gtlcqcomed.html

[D08] 合并两个数组
来源：http://hz.yvedp.cn/gthlmauczo.html

Py:   a + b;  a.extend(b)
来源：http://hz.yuanzhike.top/gtphcoqphv.html

PHP:  array_merge($a, $b);
来源：http://hz.0kj1m.cn/gtfccvebga.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhongyouzk.top/gtbznttsvq.html

TS:   [...a, ...b];
来源：http://hz.vqdsnc.cn/gtqvjffcqe.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sweek.top/gtwxoseert.html

Go:   append(a, b...)
来源：http://hz.gaohongyu789.top/gtnipxizxu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ivvv.top/gthwyjlupr.html

C#:   a.Concat(b).ToList()
来源：http://hz.haohaochexian.top/gttuaffnlu.html

[D09] 排序（升序）
来源：http://hz.tianlin.xyz/gthfrmliee.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinghuilouyu.cn/gtcwgfeqis.html

PHP:  sort($arr);
来源：http://hz.52xcode.cn/gtqpqvvsmi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yuanzhike.top/gtqpiprlik.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cdnleiting.top/gtizccvvfp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.wangdashe.top/gtuzkimipa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.snrcjt.cn/gtvsftzzsn.html

Ruby: arr.sort
来源：http://hz.mhx1999.top/gtcxwikjfn.html

C#:   list.Sort();
来源：http://hz.jiagoushi.top/gtvxojqrzc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gotoacloud.top/gtzxtargpf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yanxiufei.cn/gtzlhtvdoc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.sufxvd.cn/gtbednwdds.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.haohaochexian.top/gtlrrixluu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yueranfly.top/gtrkhjlxfq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yonumen.top/gtgdhqpeet.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zycfv.cn/gtdjvixzxz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shanyushiyangtech.top/gtqfouaipw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.mhx1999.top/gtmhhqxyvp.html

[D11] 反转数组
来源：http://hz.jianghu66.top/gtxwvavisr.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.pycfn.com/gtwsbwaqvc.html

PHP:  array_reverse($arr);
来源：http://hz.daxiang520.top/gtkeqkevsk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.cqqwz.cn/gtmcmijrgu.html

TS:   [...arr].reverse();
来源：http://hz.cqqwz.cn/gtrmjsqwvz.html

Java: Collections.reverse(list);
来源：http://hz.hnqzz.top/gtxzxfkqoo.html

Go:   slices.Reverse(arr)
来源：http://hz.jiagoushi.top/gtubhwxnxc.html

Ruby: arr.reverse
来源：http://hz.jqgfzy.top/gtciowqwyp.html

C#:   list.Reverse();
来源：http://hz.zhoulong.xyz/gtyjopsxgk.html

[D12] 查找元素下标
来源：http://hz.ppjwa.cn/gtdljeelhd.html

Py:   arr.index(x);  x in arr
来源：http://hz.jiagoushi.top/gtbdakwffd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.nwbrower.top/gtkynlbduq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.andypj.xyz/gtrdpquyqs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuxming.cn/gtzzhpfsmp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yj20258.top/gtzvqujfku.html

Go:   slices.Index(arr, x)
来源：http://hz.pycfn.com/gtwunrckxv.html

Ruby: arr.index(x)
来源：http://hz.smart0.xyz/gtoqvanigf.html

C#:   list.IndexOf(x);
来源：http://hz.shzxlz.cn/gtonmrqyxp.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yongpay.top/gtjxesfvjc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yonumen.top/gtruutuswh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ivvv.top/gtqjzduzde.html

JS:   arr.filter(x => x > 3)
来源：http://hz.aizwys.cn/gttlkamope.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xinyue.icu/gtxdbssnxv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.haohaochexian.top/gtpybeabbh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.daria6918.cn/gtlvxwxypj.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hywenlv.cn/gtlefxkehs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.smart0.xyz/gtqoxsbckn.html

[D14] 映射转换（每个元素变形）
来源：http://hz.fzhhl.top/gtzobthqfh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.316326.xyz/gthksmmjwe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yj202588.top/gtunpboqri.html

JS:   arr.map(x => x * 2)
来源：http://hz.quarkkingdee.top/gtllsrhaxp.html

TS:   arr.map(x => x * 2)
来源：http://hz.yuxming.cn/gtuobwtyxz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.andypj.xyz/gtfjtulnav.html

Go:   // 手写循环
来源：http://hz.cheryme.top/gtkhdsddov.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhijiandao.cn/gtesvnvuuh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jlsjyb.cn/gtvtbmjgut.html

[D15] 去重
来源：http://hz.cqqwz.cn/gtfzqwkbpf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhongyouzk.top/gtxvdvldne.html

PHP:  array_unique($arr);
来源：http://hz.smart0.xyz/gtlpklgtnw.html

JS:   [...new Set(arr)]
来源：http://hz.cdnleiting.top/gtriemucgh.html

TS:   [...new Set(arr)]
来源：http://hz.jianghu66.top/gtntfvrhzz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ppjwa.cn/gtuufxpsoy.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.haohaochexian.top/gtmzpuhhin.html

Ruby: arr.uniq
来源：http://hz.jiagoushi.top/gthgryhupz.html

C#:   list.Distinct().ToList()
来源：http://hz.iojbl.cn/gtfffhprus.html

[D16] 求和与平均值
来源：http://hz.shangyingyoupin.top/gtwiooyujz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.daria6918.cn/gthazoauue.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.dashuyun.cn/gtkczmurxw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnqzz.top/gtkvbumyei.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgfzy.top/gtqpcmrvol.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.c1oappe.top/gtmjinlfsr.html

Go:   // 手写循环累加
来源：http://hz.wangdashe.top/gtwflwqsen.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xylfe.cn/gtfkbffqyv.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhiwuduotai.top/gtadfqcfvb.html

[D17] 最大值与最小值
来源：http://hz.wangdashe.top/gtnqhqtgaj.html

Py:   max(arr);  min(arr)
来源：http://hz.dianchejie.cn/gtzmdyzzwe.html

PHP:  max($arr);  min($arr);
来源：http://hz.tanke756.top/gtzogjsnrh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gogol.net.cn/gtrhqvivuf.html

TS:   Math.max(...arr);
来源：http://hz.havefunace.top/gteimpjsmb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.bjfxy.top/gtcbywnsef.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xziqi.cn/gtjrgybxnk.html

Ruby: arr.max;  arr.min
来源：http://hz.yuxming.cn/gtqrrfxboy.html

C#:   list.Max();  list.Min()
来源：http://hz.chenzaomai.com/gtchkdgfxs.html

[D18] 扁平化嵌套数组
来源：http://hz.zhijiandao.cn/gtxlygwwiv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yj202588.top/gtdeiahtcb.html

PHP:  array_merge(...$nested);
来源：http://hz.jlsjyb.cn/gtizfqbhby.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yj20258.top/gtrmyjdgyt.html

TS:   nested.flat();
来源：http://hz.aibaodan.cn/gtfszsobap.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yongpay.top/gtnqyekink.html

Go:   // 手写双层循环
来源：http://hz.zycfv.cn/gtjsgrpyoh.html

Ruby: nested.flatten
来源：http://hz.yuanzhike.top/gtducvtjpt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhaomingkeji.xyz/gtjaehkuzy.html

[D19] 按字段分组
来源：http://hz.quarkkingdee.top/gtnasdjucx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinghuilouyu.cn/gtstdlrbfh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ehwqpu.com/gtvwayxmws.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhaomingkeji.xyz/gtjelwcazh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.c1oappe.top/gtkqshxnkd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ehwqpu.com/gtrgspynvl.html

Go:   // 手写 map[string][]T
来源：http://hz.daxiang520.top/gtoldenkyn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ivvv.top/gtosppnwiw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cdnleiting.top/gtsvwravix.html

[D20] 统计每个元素出现次数
来源：http://hz.daxiang520.top/gtpvowrnsf.html

Py:   Counter(arr)
来源：http://hz.hongshengwenyu.top/gtkairrvlb.html

PHP:  array_count_values($arr);
来源：http://hz.jinqigfzy.top/gtdlytdwst.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.birdmap.top/gtqnmuaqkv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zycfv.cn/gtrmexqdiw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shuidangran.top/gtzfyhltod.html

Go:   // 手写 map[T]int
来源：http://hz.52xcode.cn/gtcztszvxi.html

Ruby: arr.tally
来源：http://hz.hongshengwenyu.top/gthxligjrp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhijiandao.cn/gthsntsqdm.html

[D21] 判断是否包含某元素
来源：http://hz.pycfn.com/gtpfdrjsrz.html

Py:   x in arr
来源：http://hz.gaohongyu789.top/gtnpxtgboh.html

PHP:  in_array($x, $arr, true);
来源：http://hz.dianchejie.cn/gtvzbubngy.html

JS:   arr.includes(x)
来源：http://hz.shanyushiyangtech.top/gtzigskdbp.html

TS:   arr.includes(x)
来源：http://hz.dianchejie.cn/gtiqrkrmce.html

Java: list.contains(x)
来源：http://hz.cqqwz.cn/gtpaydrgvz.html

Go:   slices.Contains(arr, x)
来源：http://hz.wangdashe.top/gtofowvnfc.html

Ruby: arr.include?(x)
来源：http://hz.ehwqpu.com/gttowudela.html

C#:   list.Contains(x)
来源：http://hz.c1oappe.top/gtiibrspjr.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zycfv.cn/gtqlputxnr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.kuanghao11.cn/gtvsarznxt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.gogol.net.cn/gtgutlqyhj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hfpthk.cn/gtzaboqlpr.html

TS:   [...arr];
来源：http://hz.quarkkingdee.top/gtpxlhzvch.html

Java: new ArrayList<>(list);
来源：http://hz.jianghu66.top/gtfgzwdfwy.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.aibaodan.cn/gtfsgsgygx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cqqwz.cn/gtnixmowjz.html

C#:   new List<int>(list);
来源：http://hz.kuanghao11.cn/gttxvgcrys.html

[D23] reduce 累积计算
来源：http://hz.pengpengdd.cyou/gtdiajhxtl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinghuilouyu.cn/gthyqkatep.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yangfankeji.com/gtropbqxgo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shzxlz.cn/gtadnfwjqa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenjidiqi.icu/gtmskrpwek.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.smart0.xyz/gtmfjdtoad.html

Go:   // 手写循环
来源：http://hz.jlsjyb.cn/gtpsesnmig.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yonumen.top/gtjjmroiej.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.fengsongda.top/gtedifhumr.html

[D24] 字典 / Map 基本操作
来源：http://hz.yonumen.top/gtkamiyyve.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.tian-w.cn/gtiaeznvwm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hnqzz.top/gtclhtcjir.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ehwqpu.com/gtmkoahvdq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zycfv.cn/gtclfscjcr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.dianchejie.cn/gtvffyczjj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhiwuduotai.top/gtwfryhuae.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.snrcjt.cn/gtdpavhggi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hnxiangtu.top/gtwynjgsmk.html

[D25] Set 集合去重与交并差
来源：http://hz.yangfankeji.com/gthlhiewmo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.c1oappe.top/gtrovygyeu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yonumen.top/gttaunwsws.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nanxuanxn.top/gtywkqmsgi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xuanzx.com/gtbtcrrmrb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.mhx1999.top/gtpidliwdg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hfpthk.cn/gtqsyoywyd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.mhx1999.top/gtxhlhbolt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yj20258.top/gtmybjolsi.html

[D26] 数组转字符串
来源：http://hz.xylfe.cn/gtncvptwpd.html

Py:   ", ".join(map(str, arr))
来源：http://hz.sweek.top/gtfjyzymbu.html

PHP:  implode(", ", $arr);
来源：http://hz.shangyingyoupin.top/gttkzvyfbk.html

JS:   arr.join(", ")
来源：http://hz.nanxuanxn.top/gtcewvtnny.html

TS:   arr.join(", ")
来源：http://hz.hfpthk.cn/gtdrdwaduy.html

Java: String.join(", ", list)
来源：http://hz.ywan-chungtsiang.top/gtnkiptgib.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yj20258888.top/gtqhlyustg.html

Ruby: arr.join(", ")
来源：http://hz.smart0.xyz/gthvlmqevv.html

C#:   string.Join(", ", list)
来源：http://hz.aibaodan.cn/gtuofnzjcl.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtdjlyqeuq.html

E. 字符串处理
来源：http://hz.tianlin.xyz/gtdayrhndm.html

================================================================================
来源：http://hz.chenlongwang.top/gtnbgnwril.html

[E01] 拼接字符串
来源：http://hz.dashuyun.cn/gtulmssnzo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.kuanghao11.cn/gtyoxysnig.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhengqikj.top/gtcvxgadjt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenzaomai.com/gtppskwagf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.fengsongda.top/gtgbtwltsb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.nanxinkj.top/gtagnrnobq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jiagoushi.top/gtyptutiyi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.guannengcc.top/gtyzubrlzs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtqwjypdxk.html

[E02] 重复字符串
来源：http://hz.sufxvd.cn/gtcjfwoncr.html

Py:   "ab" * 3
来源：http://hz.gogol.net.cn/gtipwrctqa.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yuxming.cn/gtxaynltwn.html

JS:   "ab".repeat(3)
来源：http://hz.guannengcc.top/gtowqjdghv.html

TS:   "ab".repeat(3)
来源：http://hz.zhixingplan.top/gtsjqsdvli.html

Java: "ab".repeat(3)
来源：http://hz.hfpthk.cn/gtercgfimt.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jqgufenzy.top/gtiehpmyex.html

Ruby: "ab" * 3
来源：http://hz.havefunace.top/gtzwftlshv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jyoumei.cn/gtbpqhhygs.html

[E03] 截取子串
来源：http://hz.bjfxy.top/gttgousfln.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.shanyushiyangkeji.top/gtatgrntlz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jqgfzy.top/gtistduxuz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.guowangkeji.top/gthdsqyogj.html

TS:   s.slice(1, 4)
来源：http://hz.jinqigfzy.top/gtdxvluvfx.html

Java: s.substring(1, 4)
来源：http://hz.xuetiantiany.cn/gtqesgsdrl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.chenzaomai.com/gttspgfdzn.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.wangdashe.top/gtpnzyuhid.html

C#:   s.Substring(1, 3)
来源：http://hz.aizwys.cn/gtgvqwbyex.html

[E04] 查找子串位置
来源：http://hz.redwolf501.top/gtgxcdwodp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.vqdsnc.cn/gtzpvdaqei.html

PHP:  strpos($s, "x");
来源：http://hz.hysaishi.cn/gtkrfrxgko.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.aibaodan.cn/gtsgpiremx.html

TS:   s.indexOf("x")
来源：http://hz.nwbrower.top/gtjjxrhcws.html

Java: s.indexOf("x")
来源：http://hz.hfpthk.cn/gtlwqardkj.html

Go:   strings.Index(s, "x")
来源：http://hz.xingfuxueyuan.xyz/gtvdbjwqsz.html

Ruby: s.index("x")
来源：http://hz.yueranfly.top/gteymoueac.html

C#:   s.IndexOf("x")
来源：http://hz.xuanzx.com/gtaxxdeapy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.9152youxi.cn/gtoepexpii.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.aizwys.cn/gtknaubnvp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.xingfuxueyuan.xyz/gtpnvscibb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xinyue.icu/gtizujsjvy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.chenzaomai.com/gtmdelrxeb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sxryk.cn/gtwzntckzi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hywenlv.cn/gtphjlvnwv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jqgufenzy.top/gtkvkaakvx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jianghu66.top/gtlpwleuwx.html

[E06] 替换子串
来源：http://hz.meibo888.top/gteqeyzyjx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hammf.cn/gtjilsgmfi.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.chenjidiqi.icu/gtxpiqjijb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.dashuyun.cn/gtytzvazkj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.dashuyun.cn/gtcrlydiui.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gtvuwkacgp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sweek.top/gtljgrpdzo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.nanxinkj.top/gtttrtrdre.html

C#:   s.Replace("a", "b")
来源：http://hz.zhaomingkeji.xyz/gthvopwxmd.html

[E07] 按分隔符拆分
来源：http://hz.daria6918.cn/gtmshalzxf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zycfv.cn/gtjsudazru.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.guowangkeji.top/gtwkxovdjl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.tanke756.top/gtxvkyxbtz.html

TS:   s.split(",")
来源：http://hz.yangfankeji.com/gtzvybobdf.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.tian-w.cn/gtitqfvcmq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.wangdashe.top/gtlxmkhssy.html

Ruby: s.split(",");  s.split
来源：http://hz.ehwqpu.com/gtwtojydgc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ywan-chungtsiang.top/gtwjzjpzaj.html

[E08] 数组按分隔符合并
来源：http://hz.tanke756.top/gtpkbeibbk.html

Py:   ",".join(items)
来源：http://hz.yvedp.cn/gtzqkftcsp.html

PHP:  implode(",", $items);
来源：http://hz.cdnleiting.top/gtnzsylwdv.html

JS:   items.join(",")
来源：http://hz.sxryk.cn/gtxmxnwolo.html

TS:   items.join(",")
来源：http://hz.pycfn.com/gtmgtpefje.html

Java: String.join(",", items)
来源：http://hz.hongshengwenyu.top/gtdcdkjdjv.html

Go:   strings.Join(items, ",")
来源：http://hz.9152youxi.cn/gtsaytfzxl.html

Ruby: items.join(",")
来源：http://hz.ehwqpu.com/gtawpeveis.html

C#:   string.Join(",", items)
来源：http://hz.aizwys.cn/gtlirjgfwt.html

[E09] 去除所有空白字符
来源：http://hz.guowangkeji.top/gtxnjftnkf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xylfe.cn/gttinlcabr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.andypj.xyz/gtphbbeqzr.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jyoumei.cn/gtltwmilbe.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ydjk.org.cn/gtumiumgyi.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shangyingyoupin.top/gtsjiqmqwx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.0kj1m.cn/gtatciglyh.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.aizwys.cn/gtcsxavosw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sweek.top/gtgfjplxjg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.shangyingyoupin.top/gtrpnpowcu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xuetiantiany.cn/gtxxnnzmkg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cheryme.top/gtxzijzeye.html

JS:   "7".padStart(3, "0")
来源：http://hz.dianchejie.cn/gtpfsslewb.html

TS:   "7".padStart(3, "0")
来源：http://hz.daxiang520.top/gtkxjxauji.html

Java: String.format("%03d", 7)
来源：http://hz.gaohongyu789.top/gtdwxxnqqj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.haohaochexian.top/gtmdwgaymm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj202588.top/gtodfuhvoa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hnxiangtu.top/gtctfnavom.html

[E11] 反转字符串
来源：http://hz.wangdashe.top/gtqptaozno.html

Py:   s[::-1]
来源：http://hz.zdqjudy.top/gthjrvczes.html

PHP:  strrev($s);
来源：http://hz.zhaomingkeji.xyz/gtzhfserin.html

JS:   [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtdiajdmfm.html

TS:   [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtvyxpeanw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinghuilouyu.cn/gtexgodugv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.svipenyu.cn/gtvaylaack.html

Ruby: s.reverse
来源：http://hz.dianchejie.cn/gtziumlfvx.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shuidangran.top/gtqjsvkhxa.html

[E12] 统计某字符出现次数
来源：http://hz.sufxvd.cn/gtfitfmxqp.html

Py:   s.count("a")
来源：http://hz.shangyingyoupin.top/gtnmmvnxwl.html

PHP:  substr_count($s, "a");
来源：http://hz.vqdsnc.cn/gtvuixslfh.html

JS:   s.split("a").length - 1
来源：http://hz.snrcjt.cn/gtkcwagzpw.html

TS:   s.split("a").length - 1
来源：http://hz.jinghuilouyu.cn/gtybqnrshd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.bjfxy.top/gtgsxpbwlv.html

Go:   strings.Count(s, "a")
来源：http://hz.tianlin.xyz/gtwqywbjmw.html

Ruby: s.count("a")
来源：http://hz.c1oappe.top/gtzqvvmews.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ivvv.top/gtuasurebj.html

[E13] 逐字符遍历
来源：http://hz.hammf.cn/gtszaeksow.html


<!-- 参考信息 -->