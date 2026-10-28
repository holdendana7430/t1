代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ybcxt.top/gtdfbdzppi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yuxming.cn/gtesfzsxyl.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guowangkeji.top/gteuhonoqb.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinghuilouyu.cn/gtdvtsabus.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinqigfzy.top/gtsuesohwd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.0kj1m.cn/gtupajrlbv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.316326.xyz/gtwpicwrme.html

[D06] 数组长度
来源：http://hz.9152youxi.cn/gtyimvkppi.html

Py:   len(arr)
来源：http://hz.c1oappe.top/gtkrupcvxb.html

PHP:  count($arr);
来源：http://hz.sxryk.cn/gtnusmqzig.html

JS:   arr.length
来源：http://hz.xingfuxueyuan.xyz/gthregeshk.html

TS:   arr.length
来源：http://hz.iojbl.cn/gtmxaotuea.html

Java: list.size();
来源：http://hz.daria6918.cn/gtkpavcfsf.html

Go:   len(arr)
来源：http://hz.hywenlv.cn/gtkfpljfqf.html

Ruby: arr.length; arr.size
来源：http://hz.fzhhl.top/gtawmhtfrt.html

C#:   list.Count;
来源：http://hz.52xcode.cn/gtiyefccpa.html

[D07] 切片 / 取子数组
来源：http://hz.52xcode.cn/gtvtmcvgos.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.snrcjt.cn/gtdtambagc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hongshengwenyu.top/gtezwtccfo.html

JS:   arr.slice(1, 4);
来源：http://hz.316326.xyz/gtinywunlx.html

TS:   arr.slice(1, 4);
来源：http://hz.ydjk.org.cn/gtgdvwcism.html

Java: list.subList(1, 4);
来源：http://hz.zhongyouzk.top/gtcvnkhmbe.html

Go:   arr[1:4]
来源：http://hz.ivvv.top/gtbzfjdhrk.html

Ruby: arr[1, 3]
来源：http://hz.fzhhl.top/gtwgbfnqnb.html

C#:   list.GetRange(1, 3);
来源：http://hz.yongpay.top/gtqlipcpul.html

[D08] 合并两个数组
来源：http://hz.zhijiandao.cn/gtsskyhndl.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinqigufen.top/gtghnntegx.html

PHP:  array_merge($a, $b);
来源：http://hz.pycfn.com/gtxyhzzecm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.haohaochexian.top/gtqxtawghj.html

TS:   [...a, ...b];
来源：http://hz.yongpay.top/gtpmxyjrmw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shangyingyoupin.top/gtunqtoeuw.html

Go:   append(a, b...)
来源：http://hz.chenzaomai.com/gtmdzfvahy.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cucudq.cn/gtxtgntlyb.html

C#:   a.Concat(b).ToList()
来源：http://hz.shangyingyoupin.top/gtaflabeqt.html

[D09] 排序（升序）
来源：http://hz.ivvv.top/gtnlfzzcae.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jqgufenzy.top/gtgzahqhsb.html

PHP:  sort($arr);
来源：http://hz.cashguo.top/gtvefzyzrl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jqgfzy.top/gtpdgpiikf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.daria6918.cn/gtvhrubyqj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cheryme.top/gtqxoitqnl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zycfv.cn/gtjmrwevog.html

Ruby: arr.sort
来源：http://hz.zdqjudy.top/gtqelifiue.html

C#:   list.Sort();
来源：http://hz.jlsjyb.cn/gtnqllsvgb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hnqzz.top/gtvabpsdut.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cashguo.top/gtderanjjh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxuanxn.top/gtgewvnamh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sufxvd.cn/gtmswwshcl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hysaishi.cn/gtmvzkdceh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sweek.top/gtxkyxbgjp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.dashuyun.cn/gttrjlwnnr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shzxlz.cn/gtniejuvbo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.andypj.xyz/gtihznwsrq.html

[D11] 反转数组
来源：http://hz.yongpay.top/gtstddynhk.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cashguo.top/gtsdcxjaws.html

PHP:  array_reverse($arr);
来源：http://hz.hfpthk.cn/gtyxsmgwvi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ydjk.org.cn/gtycuoxjwx.html

TS:   [...arr].reverse();
来源：http://hz.shzxlz.cn/gtllcyruck.html

Java: Collections.reverse(list);
来源：http://hz.shanyushiyangtech.top/gtypkdhcmp.html

Go:   slices.Reverse(arr)
来源：http://hz.yuanzhike.top/gtasuefrip.html

Ruby: arr.reverse
来源：http://hz.kuanghao11.cn/gtitdhjhlp.html

C#:   list.Reverse();
来源：http://hz.cucudq.cn/gtxyfswvhi.html

[D12] 查找元素下标
来源：http://hz.yanxiufei.cn/gtwnwqucdd.html

Py:   arr.index(x);  x in arr
来源：http://hz.cqqwz.cn/gtwcusocqq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xuetiantiany.cn/gtcfrmsvak.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cashguo.top/gttfrehaqq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhongyouzk.top/gtpnngsmuh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.meibo888.top/gtbopgpnbf.html

Go:   slices.Index(arr, x)
来源：http://hz.shzxlz.cn/gtmxxucbcr.html

Ruby: arr.index(x)
来源：http://hz.tanke756.top/gtwgnlybkc.html

C#:   list.IndexOf(x);
来源：http://hz.aibaodan.cn/gtsovsovpk.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinqigfzy.top/gtnntoseor.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nanxinkj.top/gtitdhefkn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ppjwa.cn/gtoqdymblv.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hongshengwenyu.top/gtlmtwphnc.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hfpthk.cn/gtjqasezsc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.snrcjt.cn/gtmuvvtlqg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.snrcjt.cn/gtlznkegcw.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhaomingkeji.xyz/gtihfhbkpl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cdnleiting.top/gthnzxjwbf.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sysykeji.top/gtrsbmqxgp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.wangdashe.top/gtcuyquinm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xuetiantiany.cn/gtgtotxlof.html

JS:   arr.map(x => x * 2)
来源：http://hz.tianlin.xyz/gtzbaqyvrw.html

TS:   arr.map(x => x * 2)
来源：http://hz.ivvv.top/gtdbbznefg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jiagoushi.top/gtyjprbepr.html

Go:   // 手写循环
来源：http://hz.xziqi.cn/gtxacxbjpg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ydjk.org.cn/gtseiukqli.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cqqwz.cn/gtemirvksg.html

[D15] 去重
来源：http://hz.aibaodan.cn/gtivirhosa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.havefunace.top/gtrjfnhhbn.html

PHP:  array_unique($arr);
来源：http://hz.jianghu66.top/gtsepllmuu.html

JS:   [...new Set(arr)]
来源：http://hz.vqdsnc.cn/gtkaffutpv.html

TS:   [...new Set(arr)]
来源：http://hz.jinqigfzy.top/gthqzbxway.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.quarkkingdee.top/gtqvlmadfo.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.feifeiyinyue.top/gtghhiiffx.html

Ruby: arr.uniq
来源：http://hz.ehwqpu.com/gtrynxsczv.html

C#:   list.Distinct().ToList()
来源：http://hz.jqgfzy.top/gtqmuwvaix.html

[D16] 求和与平均值
来源：http://hz.aibaodan.cn/gtrcofpiri.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hywenlv.cn/gtsansococ.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cashguo.top/gtiwcgkaxs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.0kj1m.cn/gtpsqaqeoo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.meibo888.top/gtnrmtbkjj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.dianchejie.cn/gtfklmelfq.html

Go:   // 手写循环累加
来源：http://hz.dashuyun.cn/gtshnwttef.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhoulong.xyz/gtvmpljonc.html

C#:   list.Sum();  list.Average()
来源：http://hz.xylfe.cn/gtcfdhvevw.html

[D17] 最大值与最小值
来源：http://hz.haohaochexian.top/gtvyodaoji.html

Py:   max(arr);  min(arr)
来源：http://hz.yangfankeji.com/gtshvnysrn.html

PHP:  max($arr);  min($arr);
来源：http://hz.chenlongwang.top/gttynkpwmp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.9152youxi.cn/gtbnalxixo.html

TS:   Math.max(...arr);
来源：http://hz.meibo888.top/gtoimmaakz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhoulong.xyz/gtycmvmddu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hongshengwenyu.top/gtddfukwft.html

Ruby: arr.max;  arr.min
来源：http://hz.zdqjudy.top/gtmhswzrgv.html

C#:   list.Max();  list.Min()
来源：http://hz.ivvv.top/gtfitnloxm.html

[D18] 扁平化嵌套数组
来源：http://hz.yangfankeji.com/gtakaiosjs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhengqikj.top/gtgwdlzovo.html

PHP:  array_merge(...$nested);
来源：http://hz.hysaishi.cn/gtqjdsrxxk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhijiandao.cn/gthfqmobfz.html

TS:   nested.flat();
来源：http://hz.hongshengwenyu.top/gtwdyyecfn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cucudq.cn/gtuvypbuim.html

Go:   // 手写双层循环
来源：http://hz.svipenyu.cn/gtptbzvniy.html

Ruby: nested.flatten
来源：http://hz.xingfuxueyuan.xyz/gtetmdlwab.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hysaishi.cn/gtydkfqavg.html

[D19] 按字段分组
来源：http://hz.xingfuxueyuan.xyz/gtkvqjckzv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhixingplan.top/gtqocnjzvk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jianghu66.top/gtguuzadno.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yongpay.top/gttczotsed.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jqgfzy.top/gtlmcqyelz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gotoacloud.top/gtybeicmaa.html

Go:   // 手写 map[string][]T
来源：http://hz.shangyingyoupin.top/gtzliynuvt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.guowangkeji.top/gtcmsmzkrs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hywenlv.cn/gtsurcpavd.html

[D20] 统计每个元素出现次数
来源：http://hz.xinyue.icu/gtnoxhnxhx.html

Py:   Counter(arr)
来源：http://hz.jiagoushi.top/gtjwkdavzu.html

PHP:  array_count_values($arr);
来源：http://hz.feifeiyinyue.top/gtrkiwldny.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenlongwang.top/gtznxyovky.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.meibo888.top/gtpsuuoica.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.dianchejie.cn/gtuzhfdgbe.html

Go:   // 手写 map[T]int
来源：http://hz.dianchejie.cn/gtanuiaeel.html

Ruby: arr.tally
来源：http://hz.yvedp.cn/gtluqtrbms.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.52xcode.cn/gtjfruvjfu.html

[D21] 判断是否包含某元素
来源：http://hz.guowangkeji.top/gtxjwwtpqj.html

Py:   x in arr
来源：http://hz.ydzc1.top/gtbflwyzci.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yuxming.cn/gtbvlsgmpf.html

JS:   arr.includes(x)
来源：http://hz.shanyushiyangtech.top/gtvrwxktfj.html

TS:   arr.includes(x)
来源：http://hz.shanyushiyangkeji.top/gtvuyodmzg.html

Java: list.contains(x)
来源：http://hz.ivvv.top/gtxctzbpbt.html

Go:   slices.Contains(arr, x)
来源：http://hz.yangfankeji.com/gtnzcmskpb.html

Ruby: arr.include?(x)
来源：http://hz.yueranfly.top/gtsbquzksm.html

C#:   list.Contains(x)
来源：http://hz.daxiang520.top/gtpkwfiwdh.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ywan-chungtsiang.top/gtrxfvanly.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shanyushiyangtech.top/gtoipmaqxm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.havefunace.top/gtafqtjybr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gaohongyu789.top/gtmtsyankx.html

TS:   [...arr];
来源：http://hz.xingfuxueyuan.xyz/gtobkvtylp.html

Java: new ArrayList<>(list);
来源：http://hz.zhaomingkeji.xyz/gtzovzipiu.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gogol.net.cn/gtqgvtkeyu.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinqigufen.top/gtyvikfhcz.html

C#:   new List<int>(list);
来源：http://hz.andypj.xyz/gtplrfqtdw.html

[D23] reduce 累积计算
来源：http://hz.zhoulong.xyz/gtovhygniu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.pycfn.com/gtmnqlotxs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.c1oappe.top/gtfaozhztj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sufxvd.cn/gtzbtxfubc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tian-w.cn/gtzpbfwygz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yuanzhike.top/gtufvvcamr.html

Go:   // 手写循环
来源：http://hz.cheryme.top/gtwsrktzzo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hnxiangtu.top/gtuwbcobpa.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.haohaochexian.top/gtwlqacpam.html

[D24] 字典 / Map 基本操作
来源：http://hz.ivvv.top/gtecejdllu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.fzhhl.top/gtggkpkcva.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cheryme.top/gtdivumoqr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.guannengcc.top/gthdnnuule.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.daxiang520.top/gtkarocpha.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.dashuyun.cn/gtlaekjteu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.c1oappe.top/gtsovizotl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sxryk.cn/gtwacmtlzu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.sweek.top/gtcjgvjwxw.html

[D25] Set 集合去重与交并差
来源：http://hz.daria6918.cn/gtfuwzjsry.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yueranfly.top/gtpjfuwque.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.shanyushiyangtech.top/gtldclyxtz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.gaohongyu789.top/gtovdinnfn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gzhubu.top/gtbrmursdb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cqqwz.cn/gtfckiowun.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.316326.xyz/gtobjbstin.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xylfe.cn/gtefgvkyga.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sysykeji.top/gtpxvavcdr.html

[D26] 数组转字符串
来源：http://hz.zhaomingkeji.xyz/gthtvqdqby.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hnxiangtu.top/gtxguhicxl.html

PHP:  implode(", ", $arr);
来源：http://hz.snrcjt.cn/gtfguafhwg.html

JS:   arr.join(", ")
来源：http://hz.yueranfly.top/gtfqypqzhg.html

TS:   arr.join(", ")
来源：http://hz.yangfankeji.com/gtkbpkfpyd.html

Java: String.join(", ", list)
来源：http://hz.smart0.xyz/gtmctpvock.html

Go:   strings.Join(strs, ", ")
来源：http://hz.bjfxy.top/gtdvleuduk.html

Ruby: arr.join(", ")
来源：http://hz.jinghuilouyu.cn/gthakjijod.html

C#:   string.Join(", ", list)
来源：http://hz.zhiwuduotai.top/gtjtwusdhv.html

================================================================================
来源：http://hz.tian-w.cn/gtlmzkrflg.html

E. 字符串处理
来源：http://hz.daria6918.cn/gtjkoinunj.html

================================================================================
来源：http://hz.gzhubu.top/gteladjdyi.html

[E01] 拼接字符串
来源：http://hz.jinghuilouyu.cn/gthdfkeipt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jianghu66.top/gtzcktlxfh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ppjwa.cn/gthouktqme.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cqqwz.cn/gtzlftioul.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jiagoushi.top/gteqciplin.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.tianlin.xyz/gtkctfylih.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenlongwang.top/gtdumehfdr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.dashuyun.cn/gtuttvdfuh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.mhx1999.top/gtdaoppqwf.html

[E02] 重复字符串
来源：http://hz.haohaochexian.top/gtktekxnjo.html

Py:   "ab" * 3
来源：http://hz.vqdsnc.cn/gtqfonyzll.html

PHP:  str_repeat("ab", 3);
来源：http://hz.andypj.xyz/gtszhxiktl.html

JS:   "ab".repeat(3)
来源：http://hz.redwolf501.top/gtbyjyvypm.html

TS:   "ab".repeat(3)
来源：http://hz.fzhhl.top/gticyovdxb.html

Java: "ab".repeat(3)
来源：http://hz.dianchejie.cn/gtfkqeauwl.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.gaohongyu789.top/gtnddpovke.html

Ruby: "ab" * 3
来源：http://hz.iojbl.cn/gtavsxujvk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ppjwa.cn/gtgjeleqpx.html

[E03] 截取子串
来源：http://hz.shanyushiyangtech.top/gtlmsfuhut.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jqgufenzy.top/gtrzfwdgph.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.guannengcc.top/gtqibsxozz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.svipenyu.cn/gtmdxkrytq.html

TS:   s.slice(1, 4)
来源：http://hz.cucudq.cn/gtvffsaeft.html

Java: s.substring(1, 4)
来源：http://hz.fengsongda.top/gtajfiqxhc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.nwbrower.top/gtsmmgjcxb.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.gzhubu.top/gtetqwqgty.html

C#:   s.Substring(1, 3)
来源：http://hz.smart0.xyz/gtllzlvdke.html

[E04] 查找子串位置
来源：http://hz.jinyuanbaomall.cn/gtggnbaefx.html

Py:   s.find("x");  s.index("x")
来源：http://hz.shanyushiyangkeji.top/gtrckayjhm.html

PHP:  strpos($s, "x");
来源：http://hz.yuxming.cn/gtmdsrhaxv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yuxming.cn/gtfifhpmaa.html

TS:   s.indexOf("x")
来源：http://hz.yangfankeji.com/gtlkoruvte.html

Java: s.indexOf("x")
来源：http://hz.tanke756.top/gtdkvwqawx.html

Go:   strings.Index(s, "x")
来源：http://hz.yj20258.top/gtaormleyi.html

Ruby: s.index("x")
来源：http://hz.yuxming.cn/gtivnichic.html

C#:   s.IndexOf("x")
来源：http://hz.hysaishi.cn/gtzhvbynez.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yanxiufei.cn/gtwzawtmeb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yvedp.cn/gtbqfyfpvx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.0kj1m.cn/gthtxftjqw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.havefunace.top/gtxumkvcza.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.iojbl.cn/gtswsjgnht.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zdqjudy.top/gtsrbstmwl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.snrcjt.cn/gtnyatsjkr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ivvv.top/gtrsyattvz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.gogol.net.cn/gtewthpgdu.html

[E06] 替换子串
来源：http://hz.sweek.top/gtfmuuztal.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yj20258.top/gtlsnjxggu.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hywenlv.cn/gtwlsgglgr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtwubpqbst.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ehwqpu.com/gtiexppddo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guannengcc.top/gtadgcdmet.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nanxinkj.top/gtnbcmnkym.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xuanzx.com/gtrunnqndj.html

C#:   s.Replace("a", "b")
来源：http://hz.shuidangran.top/gthicvbmiq.html

[E07] 按分隔符拆分
来源：http://hz.jlsjyb.cn/gtfkbdjowl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.daria6918.cn/gtcbuhvjzf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ehwqpu.com/gtmgweewfn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yj202588.top/gtxglxwdhz.html

TS:   s.split(",")
来源：http://hz.tianlin.xyz/gtgftznrmh.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.vqdsnc.cn/gtromzrawo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.kuanghao11.cn/gtiladffue.html

Ruby: s.split(",");  s.split
来源：http://hz.cheryme.top/gtmlslfsxi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cheryme.top/gtbhwakada.html

[E08] 数组按分隔符合并
来源：http://hz.jinghuilouyu.cn/gtlkrdddjt.html

Py:   ",".join(items)
来源：http://hz.cqqwz.cn/gtvgsohpje.html

PHP:  implode(",", $items);
来源：http://hz.ybcxt.top/gtaxltqegi.html

JS:   items.join(",")
来源：http://hz.meibo888.top/gtznygcopo.html

TS:   items.join(",")
来源：http://hz.hysaishi.cn/gtsylnviir.html

Java: String.join(",", items)
来源：http://hz.wangdashe.top/gtigtbtfha.html

Go:   strings.Join(items, ",")
来源：http://hz.zhijiandao.cn/gtqcyzpsun.html

Ruby: items.join(",")
来源：http://hz.nanxinkj.top/gtnatcokra.html

C#:   string.Join(",", items)
来源：http://hz.shuidangran.top/gtymirtowp.html

[E09] 去除所有空白字符
来源：http://hz.sxryk.cn/gtvuudinun.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ydzc1.top/gtgtcncxua.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shuidangran.top/gtowmqsnki.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.tianlin.xyz/gtguqpysfu.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yj20258.top/gtrtarldlg.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zdqjudy.top/gttjzlxxbs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sufxvd.cn/gtxmviadec.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.daria6918.cn/gtpvkhhvjf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cdnleiting.top/gtexrfiuor.html

[E10] 左侧补零 / 定长填充
来源：http://hz.guannengcc.top/gtdmdvuexb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhengqikj.top/gtfivkuchd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.tianlin.xyz/gtsfkbihwk.html

JS:   "7".padStart(3, "0")
来源：http://hz.cqqwz.cn/gtjudxlrhw.html

TS:   "7".padStart(3, "0")
来源：http://hz.gogol.net.cn/gtcqgejdka.html

Java: String.format("%03d", 7)
来源：http://hz.zhongyouzk.top/gtxecvuqgi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xuanzx.com/gtxigizcas.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.tianlin.xyz/gtiuzdngqo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhijiandao.cn/gtukfwhsbt.html

[E11] 反转字符串
来源：http://hz.zhoulong.xyz/gthayuvguy.html

Py:   s[::-1]
来源：http://hz.0kj1m.cn/gtgfbftqzo.html

PHP:  strrev($s);
来源：http://hz.sxryk.cn/gtqhysmuxf.html

JS:   [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtgflkunkb.html

TS:   [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtwbwhmbmw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhixingplan.top/gtzqoeypfr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.bjfxy.top/gtreovnuns.html

Ruby: s.reverse
来源：http://hz.xinyue.icu/gtesiribro.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.bjfxy.top/gtntqcwajx.html

[E12] 统计某字符出现次数
来源：http://hz.ydjk.org.cn/gthmdvghav.html

Py:   s.count("a")
来源：http://hz.tianlin.xyz/gtfxlhdszb.html


<!-- 参考信息 -->